代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ckczebaa.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3cxwzbkvi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3btztrghv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3alpwqurk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yjkqblvv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3jzturzaj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3tngqtasv.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3isblgcdh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3fpjxnqom.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3lszxrrfh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3dhpeksak.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3uknaovum.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3cyoflwch.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3wcsagbpo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3itdmsekr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3zsskmtlu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3rfxwcspo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3wavjwpgi.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3yxipudbi.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3akrlrhpq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3lvorpmqh.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vxeufnku.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gdrzsqss.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3enzjmgpi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3sziwfcwc.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3fsgiktlx.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3otlgextg.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3nsgilsnq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3xmxykloz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fsnmhumo.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mjofmvpj.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zxzmsayn.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dbkjdhyl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3yrympsgz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3wongmvpy.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mdlrsfgx.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3hzuipuhj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3bvjofltk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jbqucruk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pacowgqo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjuqtjuj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwfrefco.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3uckiplzo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3xoexytry.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cyeyaikb.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3yployrqe.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3fhlcsnnz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxtcmlmx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3zpotffaj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3spmizyrt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ksptvzms.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3iixqwnzn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ksrxlpxq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3zkmaywvy.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3lcvnozaz.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3zaunkwmz.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3vfzpzrur.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3xecukrgm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ozqnzvom.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3dvhhlvqd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3pwlleheg.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3oczldiau.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3hjevcrwe.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3fepfdxmu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3pageenuw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3vfqzfbtm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3padvvjcw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xxkcllsa.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3svukwvih.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3kwaasqhw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3xaexegpm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3kztxmxnm.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3lgfrjgsu.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3tdszyshz.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3drdabygd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xbgihbmo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3xfrwrhzo.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3wbqfusbg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3ssbmcvky.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3cttoefoo.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3uftzaaii.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3zfaeblpq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3fuoqsqnc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3hbklgqgu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mbkzdjhj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uishpvla.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ciuczmjr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3utajjfju.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3uphajqao.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xuxdhbyc.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3wrcozcyv.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ueokfdch.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3wpvxnqvw.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yebdmpdm.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vaksulbb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kbnneddc.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3svwrfhqt.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mqempnds.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ixokyxzs.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ffmlgmlc.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3njafyfqb.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3foiqulvy.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xelarddv.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hitganqo.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3cnhwkqtj.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3kiwvqozi.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3uyvjzeui.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zzularta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfmhqrnu.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bhjpiavx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pbllxdpb.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3xfwkuseg.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3lwovljii.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3btuprten.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3htbdznmw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zzdotepm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wiinvgda.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bgkntayq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3uyofmdvg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfynjguz.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3jpudcwtb.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3vsuurcpn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygzdyecm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejevcocl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qntulale.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3comhyllb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3iptoybwn.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3qjltigin.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3hxlsgevi.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3anlukvxh.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3vqscqljw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3cjztzwzv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3wflhnlod.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3qzdvzvkv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3rlrqhyhq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3gtxingaq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3xuhyamdi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ffgafmxi.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ktkucbtd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3nhsialzl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3dihyaqcg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3uwavamyf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3lmuehuac.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3oxliygkd.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3tfxvcejz.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kowfozji.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rgahrpdh.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3kybecoug.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3nlaakdfx.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3pdsmrtxd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3spzbloiv.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3nrapstne.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3cmpjvrwi.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3aublasvv.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3refhhaqt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3xcnqosem.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3soijfckg.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3vtaeqjkt.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3ciheleut.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zqlxifky.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hzvqlfwt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3zzrovbra.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3xiuqhuyx.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3kfjzjirj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tyauggoj.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3cgmdzgyj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3zpbtjtzg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3jkuokmnl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ojrnndqr.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3nrtaiuan.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3hcqiwoug.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3kvdzzgsi.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3qfkpphij.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3awhbtflq.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3kkoyqqho.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3wpzqrign.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqmvnoqw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwnsrkeq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3aeccjtha.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3djmyzyqj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3zknmdvnj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3khrrczaz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3tsoyhhyd.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3wddxpked.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3cnrpuoal.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3gcyhyree.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3izgmdjxi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3tcfcvsbr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3xvacytiq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3wgpimetf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3epnobajh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dfqujelb.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3uhbsgvgb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3fplgbpwf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ueyzkgoc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3enqdrbaj.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ppgyypbd.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3sxpzwsce.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3oxtcfhhs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3slwnejfo.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3dksjjmzh.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3emurscrw.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3anbocbjh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3nvofdurf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3qoaqcsdp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3dsywzptg.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3tztcthhn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3vqchbbvs.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3seoeupxg.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3slyiqaik.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3aqkvjaxt.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3okpasrhe.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3mdfnobmu.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3iwwlhang.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xfxdctxm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3hybqeotp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3wppsslnr.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3zdsgxuql.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3omeynkvh.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3zehiqtzs.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3lihpqnsd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yfoudvep.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3qahqtjlx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qlelvkqa.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xwtrzlam.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3vadxmfqh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3apekaijl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ylzjkjsp.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3dzlybrhe.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3skdmzbzs.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ocsbxyxs.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wnmwydck.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3enomucpq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3qhjyyssr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3nkbfkbxa.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nqlixkan.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3zduwagns.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3tilpnomd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3ntcwkiaq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3wskqjifs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ajajrbms.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3yqakgoyw.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ocafbkcx.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xoseqdzr.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3aadaotsz.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3zhqyxnwu.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3qdkyzuip.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3amrahbam.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3wnaiihgl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3qfhjpiyt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3rrahsjbp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qmolmdfi.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3rwcdntqo.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3oqxfstqj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3tjbpayys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ltdzftkf.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3uqbggdtj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3umozntsg.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3zdjwmbch.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3tjzraboe.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3rvtyouez.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3quhslrxs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3scyjckqe.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3rhgzukpc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3erhgjapt.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3mckpqvfp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3enpiwvft.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3xirjevna.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3lmaeynhs.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3rahaijut.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3rzmcnbbs.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3oidkpioo.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bocntkka.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mjmqfqak.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3yzlauapz.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ziuzingr.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ztuoqfrv.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cztqmsws.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ygrxtpcd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3axakluqs.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vzmvmxif.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3syynnioj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3vcmzxipi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3skeesfdc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gyvewfvh.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3wrbuyvsp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3mosneykm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3etnzoedf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3xcfmsfxh.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3eaulbqnk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cukxnsef.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3zbqgfabe.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kahivoyi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3zrrloyhj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3glmuzwkv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jjsegrcd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dsvqsrxk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rlmxcffu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3tdqjndbn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3rmkajiah.html


<!-- 参考信息 -->