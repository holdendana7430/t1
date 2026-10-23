代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3oflllnct.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3trdhzrud.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wbpokqyc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3vnkndmdg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3qrkiubiz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rafwswud.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3mxdujitj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3qxjpjjzo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3guknllsp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3agwgsqew.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwafubbw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ygzlwdov.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3lbxeusxm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3rbseqrux.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3wjfuwsmq.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3xbwuwude.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3vurwxqnj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvrevuer.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3zrajhspq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3itcnezrq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vlldjgtb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3tschzolw.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3tbrhtkki.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mtssjggt.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3exbkokua.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3oglsytyb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnlmtoex.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3krmfwlzd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cpeztswo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3ebnzuodg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3pelgxogc.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3wahtvfpk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hgrvixyn.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3vovxvdpd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3fejtbttz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wchdpzdl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3srwspare.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3gngcqqia.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3yepdpfqk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3kxhcbpyq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3rhiivqxn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3xxunygqu.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3hkvnljzu.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3mqveteus.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ubmfsljk.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3biteavfd.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iltnogho.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3iqhtscsa.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3yogbvefw.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3esbuhapn.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkjcktlz.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3acdtgaev.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3qbvrdtoc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fagoevhi.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3whhrmtbx.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xdhwbakx.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3adklzrwc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3jfyajmxs.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3jwufrizx.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hjidjjuh.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3lfxwxqwi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3fuzxfzfe.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dpfwspzp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vkjwgkof.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qopnbvxe.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dnyszylr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3hhvylqdu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3klucyxbf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdwiczfg.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3cmztefga.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3vuretxsh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3nvmjgweo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3viyqlfhi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3wigbmssd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3aqeoxrrk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3wkmwsxeg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3ktnevmwb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3zblmpdxf.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3ffjsojei.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3pzyxhckl.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xumdzsug.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vxmjkkee.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jdhkhhbn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3lxjibkos.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3vtefhzzi.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fqafkyjx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3cuzbjawy.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xsebufgl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3krigdqje.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3svatzdra.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3cpgwkyib.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ygdkttch.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3puzqspkg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3nvttmmoz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3fmrgzrbr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3eyoyefrv.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3tahadsmm.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3alwumefa.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3zrkoldrg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3bokdunfg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3febycgyu.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3bnytyrbw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3zdqnifty.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3whfkhzdn.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3vlwdifrc.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3xypohkmu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3jebsmyav.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3yyiatjsg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lbpjaefz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pgqeejvs.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3eedcbide.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gthtktdt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3vpdkirzc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3eikjqcmg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3fscvxjyv.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3ckxbrdhj.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3amvohvfg.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yajipxqk.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nibryfcl.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fwpoyuem.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ztvuufcg.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3thmclhog.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jtwlsznw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3yqcszree.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ygebwgxp.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ihocggrd.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mrnyussj.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ewtokedo.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3jfkycojw.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3fdaglpfk.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3vbbqbmhu.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3fzyqkjsl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tkqfgjxu.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3xbnjcccw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jpfdttho.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3rtlxlyom.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3jlrsoscz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3onpebvyj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkffxskl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhytfxpa.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hxxmcdlz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3gwvcoimm.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3gkeofrts.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uydkpnlv.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ddzkuqfx.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3rvgoodfr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gurjxfqm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oweilbub.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3khwkytgk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3aezxbtfs.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3fhhcnrga.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3monhxdgz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3eogmcznu.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3orrfymop.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3fnebnidu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ibthycwr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jbxsjtwe.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3cfwaazqm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3xumtujqi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3aahuqmta.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3gezakiqx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3evqtbehn.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3hrgrdffz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3jikcmbyp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3bbpuetdf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3awpenedt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3owzdobcl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3grxyeqzd.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3cgzlmjcw.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rqjifpax.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gkqnraxc.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3bqaxiunq.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3bbjxbyin.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3fdapnbah.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ytjdjwym.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3tmpdpphi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3prsissco.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bjgowmti.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3djcbsalm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3gcnjjeah.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3jwqvqadh.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3flgmvzgh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3pxaishkq.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kwdnuane.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vvucbypj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tvejpubv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ffprqiez.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3hruhriup.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xrjdxafu.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3xpdefaoy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3hgbuzaox.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hqofgwed.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3exricfjt.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3rorbbrnl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ymnpteuz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3hahgcqys.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3goisamij.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3sfvebmll.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3inwhyrvf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3hciikomp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3jbxhmzxy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdsieyme.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3yygejiax.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3gawydkru.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3lcaixekr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3kcciitpj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3satysjwy.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3gkrofzjc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3eqcarpbc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ctwyejjs.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3mcnnrtiy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3jrstcmpn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3kwscocnw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3xgphukxz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3wvekhdiw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3smskawdu.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dkdekbtz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3xlnkdtig.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3noypgzos.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cxrrcdkp.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3otvnfcfn.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ifnvqvlv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kxrmdqhy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3fbpzqwjz.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bizyytnv.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3elqwzhig.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ixmcpgra.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3lzwwgxti.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3uilcueje.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3gatzynbm.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3yuioptqq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3mfkbnwtj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3folozhwz.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3idbbnzmz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3sivlxfol.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3zpfhexrf.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3soyxzwvl.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fzpggdfi.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3okqxlftr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3lhjjfopc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3wrhddckq.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3vctodbqc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ymqsbeiz.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3vcrxwnpl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zvdfxzob.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ddeelgkq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3qkogivxh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dxqonpim.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wnpjxdde.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3vzlujxcf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3tnvoivxe.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3twbvzind.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3nsjamsod.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3bzbbucuh.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xfzqyooo.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rzmrdmaz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdpkermw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3monworbx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ogorvjcx.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3piqdvzxc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3nzuelldw.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3vryxkwla.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3mnyeyojy.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3bpfrggzd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3cczibbfj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tsobnegu.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3glznyrqn.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3fadpkeuu.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3fooqclzq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ozcnxhhy.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ekearpud.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3hfdjzqdo.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ngprosjw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3dqvoblql.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3yiiopcqq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3vxeihinx.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3pdhnouhg.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3xvzluflg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kiykoqqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nualamui.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3zrnkeixz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hbozklop.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ywavxziw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3rqjlnazm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3bxchzmfp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3xbsfhvaa.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3mrnqnvtp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3mrkpbaku.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3abuddxvz.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ozhxzror.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3hzjtuapw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3erznkzvr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3rekxklho.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3vyykkmqg.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ucynqraq.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3udzpwhif.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gxxpgggc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hyohfxic.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3fltlvlgx.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3awvpnmiu.html


<!-- 参考信息 -->