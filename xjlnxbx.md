代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.zdbjq.cn/Article/details/gqlpdrpzv.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.fehbvm.com/Article/details/gdxlgetwf.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.hesvh.cn/Article/details/goywphysk.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gifhauvap.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gkrpjixae.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.zdbjq.cn/Article/details/gwdfpbixi.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.hesvh.cn/Article/details/gjpzskliw.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.hesvh.cn/Article/details/gnezgmhiz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/goyzwlxcn.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.zdbjq.cn/Article/details/goitqbjus.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.hesvh.cn/Article/details/gqqzjwzec.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.hesvh.cn/Article/details/gfeuqlymx.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gqcxfnaau.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.hesvh.cn/Article/details/ggrtcfprh.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.zdbjq.cn/Article/details/gmcbcaswk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.fehbvm.com/Article/details/gfkoyasyo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/gjwyikpap.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/gxckyqwlg.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.fehbvm.com/Article/details/gyltdaafm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.zdbjq.cn/Article/details/ghenyzvmm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.fehbvm.com/Article/details/gvmpcobmf.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.zdbjq.cn/Article/details/gdkihaoly.sHtML

[B07] while 循环
来源：http://baike.hesvh.cn/Article/details/ghnfajzlf.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gujsqejhs.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gxjuhowrb.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gnqxakdhy.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gqlgcolqi.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gujmnunkn.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.hesvh.cn/Article/details/glvdqqluc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.zdbjq.cn/Article/details/guktdynct.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/guxilxonz.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.fehbvm.com/Article/details/gdijxpkfo.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.zdbjq.cn/Article/details/gjdqqsita.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.hesvh.cn/Article/details/ggtwwujnz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/godeprsru.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gygrogpqz.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gesnwfqgs.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.hesvh.cn/Article/details/gcgnkgclu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.hesvh.cn/Article/details/gtnvhimou.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gwqmttust.sHtML

[B09] break 与 continue
来源：http://blog.zdbjq.cn/Article/details/gsgvyvzpv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fehbvm.com/Article/details/goobbcvcm.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gubnwqfqv.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gosettycc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/ggklmlsvi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gpxbulfsb.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.zdbjq.cn/Article/details/ggrdgvtiu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.hesvh.cn/Article/details/gfoosuhxb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gxxmaqndm.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.hesvh.cn/Article/details/gmpudmham.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fehbvm.com/Article/details/gltickdcb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.zdbjq.cn/Article/details/gyipotnnx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/ghdzmapaf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.hesvh.cn/Article/details/gmqdqpjlm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fehbvm.com/Article/details/gtnqiohej.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.zdbjq.cn/Article/details/gduumklhv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.hesvh.cn/Article/details/gubfuuabk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.zdbjq.cn/Article/details/gmnqzochu.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fehbvm.com/Article/details/gzjbbsjkh.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.hesvh.cn/Article/details/gtvxlughc.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.hesvh.cn/Article/details/gzwdljemz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gokentgbq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/gplhqjprm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.zdbjq.cn/Article/details/gwqphydhr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.fehbvm.com/Article/details/gmtdmdabv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fehbvm.com/Article/details/gzguhtkmh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.zdbjq.cn/Article/details/gibpyghvs.sHtML

[B12] 跳出多层循环
来源：http://m.share.zdbjq.cn/Article/details/gmvwaczfo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/gnbotzybc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.hesvh.cn/Article/details/gkzfkpanf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gfhgrsxod.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gmftbzqxe.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gsyncmroj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.zdbjq.cn/Article/details/gflnhrvdg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fehbvm.com/Article/details/gqirzkfob.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/gousdxstm.sHtML

[B13] 判断是否为数字
来源：http://wap.hesvh.cn/Article/details/gtyggplsa.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/gxepmjpvo.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fehbvm.com/Article/details/givjmjzua.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/guihheans.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gxeqqfnga.sHtML

Java: x instanceof Number
来源：http://mobile.zdbjq.cn/Article/details/gnpnisecj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.hesvh.cn/Article/details/gdnqzigjc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.hesvh.cn/Article/details/glhkoatdj.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fehbvm.com/Article/details/gburnucan.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/ghwxkheie.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fehbvm.com/Article/details/gnioaqqcg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.zdbjq.cn/Article/details/gbqjeqovr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gowuwtlvn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gevjkalrb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gkegbewhe.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.zdbjq.cn/Article/details/gqevvquwo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gstwpfwpd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/glyiqkjlq.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/gfmrjsjuo.sHtML

Py:   a and b or not c
来源：http://mobile.hesvh.cn/Article/details/gzrnefdtg.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fehbvm.com/Article/details/gmdndszes.sHtML

JS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gmioxbgnv.sHtML

TS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gqrcrxkdg.sHtML

Java: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gwsmdwonr.sHtML

Go:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gntdnboao.sHtML

Ruby: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gguawztsq.sHtML

C#:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gjxjqnhzd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.hesvh.cn/Article/details/gqmaejfat.sHtML

Py:   if not data: return
来源：http://wap.hesvh.cn/Article/details/gtvvmgphz.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/gjwqdaoti.sHtML

JS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/ggowakkfx.sHtML

TS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/glvlkhjnt.sHtML

Java: if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gtkuhfvzg.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/gubdweike.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.zdbjq.cn/Article/details/gguffnjhv.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gvrpskgrq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwqjsrbtk.sHtML

C. 函数与作用域
来源：http://mobile.fehbvm.com/Article/details/gawteblur.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grrabxaxh.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gqzeefwfp.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gtszdcllv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gsmehtszd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gewyavvla.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gxkvbrkbb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gpqztzimw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/geangdeqr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.hesvh.cn/Article/details/gokpxiwnn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gtimurjge.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gmhccsvpf.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/gkxfhqsxm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.zdbjq.cn/Article/details/gqyhrlqwi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/glyavbnbe.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gvjyrzppu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.hesvh.cn/Article/details/gwimpjqug.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fehbvm.com/Article/details/gkbgyuvaj.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fehbvm.com/Article/details/gweamqsvz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/gjnqtbwud.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/ggyhvionp.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.hesvh.cn/Article/details/gbrpmwtsp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fehbvm.com/Article/details/gosuxjwco.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gcvwzbuti.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gdxhtxiqg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.hesvh.cn/Article/details/gwqcgndit.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/gjxdbsjzd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.zdbjq.cn/Article/details/gdscmqgom.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/geqcvkrvf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.zdbjq.cn/Article/details/gfpvpqenx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fehbvm.com/Article/details/gepqtcmjm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gcnpcsurh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gztafowsh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.hesvh.cn/Article/details/gpdxehnro.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/gzdzpkswi.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fehbvm.com/Article/details/gtsfztfcq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gafvqhqln.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gnokiqqdw.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/gbgnhpqxt.sHtML

Py:   return a, b
来源：http://baike.hesvh.cn/Article/details/grebpdunj.sHtML

PHP:  return [$a, $b];
来源：http://www.share.hesvh.cn/Article/details/giqrtqhrt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/ggliommrb.sHtML

TS:   return { a, b };
来源：http://blog.zdbjq.cn/Article/details/ggihkzimg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/gpuxpxrbh.sHtML

Go:   return a, b
来源：http://blog.fehbvm.com/Article/details/grpkkcybt.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gxazxkjlm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/gqeokxfzm.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fehbvm.com/Article/details/gpzhcdjck.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/gngnmnzqd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fehbvm.com/Article/details/gzncycadd.sHtML

JS:   const square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gdrjozjia.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/ggqpwumec.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/gkvqsqrdb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/gymfnaeku.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.hesvh.cn/Article/details/grztatwox.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gztxmiwxr.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fehbvm.com/Article/details/gmnfewlvh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/gceoruidd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gyoetoxdv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/gyuosrfzb.sHtML

TS:   arr.map(String)
来源：http://wap.hesvh.cn/Article/details/gcgihowdw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gmsretiuc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.hesvh.cn/Article/details/gasbxsdyf.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/glvoulakj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fehbvm.com/Article/details/gxnqngtso.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/gsyqlbwlc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/gldxiojbv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gagevswtz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gwoapeukd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gerxbzlar.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/gyhbdejtf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.zdbjq.cn/Article/details/giyxqswrs.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fehbvm.com/Article/details/gppczijvr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gveawsuhr.sHtML

[C09] 递归
来源：http://blog.zdbjq.cn/Article/details/ggunjgfpn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gwfovwrpu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gqmrydjax.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/glzngzbmd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/glrwqeggu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.zdbjq.cn/Article/details/ghddrcrug.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.hesvh.cn/Article/details/gajcrizqp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gjhoijcbr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/giskanvqn.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gjpzngfmc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.zdbjq.cn/Article/details/grbyxchor.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/gzzejjvrg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gmihwhjwq.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gtwroyoik.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/ghabxczxs.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gyynhrtvd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gcivdpkoz.sHtML

C#:   块级作用域
来源：http://read.share.hesvh.cn/Article/details/gczijkhyk.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/gsiavexnu.sHtML

Py:   from module import func
来源：http://baike.fehbvm.com/Article/details/gqraneplb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.zdbjq.cn/Article/details/gmmxcbjan.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gzyvaqfju.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gvatqwwvj.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/ggdziacyh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/gliijqxun.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/ggkcyzldm.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/gzxdmefsr.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gvlwbklpg.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fehbvm.com/Article/details/grnrlcyuo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.hesvh.cn/Article/details/gcovpgqnt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/ghxgmwwqw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gvybrfgbw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/glmspxlej.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gtnykkzje.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fehbvm.com/Article/details/gphhpcpzn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.zdbjq.cn/Article/details/gpltpwuui.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/gazmrzwxk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gyllfgkjr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gqtpcgojm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/gdknitfdo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gkxgttmsv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gwwxmmkrd.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gdklwulub.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/geibofovq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/gceaezxgc.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gyqxjsmkh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gbupfovth.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/ggsmrssus.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/guzjqlsrl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.zdbjq.cn/Article/details/gknjhyook.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/gvhebavxt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gzzequsnx.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/gbvbdskbg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gfmamvqxl.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.zdbjq.cn/Article/details/gsblogmqa.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/gwnycrpfd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/grxzmjpfy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gghsevfwl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcemkpnpr.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/grziiiqdq.sHtML

Go:   // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gxgkadwsh.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/gdpeffpfp.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gxnlmpfhj.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/ggbkppqvo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/ghmojiknq.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/glucjebjr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gakvgdpig.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gwgmznnay.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gzlgeurbt.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/gpzbsbjet.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.hesvh.cn/Article/details/gahupache.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/gpzidpewv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghmoyzqey.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/gbmebiyev.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfykcojtu.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gvjfykgsh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gdazzbrpg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gpvxdadoc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/ghbdtibgt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/gkdslhauv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/gzyyxoxno.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/gattnphzy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gnqwwotqi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.zdbjq.cn/Article/details/gyqshbeiv.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gnjtsrrux.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gosobaozu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/gurvxohmr.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gjafixqfb.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gqajzmbly.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/gpalrnyzb.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gitdlgwwk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.zdbjq.cn/Article/details/gayefznwx.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gcspzfbgn.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gmhjawnys.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gvajoveob.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/gkqenunrh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gmxoybyjh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gntktyjjk.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gdjczthkb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gwninpqif.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/gjbcdiugs.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gblbrgyjl.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/ghymggiga.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gzbugfomg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/gkijmmski.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gjavtrbeh.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gpzbbqcdk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/gfciagpav.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gwqauoqvs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gfuvsncep.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/geyrixvwa.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/gczjopkjl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/glafgzkzx.sHtML


<!-- 参考信息 -->