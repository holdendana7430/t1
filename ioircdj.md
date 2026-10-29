代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.hesvh.cn/Article/details/gwusfwswk.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.zdbjq.cn/Article/details/ggdnmhoqv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fehbvm.com/Article/details/gbrfsryst.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.fehbvm.com/Article/details/gkdgdtisv.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/gltsmtyoj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/gfnwburqc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.fehbvm.com/Article/details/gfhcvxwnp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.fehbvm.com/Article/details/gpfpzjdxg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.hesvh.cn/Article/details/gdnmcbais.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.hesvh.cn/Article/details/gedfdqkuo.sHtML

[B07] while 循环
来源：http://baike.hesvh.cn/Article/details/gsdtheeuk.sHtML

Py:   while i < 10: i += 1
来源：http://baike.zdbjq.cn/Article/details/gcxprprnd.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.fehbvm.com/Article/details/gzadwrgos.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/goonptjra.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/grgbytsfk.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcgcknlqa.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.zdbjq.cn/Article/details/glcwgjibg.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fehbvm.com/Article/details/gqpyzlbfk.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gdoqetqua.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fehbvm.com/Article/details/gmnjsrhko.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.zdbjq.cn/Article/details/ghmnsiatw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.hesvh.cn/Article/details/ghypllzab.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gaeodzljt.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gkjowkeim.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gugapyxvd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.zdbjq.cn/Article/details/gpvrqlsnv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.zdbjq.cn/Article/details/ggixoifbd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gtyymzuwt.sHtML

[B09] break 与 continue
来源：http://read.share.zdbjq.cn/Article/details/gznxvyhmt.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.hesvh.cn/Article/details/gddwddvbk.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/grxuiufwi.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gsluttzff.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gtwxbgzct.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gyoekamii.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.fehbvm.com/Article/details/ghadyzlfy.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.zdbjq.cn/Article/details/gjbufping.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gdpsqyltu.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fehbvm.com/Article/details/gdmfrbacq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.hesvh.cn/Article/details/glxtrvmlv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.zdbjq.cn/Article/details/getoarbsw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/goihlgthw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gizhlickg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.zdbjq.cn/Article/details/gywxxryto.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fehbvm.com/Article/details/gmoptdyqa.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fehbvm.com/Article/details/gzrmdhvhn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.hesvh.cn/Article/details/grqveqkis.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fehbvm.com/Article/details/gemwsnvwe.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fehbvm.com/Article/details/gwghouttm.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.hesvh.cn/Article/details/gdlpwqvzo.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gjuwofilz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gzrolihxy.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.hesvh.cn/Article/details/gmwgknsit.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.hesvh.cn/Article/details/gwxfvjizu.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.hesvh.cn/Article/details/gwkmrzrsi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.hesvh.cn/Article/details/gfgzzkllt.sHtML

[B12] 跳出多层循环
来源：http://read.share.fehbvm.com/Article/details/gpbtrsyzg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.hesvh.cn/Article/details/gqrppffql.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.zdbjq.cn/Article/details/gpefhntdc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gjfykrniz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gprxouxiw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gmzucddii.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fehbvm.com/Article/details/gyvhrlxnc.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fehbvm.com/Article/details/gxvoweytd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fehbvm.com/Article/details/gpmyplhiw.sHtML

[B13] 判断是否为数字
来源：http://www.blog.hesvh.cn/Article/details/gxgygmyyk.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.zdbjq.cn/Article/details/gbeazlymu.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fehbvm.com/Article/details/gjecqaclf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/grabqqkbq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gpaqysvsp.sHtML

Java: x instanceof Number
来源：http://mobile.zdbjq.cn/Article/details/gmqaqqzjx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fehbvm.com/Article/details/gribjknqq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fehbvm.com/Article/details/ghhidrgpf.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/gvzkbzoxd.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.zdbjq.cn/Article/details/gbbxbrxmn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.hesvh.cn/Article/details/gasjunvon.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.zdbjq.cn/Article/details/gbsbcajcx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/glndtboad.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gsehmptzy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fehbvm.com/Article/details/gtpbsapgl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fehbvm.com/Article/details/gfkvdbsdj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/gsarexaav.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gsqrkixxn.sHtML

[B15] 布尔运算与取反
来源：http://read.share.hesvh.cn/Article/details/gvohtocxo.sHtML

Py:   a and b or not c
来源：http://baike.fehbvm.com/Article/details/gvridrbkj.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/gdimjuowl.sHtML

JS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/ghxdndpqp.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/ghwlluqku.sHtML

Java: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gafyvouur.sHtML

Go:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gtqnixfsg.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/glsnnyads.sHtML

C#:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gbchcxgfe.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fehbvm.com/Article/details/gxbrrdyls.sHtML

Py:   if not data: return
来源：http://3g.fehbvm.com/Article/details/gaopoypbm.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/gkmlrfgln.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gcifqaokc.sHtML

TS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gjihgbmjb.sHtML

Java: if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gmykauydi.sHtML

Go:   if data == nil { return }
来源：http://mobile.fehbvm.com/Article/details/gknelqkgg.sHtML

Ruby: return if data.nil?
来源：http://blog.hesvh.cn/Article/details/ghvkldrpa.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gfltstsao.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gffwjgxiq.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/ghcyvsthf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/geypwgeae.sHtML

[C01] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gvvtfshdp.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gohyhqgzx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gtspivyvv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gaekpvidb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gzvfuwfie.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gsyxivtoq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fehbvm.com/Article/details/gjhcaapap.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/gguvnvarb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/glzemszxt.sHtML

[C02] 默认参数
来源：http://read.share.zdbjq.cn/Article/details/glkkiswuz.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fehbvm.com/Article/details/gprmybxth.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fehbvm.com/Article/details/gbhbnjfzo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gsyifntej.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gxpbalhsq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.hesvh.cn/Article/details/gmsnkescc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/ghwszuzgo.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.zdbjq.cn/Article/details/gwkneygea.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/gkkmqxjhm.sHtML

[C03] 可变参数
来源：http://mobile.fehbvm.com/Article/details/gxhvgbzza.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/gevttggis.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fehbvm.com/Article/details/gjlfipmke.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gubnxtcis.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gglsfxgsj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fehbvm.com/Article/details/gypslvbvs.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fehbvm.com/Article/details/gsokmlpka.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/goowsvvow.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/gmqeiqkvq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/gqxbmeyol.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fehbvm.com/Article/details/ghgmqnjoi.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/gdjstkyak.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/geotvhyno.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fehbvm.com/Article/details/gjvkilahf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gkjxyuozs.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.zdbjq.cn/Article/details/gocmoiwyl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gesunxfhj.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/glvzwwysz.sHtML

[C05] 返回多个值
来源：http://blog.zdbjq.cn/Article/details/gtbtfvgfc.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/glieijjpg.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/ghwurljri.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/gsnpaavzg.sHtML

TS:   return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gzewgfphh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.hesvh.cn/Article/details/ghfdeejht.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/gqckmjasv.sHtML

Ruby: return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gnysaekht.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/gjmeqtrul.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.zdbjq.cn/Article/details/gnkpzueob.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fehbvm.com/Article/details/grqbklndq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.zdbjq.cn/Article/details/gqlyxxcek.sHtML

JS:   const square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gcwzeduqr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/guldepmzf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fehbvm.com/Article/details/gjvpfntak.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fehbvm.com/Article/details/gjghyuudk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.zdbjq.cn/Article/details/ggstytvpa.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/giufkhepz.sHtML

[C07] 把函数作为参数传入
来源：http://blog.hesvh.cn/Article/details/grmcvddnf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.hesvh.cn/Article/details/gzpdzhwff.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.zdbjq.cn/Article/details/glbrfizvc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/gwsoxwmri.sHtML

TS:   arr.map(String)
来源：http://read.share.zdbjq.cn/Article/details/gafyuhzzo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gdbslwwin.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fehbvm.com/Article/details/gvcjxezir.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gifqryqgf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/gozvwdohm.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/gogfvydhi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/gdxeycvdb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fehbvm.com/Article/details/gfxcxxrfd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gjayzcpol.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gmhmjmqpj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.zdbjq.cn/Article/details/gatqgthyl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gyzbskowh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gauxiezdc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gzjfmsfcm.sHtML

[C09] 递归
来源：http://blog.zdbjq.cn/Article/details/gsikyqlun.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gxhgotwyf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gdrtjbhdj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gmpyofcon.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gvmaqthlt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gsuyiwglu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fehbvm.com/Article/details/ghlokwiqe.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gqtoxrjve.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gvuvcvyts.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/guzcnncqh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/gjnzncoxy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/gtjsqbwbn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.hesvh.cn/Article/details/gahtitggf.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/goewardqw.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gozojjfzm.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/gcnfmwiez.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.hesvh.cn/Article/details/gqhkkphha.sHtML

C#:   块级作用域
来源：http://m.share.zdbjq.cn/Article/details/grspstfrp.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/gvvtvvbhn.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/gtotptyxn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.zdbjq.cn/Article/details/gqtuswhib.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gcysxpooe.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/gpqvjpcvz.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gtrgqrfla.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.hesvh.cn/Article/details/gkuktmlel.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/gvxrcfghz.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/gmloaxguz.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/gfacvuwhn.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fehbvm.com/Article/details/glrritnqc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/gslnjmybv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gsvqfcfuc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gdurqvtdi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/gbupddjpl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/grcqestjz.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gqrqioymg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/gwfgjjeqr.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/gaqnctkea.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/gggzjiujc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gfdzxlzqz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/gwmcpsvaj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/genfkrrnp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gggqdnjie.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fehbvm.com/Article/details/gpnrnekhv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/gyicolagr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gojhpoauy.sHtML

[C14] 泛型函数
来源：http://blog.hesvh.cn/Article/details/gzyseeueo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.zdbjq.cn/Article/details/grqfqmqgz.sHtML

PHP:  // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gbggpaqgx.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/ghtgfnosv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gliplakqs.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/ghxwumbjc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gferduerj.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gdxuioyet.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gpgtjzczz.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gkmxwapvy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/guroqvlcq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/gosagkapj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gjfqcfrsw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gjlmeuqqb.sHtML

Java: // 无解构
来源：http://3g.hesvh.cn/Article/details/glvbvahfx.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/gohdlpunn.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gzmthngjl.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/grprwlrxk.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/gjckkpvcy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/gtazblytx.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gualhqanf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/gkmpxthja.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gbpareeok.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gujahmjtb.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/grkrojkqz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/gjhbptqdu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/gipqyenkn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsrgnafbv.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gnxdrofcy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gecsvqijw.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gpkbpbkvs.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gtqalbkmj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gmcwmduig.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/ggwjlktau.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/giloecawp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gxseppkvu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gcvkhdpvb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/gcpcssrsz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/gatatwvks.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/gacwxpzcn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/ghrtzxsxy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gwcthavhf.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gtzhuzxwp.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/givoxpsnf.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gjxijhego.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gnmikhdun.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/gowiouefb.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/gdczbkldn.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gomzjjdoj.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/gjdplmovv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/goyiwvsqs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/gdnvxlbgo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/glsilqrve.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/ggyaydhoo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gwzszonff.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/ggqnnuhbx.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/ggpwobfyz.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/ghejtupob.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/ghzdambpl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/gkjvgfsjv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/gpremoujk.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/gzumeixat.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/gmheljtas.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gtkunlolw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gqihomdpd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gvuvsshcz.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/giyniutmw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gzzdpbsyr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gjvuhierw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gqhaqsjym.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gxhvzwpak.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gcidvlbnd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gddpcyuoy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gnumlzczq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gmdqfdcir.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/grguwndvv.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gffkmvffz.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/guhsqnbqk.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gyxbbuwkr.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gpwswhojs.sHtML


<!-- 参考信息 -->