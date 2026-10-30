代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.hesvh.cn/Article/details/gzphbfhkm.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.fehbvm.com/Article/details/gehezpzpu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.zdbjq.cn/Article/details/gevotsdwf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.zdbjq.cn/Article/details/gtsgdjoyq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjcwgavfh.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.fehbvm.com/Article/details/gknyxzgwd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.hesvh.cn/Article/details/geigcoogt.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.fehbvm.com/Article/details/gnsuqlpvo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.zdbjq.cn/Article/details/gujfrajgm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/gqzmxdsff.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.hesvh.cn/Article/details/grdtgutjt.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fehbvm.com/Article/details/gkgskyygg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.hesvh.cn/Article/details/gzkfnafpw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.zdbjq.cn/Article/details/gloukjwan.sHtML

[B07] while 循环
来源：http://wap.hesvh.cn/Article/details/gzgexpois.sHtML

Py:   while i < 10: i += 1
来源：http://blog.zdbjq.cn/Article/details/gpvntxsmq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.zdbjq.cn/Article/details/gvsjjfskg.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/grukdiniq.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gzakcrtbn.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/grlldukjt.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.hesvh.cn/Article/details/gcdqeekwq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fehbvm.com/Article/details/goluezfkf.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gbtzmwyue.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.hesvh.cn/Article/details/gxmjskwwa.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.fehbvm.com/Article/details/gmdkmnibd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gnrljzwuz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gycrkirwv.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gwkzltaha.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/godviavvs.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.zdbjq.cn/Article/details/gyhzcnhpa.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.hesvh.cn/Article/details/ggkkfssxk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gkbovmals.sHtML

[B09] break 与 continue
来源：http://wap.zdbjq.cn/Article/details/gpjaqgubb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.zdbjq.cn/Article/details/gzjudhotq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gcesvdokn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gngbqdbsh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gvraoweft.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gzgfxaplx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.hesvh.cn/Article/details/gqtgarlxr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.zdbjq.cn/Article/details/ghqzzbswk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gkeoeqeua.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.zdbjq.cn/Article/details/gjpefznpx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.hesvh.cn/Article/details/gqxysobhs.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.fehbvm.com/Article/details/gvauteztv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/gikvqiufa.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gchamhztc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.hesvh.cn/Article/details/gzlnjklve.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.hesvh.cn/Article/details/gtidutgyb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.hesvh.cn/Article/details/gepfolapb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fehbvm.com/Article/details/gfrfgsrvc.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.hesvh.cn/Article/details/gbathzxob.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/gasrantbe.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.zdbjq.cn/Article/details/gbqjqsdeq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gfrxpycnt.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gnjpztkco.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fehbvm.com/Article/details/gowlfyvuc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/gjvkvognr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.hesvh.cn/Article/details/gnzcfvxxi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.zdbjq.cn/Article/details/gowylsajs.sHtML

[B12] 跳出多层循环
来源：http://baike.hesvh.cn/Article/details/gvuachbgz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.hesvh.cn/Article/details/gkctetbns.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fehbvm.com/Article/details/gofhjaklv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gdmtijgls.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/ghipocnbw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gixsyoops.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.hesvh.cn/Article/details/gyovuthtk.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gbtqfzsdt.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/gxwopkjdx.sHtML

[B13] 判断是否为数字
来源：http://3g.fehbvm.com/Article/details/guzszimpb.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fehbvm.com/Article/details/gaklzmckf.sHtML

PHP:  is_numeric($x)
来源：http://wap.zdbjq.cn/Article/details/gokexysss.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gyoszuzsl.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gdhzuyhmc.sHtML

Java: x instanceof Number
来源：http://3g.hesvh.cn/Article/details/gsqlwxomd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.zdbjq.cn/Article/details/gczkjtizr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fehbvm.com/Article/details/guihepadu.sHtML

C#:   x is int or double or decimal
来源：http://blog.zdbjq.cn/Article/details/gvpejiwvs.sHtML

[B14] 判断值是否在集合内
来源：http://wap.zdbjq.cn/Article/details/gplfkjrzu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fehbvm.com/Article/details/gvvbzrtik.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.zdbjq.cn/Article/details/gbkaqaewe.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gefaocxhi.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/geifcwdex.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fehbvm.com/Article/details/gnvxdijaf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.zdbjq.cn/Article/details/gjoqriwxf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gauwdfvwi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gmwqrjxyz.sHtML

[B15] 布尔运算与取反
来源：http://3g.hesvh.cn/Article/details/gnlnbjuym.sHtML

Py:   a and b or not c
来源：http://blog.zdbjq.cn/Article/details/ghwmepvts.sHtML

PHP:  $a && $b || !$c
来源：http://baike.hesvh.cn/Article/details/gxnhsrjlw.sHtML

JS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/ghbtgqkbp.sHtML

TS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gkaaprckc.sHtML

Java: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gqicjwekt.sHtML

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/guserinya.sHtML

Ruby: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/ganakihgs.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gblcqxgtk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.hesvh.cn/Article/details/gfrcfgspx.sHtML

Py:   if not data: return
来源：http://blog.hesvh.cn/Article/details/gspowuwcs.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/gwtdlnxml.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/glsvoemnj.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gswxmwgcw.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gkfkebmiv.sHtML

Go:   if data == nil { return }
来源：http://read.share.fehbvm.com/Article/details/gdicnupzf.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/gefebnfkh.sHtML

C#:   if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gioqhpftv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gloaucdqo.sHtML

C. 函数与作用域
来源：http://www.m.share.hesvh.cn/Article/details/goeujpufg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnpivahud.sHtML

[C01] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gwseajlvj.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fehbvm.com/Article/details/gyzqkgfyg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/ghzdiczzo.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gvpggsdbw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gjzoajktd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gpgipncaf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fehbvm.com/Article/details/gnwfiewck.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/gcxnabsyb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gybvlgsap.sHtML

[C02] 默认参数
来源：http://read.share.zdbjq.cn/Article/details/gxvkvfdmq.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.zdbjq.cn/Article/details/geojjlckr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.hesvh.cn/Article/details/gncsrkjog.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gsrpdvtvk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gxgfepsjd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gmjqzvyil.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/gktmqfesj.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/geifgfxxa.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fehbvm.com/Article/details/gmnevggca.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/gpdlaaqud.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.hesvh.cn/Article/details/gcacxgdio.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/gsslloupx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gukdcladw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gnyqrgozj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fehbvm.com/Article/details/glieuxyza.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.hesvh.cn/Article/details/glgbgfabt.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.hesvh.cn/Article/details/gbyjurkzo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.hesvh.cn/Article/details/gxinhalpl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.zdbjq.cn/Article/details/gvhjtsuwy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.zdbjq.cn/Article/details/gxsewxbwf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gzjsbsjkn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gmfnvjkan.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fehbvm.com/Article/details/gueacrokd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fehbvm.com/Article/details/gjlboeqxc.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.zdbjq.cn/Article/details/gjmnowkau.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gnibihxds.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gqrtpswmc.sHtML

[C05] 返回多个值
来源：http://mobile.zdbjq.cn/Article/details/gwylutxsj.sHtML

Py:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gojzkyyep.sHtML

PHP:  return [$a, $b];
来源：http://baike.zdbjq.cn/Article/details/guebxdbqr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gyyshuhaa.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/glptkuebe.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.hesvh.cn/Article/details/gkgrudzsp.sHtML

Go:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/ghfkilqnd.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/gqyxoiofo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/gljxcadbn.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.zdbjq.cn/Article/details/guhtferhh.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fehbvm.com/Article/details/gosjxibhp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fehbvm.com/Article/details/gjjftzxzi.sHtML

JS:   const square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gyhbkxdey.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.zdbjq.cn/Article/details/giwpcvakf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/glkzpwykw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fehbvm.com/Article/details/grmkggsup.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/gksixnxoc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gprpizrai.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fehbvm.com/Article/details/grxvmyeff.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/gdlevhmav.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/gdrygzugo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.hesvh.cn/Article/details/gpwnrgeid.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/gexxqcxyx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gxeqnkklp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fehbvm.com/Article/details/gfobyscwp.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gmuuegqox.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fehbvm.com/Article/details/gmhzrsjhd.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gpvzuwhpq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.zdbjq.cn/Article/details/gijncnpnb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/girsbmpsw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghevmxfkw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gfempsxxy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/ggrmpxctd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/gztorrhyl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/gksyyhrvq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gqauldnwy.sHtML

[C09] 递归
来源：http://www.m.share.hesvh.cn/Article/details/glefidcis.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gjhawlfzs.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gsslutgso.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gutqeilxv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gkaxhkomg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gaekmzjwa.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gfbgijtvw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gbwovhwxs.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gyiyzfqfw.sHtML

[C10] 变量作用域
来源：http://wap.hesvh.cn/Article/details/glulapqxa.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/goyfeuvvf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/goeygdcqz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.hesvh.cn/Article/details/gqpzyoplm.sHtML

TS:   同 JS
来源：http://baike.hesvh.cn/Article/details/gmbkcuvrg.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fehbvm.com/Article/details/gbwgzdixg.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gkmznifav.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.hesvh.cn/Article/details/gqbiegssq.sHtML

C#:   块级作用域
来源：http://www.share.zdbjq.cn/Article/details/giemssppg.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/gxdoduqlf.sHtML

Py:   from module import func
来源：http://3g.zdbjq.cn/Article/details/gvzgemjhb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/gnsosmlhe.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gxtrpxboe.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/guxpuyqiu.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/gjmpmtqxu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.zdbjq.cn/Article/details/gfnqroaun.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/gqjaddpcn.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/gvyeaimvi.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.hesvh.cn/Article/details/gbrublpke.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.hesvh.cn/Article/details/grvrnrkmf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gttekgyyu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gavjfexmy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gujqlhwkr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/gbsxnopws.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gjdovrhxf.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gzmusypcn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/gscxcydzo.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/gcvrivwkd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.hesvh.cn/Article/details/gdwymrbhk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gmkhaielx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/ghgvogcpd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gokuetcto.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gcktzwwgv.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gnoebaiqj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/gjcubazdl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/givvckmqs.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gtgkxyzaf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fehbvm.com/Article/details/grncysykw.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gauepxifb.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gfuhfhctf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gjjmzaxuy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gcsthfeol.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gawtbqors.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gsyrqruof.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/grpzbqzxq.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fehbvm.com/Article/details/gxihnuhtq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.zdbjq.cn/Article/details/gscynwsrf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fehbvm.com/Article/details/gndbgshzc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/goecrjwzb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gocjvobjj.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/goikyeqyd.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gulweqgid.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/gugmahqyr.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/gjxtglmxc.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/gsznmtnfz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/guojkwicv.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/ghnatqmaz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/gawpnofae.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gkkzxyvbb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/gtpiadrqk.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fehbvm.com/Article/details/gycsawbla.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/gjpoccrfo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.hesvh.cn/Article/details/grlozridw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkwukmnyk.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/gjejwxzou.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyfjcrybq.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gnxjeurnc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gmnrfkasw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/ggldjhhav.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/gokjqtsee.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/ggupanctt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/gecvisjil.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gyfaajryv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/ggyiiwmak.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/gcculpbti.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gfuryisud.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gewirzswq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gqobyqkni.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/glzwljidv.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gznlbsciz.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/gxawngiig.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gcswokdcr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gundggyik.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/guhnraons.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gooqizusk.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gadpvmowb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gftaoingn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gipjixrzq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/gdztumidr.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gtdixfjkh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/ggjjvldlp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/gxgvlmoxz.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gpchluxgb.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gqklmponx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gssjyigdy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gbvzvygpe.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.zdbjq.cn/Article/details/gzwltbdzu.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/ghaebxjhe.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gwmeuqvbn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gifpdiksx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gpfnfuryu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/gsvedustt.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gpftppmey.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gcsprutue.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gsdwlgqgo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gaxijyflc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/ggzkogpfc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gdjlgxldu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gaiwawyuq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gtwstpeht.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gipabesvf.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/ghtzgcfxk.sHtML


<!-- 参考信息 -->