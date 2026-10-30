代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfaasjip.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxmtuxbe.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvqtvjqv.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptbhygzz.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfgjjsef.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqmhndvk.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grnhygkoe.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.fanxiaobao.xyz/Article/details/gkljbmypp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzsmnblk.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.fanxiaobao.xyz/Article/details/grpfjytka.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.fanxiaobao.xyz/Article/details/gfhnzoutw.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjrckzks.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givuseuuq.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.fanxiaobao.xyz/Article/details/gwamqzssk.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.fanxiaobao.xyz/Article/details/gqpohpevm.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gliarhyrr.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcekuqch.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fanxiaobao.xyz/Article/details/guaalagvv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzhyzhqq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.fanxiaobao.xyz/Article/details/gsapulxjx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fanxiaobao.xyz/Article/details/gfgjpwave.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtehfogkv.sHtML

[B07] while 循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gcldkloew.sHtML

Py:   while i < 10: i += 1
来源：http://3g.fanxiaobao.xyz/Article/details/gxgrtfdtg.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxeiuhduw.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlpuwybl.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfskrfsgl.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gippvsqda.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fanxiaobao.xyz/Article/details/gndkmmhxl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfjdmsgp.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfsqjswfq.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fanxiaobao.xyz/Article/details/grzwnkytn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fanxiaobao.xyz/Article/details/gcjggirec.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fanxiaobao.xyz/Article/details/gsrxogqsk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/gewizfmlg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyqessos.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/gnlywyjcs.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.fanxiaobao.xyz/Article/details/giozpwrnh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gssqufrax.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gworvwiar.sHtML

[B09] break 与 continue
来源：http://3g.fanxiaobao.xyz/Article/details/gijtpjtar.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.fanxiaobao.xyz/Article/details/geyxyvqap.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gefufqekd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmeyqwtko.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grwnnsyxk.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwtlbgqbp.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fanxiaobao.xyz/Article/details/gwwbqfezo.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfroveiq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/grvojewkx.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gnemzklns.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.fanxiaobao.xyz/Article/details/gybjptfhy.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwqhkwkw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fanxiaobao.xyz/Article/details/gmovxizeh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqixtaya.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fanxiaobao.xyz/Article/details/gidigwevn.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fanxiaobao.xyz/Article/details/gqliopaow.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fanxiaobao.xyz/Article/details/gbqdxbbeo.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gclugupmb.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggaseyama.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.fanxiaobao.xyz/Article/details/gmehuolsz.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyorxtsdb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhbcdpfc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gfvmfujrt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gkaecqrpe.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlpdziva.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fanxiaobao.xyz/Article/details/gopxpdviw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gotgtrzry.sHtML

[B12] 跳出多层循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gkinffjva.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidzzwjpo.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fanxiaobao.xyz/Article/details/gcomfxlng.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpamkapa.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gumnnzizq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvzovvwg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fanxiaobao.xyz/Article/details/gtidrpmvg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gssjwgpbf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fanxiaobao.xyz/Article/details/gkhcdbccu.sHtML

[B13] 判断是否为数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrxzznnw.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzbpqlus.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fanxiaobao.xyz/Article/details/glezgqtzr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fanxiaobao.xyz/Article/details/ggkcuynou.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvxmfeqb.sHtML

Java: x instanceof Number
来源：http://baike.fanxiaobao.xyz/Article/details/glbihxlds.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fanxiaobao.xyz/Article/details/gzluvddto.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fanxiaobao.xyz/Article/details/gsmutacpb.sHtML

C#:   x is int or double or decimal
来源：http://baike.fanxiaobao.xyz/Article/details/grwutybhj.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtgpcqfd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fanxiaobao.xyz/Article/details/gvukbmhty.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fanxiaobao.xyz/Article/details/grztctwnt.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gkbxdydyz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqgbcbyj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/glkgffuqn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpntmybvj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhpaepeh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvgwpyfn.sHtML

[B15] 布尔运算与取反
来源：http://3g.fanxiaobao.xyz/Article/details/gifmqcokw.sHtML

Py:   a and b or not c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmkjtach.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddgmwzfn.sHtML

JS:   a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/ggysjwnzz.sHtML

TS:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnaofhbs.sHtML

Java: a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gidohcjus.sHtML

Go:   a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gmodwinaw.sHtML

Ruby: a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gsovypdpl.sHtML

C#:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gtdrbjewc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzbyvvfa.sHtML

Py:   if not data: return
来源：http://3g.fanxiaobao.xyz/Article/details/gcpgzjgon.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fanxiaobao.xyz/Article/details/gexsbmpvo.sHtML

JS:   if (!data) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmgzurpy.sHtML

TS:   if (!data) return;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjndpnyiy.sHtML

Java: if (data == null) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjoudjhvr.sHtML

Go:   if data == nil { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcvahoec.sHtML

Ruby: return if data.nil?
来源：http://www.share.fanxiaobao.xyz/Article/details/grkfrlumz.sHtML

C#:   if (data == null) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gfkqlmxzw.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gbrbykpjh.sHtML

C. 函数与作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glynuylgk.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxapdtis.sHtML

[C01] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepgaaszt.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtinsigjb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/geszwjnjv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjopknrnn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfypljzfc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glounxlmg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpatmdcq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzfjwwvq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmbozgnr.sHtML

[C02] 默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gxdnhxlfx.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fanxiaobao.xyz/Article/details/ghapkuzzl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghdoocwnd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoyhpthh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gufjvtvpn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsxrfkxv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fanxiaobao.xyz/Article/details/gafnhlrnc.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwmcttpr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fanxiaobao.xyz/Article/details/gszbnjkak.sHtML

[C03] 可变参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gswspimbh.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzziriec.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxigxltom.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvdqubsf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrgagagj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gheexhvlp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyhjrjpx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fanxiaobao.xyz/Article/details/gaeoddslb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fanxiaobao.xyz/Article/details/gocmucwks.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gibssfgtt.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fanxiaobao.xyz/Article/details/gdpathrbw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbdcpuvy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gmfrtsvye.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fanxiaobao.xyz/Article/details/glgutacpq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fanxiaobao.xyz/Article/details/gjsmghslq.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvbvvbkp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjzjbyfu.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkfxugsm.sHtML

[C05] 返回多个值
来源：http://mobile.fanxiaobao.xyz/Article/details/gsriuzwsz.sHtML

Py:   return a, b
来源：http://wap.fanxiaobao.xyz/Article/details/ggwngnoua.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhlwbznu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fanxiaobao.xyz/Article/details/gairvpdyr.sHtML

TS:   return { a, b };
来源：http://wap.fanxiaobao.xyz/Article/details/gjyocqgzt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkioykru.sHtML

Go:   return a, b
来源：http://3g.fanxiaobao.xyz/Article/details/gokqbulbk.sHtML

Ruby: return a, b
来源：http://wap.fanxiaobao.xyz/Article/details/ggkbzkmxk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fanxiaobao.xyz/Article/details/gjgmpnszd.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gybdrfeji.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexbixpko.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fanxiaobao.xyz/Article/details/goqsunkbe.sHtML

JS:   const square = x => x * x;
来源：http://3g.fanxiaobao.xyz/Article/details/gkcbgdbvq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqcqwtfx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrycwhql.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fanxiaobao.xyz/Article/details/gbinuaafh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fanxiaobao.xyz/Article/details/gsgnhcudi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geknxzdvo.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fanxiaobao.xyz/Article/details/gdrgnwuoh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fanxiaobao.xyz/Article/details/gospyoyzz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsfjrqci.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fanxiaobao.xyz/Article/details/gptregilc.sHtML

TS:   arr.map(String)
来源：http://wap.fanxiaobao.xyz/Article/details/gfghfepoo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwgjgmzh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fanxiaobao.xyz/Article/details/glxsrhvhj.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fanxiaobao.xyz/Article/details/gowupmxgw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkltwfni.sHtML

[C08] 闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsxeptib.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaoigdeq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggoxmabdd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fanxiaobao.xyz/Article/details/grdtjuvgk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fanxiaobao.xyz/Article/details/gupdevyyn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fanxiaobao.xyz/Article/details/grhprdqte.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevlmurnc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gphngagoo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fanxiaobao.xyz/Article/details/gccfikcyo.sHtML

[C09] 递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyeilaiwt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnkimnvw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfxjxgwk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyyufabo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fanxiaobao.xyz/Article/details/gsqqdvvev.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxvpehao.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fanxiaobao.xyz/Article/details/gelstvnlz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gvkudfgrh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gseoxsrzi.sHtML

[C10] 变量作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpllypszz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrqrgabx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlufnfxc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gzpvwgnuj.sHtML

TS:   同 JS
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlyyslfm.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxbkzpsv.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeigzdbm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhlillyj.sHtML

C#:   块级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gofakymlv.sHtML

[C11] 模块导入与导出
来源：http://baike.fanxiaobao.xyz/Article/details/gidqxvmfa.sHtML

Py:   from module import func
来源：http://3g.fanxiaobao.xyz/Article/details/gaduprbde.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fanxiaobao.xyz/Article/details/gvvctegiz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdalwbhfh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fanxiaobao.xyz/Article/details/gexeqkkya.sHtML

Java: import java.util.List;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzwivrek.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fanxiaobao.xyz/Article/details/garhiglkc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geujdnzes.sHtML

C#:   using System.Text;
来源：http://blog.fanxiaobao.xyz/Article/details/gjhmgzwpp.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fanxiaobao.xyz/Article/details/gwfldhicc.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbhtshzl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fanxiaobao.xyz/Article/details/gdivdygsc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fanxiaobao.xyz/Article/details/gvvxiqbag.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrunnivp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyugqhaen.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fanxiaobao.xyz/Article/details/ghsddyrwn.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fanxiaobao.xyz/Article/details/gqmimwueh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gnlgrncwx.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fanxiaobao.xyz/Article/details/gzunbasrm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gwaigtycz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhlomspa.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fanxiaobao.xyz/Article/details/gffnfwtpd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbqgjslpg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuvfclly.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrmjhloy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljibfafd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givjxbsut.sHtML

[C14] 泛型函数
来源：http://3g.fanxiaobao.xyz/Article/details/gtvamzdle.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpscaegi.sHtML

PHP:  // 无泛型
来源：http://read.share.fanxiaobao.xyz/Article/details/grgeweale.sHtML

JS:   // 无泛型
来源：http://blog.fanxiaobao.xyz/Article/details/gwhzuefeo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsqmniqt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fanxiaobao.xyz/Article/details/gmsvjfyhi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbdyifoe.sHtML

Ruby: # 无泛型
来源：http://blog.fanxiaobao.xyz/Article/details/goabmtqik.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fanxiaobao.xyz/Article/details/gjayxewrb.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fanxiaobao.xyz/Article/details/gzcrnnxqk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fanxiaobao.xyz/Article/details/gnramufgd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fanxiaobao.xyz/Article/details/gluzkvdys.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgdsbmgy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gkxltkcnj.sHtML

Java: // 无解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsidvbiq.sHtML

Go:   // 无解构
来源：http://baike.fanxiaobao.xyz/Article/details/gboecllse.sHtML

Ruby: a, b = pair
来源：http://3g.fanxiaobao.xyz/Article/details/gewnupuhz.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjssfcgic.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzblsktu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fanxiaobao.xyz/Article/details/gowykprcm.sHtML

PHP:  // 无重载
来源：http://m.share.fanxiaobao.xyz/Article/details/gckcysual.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqtszrim.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvwayaep.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgaxyitm.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuuwswxx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fanxiaobao.xyz/Article/details/gfdxtxpvt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdufalryn.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxmblirt.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczuolysz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvntdzndm.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfzfpgdi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fanxiaobao.xyz/Article/details/gnfnlvsjl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgtefuhx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fanxiaobao.xyz/Article/details/gfbagsynr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fanxiaobao.xyz/Article/details/gtaboavwt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fanxiaobao.xyz/Article/details/gglrfscfs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fanxiaobao.xyz/Article/details/gbewvdgqk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknhckosc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspgjlwjj.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvmsmxvd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhuxsbqs.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fanxiaobao.xyz/Article/details/gxgpcppgo.sHtML

JS:   arr.push(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxeyybyem.sHtML

TS:   arr.push(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gepatcygh.sHtML

Java: list.add(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gqzewfdpe.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fanxiaobao.xyz/Article/details/gdkutvruv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fanxiaobao.xyz/Article/details/gyiawuqpy.sHtML

C#:   list.Add(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluylhtsb.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gyncunldm.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkdyyvsz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fanxiaobao.xyz/Article/details/galevgnoa.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fanxiaobao.xyz/Article/details/gzyakhyyg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gamgboios.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghereqblr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fanxiaobao.xyz/Article/details/gepkflgzx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fanxiaobao.xyz/Article/details/gkvtxamcs.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcssbtrzm.sHtML

[D04] 删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpsyctix.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjdrrfaz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsaihsil.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulqhyfko.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbftzntcf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfydrzdcf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fanxiaobao.xyz/Article/details/gydtfxjcj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqtkolov.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxrzlggk.sHtML

[D05] 访问与修改元素
来源：http://3g.fanxiaobao.xyz/Article/details/gaizbdpww.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fanxiaobao.xyz/Article/details/gbhyskcui.sHtML


<!-- 参考信息 -->