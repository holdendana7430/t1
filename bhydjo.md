代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2bdldxslo.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2akdcojlm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2esrgzqya.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2clxhwblx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2tjzjszso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oecrrklh.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2wdyodtkb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fbaeuyuj.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2koqlrgtb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2aekuvkvb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2pivqgibq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wnucmili.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bephufbr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2plhzlumy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2fabgpptl.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2sapsjzue.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dvqmcnsk.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2fwjqxzbj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2bmklvjsz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vttgzsai.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2syeadmqr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gpbtpkia.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2yfphadrp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2hryxbqrk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2srvzuhov.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2glyubkgp.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2qmutmbqp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2eenaonnn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkldfbvu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2etgswbvu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2svkfekug.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvlkkpzd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2jqfulfqf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2fsxwczqc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2phbkpcej.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2rhimmukr.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2zgqozhcy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2uggfsujy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pjnbbpir.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wfgxkkxs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2glgcuism.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2tvcczyxs.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2haqsogev.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vzxajnxu.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2eervnbpb.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2sbsgfetq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ffzuukgk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vxealjnb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vqqrefxu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2qnoxzktu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2ajschkce.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2lnusjdlq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2qdjutczw.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2rhhegcys.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2qjokzpyp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzrdenzs.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2mjlquwjl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ebqwskdu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2pqjyercj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2uxathglm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2nsyfoxhb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2bcxmpksl.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2mmtlqupp.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2cvszxlvj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2kxzyuktf.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2appzvtxc.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcosynkv.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rthdjwiz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2xvcrtnpf.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2wemwegct.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtkkoqtx.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2xorbfxmv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2nddgcoqg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jeneckzq.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xghqgntb.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kbhigvki.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hkjbwcvd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2omcsgftr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2qklkusto.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pywtlqft.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2ljjukzwr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2exwhdpal.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bgngtzyf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dqtubavt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2drzjdopw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qwwzfgpp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2gfrjuiki.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ilhpbqfq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2farnbkan.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2coapletp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ydjwkvqg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2tkttvjvk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2nzfaqxor.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2jrrrzfoz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2bkzokehc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2bywswxlk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2uijgargu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2onywyyhp.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2grlrdlot.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2zqowirou.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2uzmcvdgw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2newrlerc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2tastjsde.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rsvvxclr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ijfiisxe.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2xvqxpzyo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2twfpywol.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ulzbzddh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2uddaowjc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2jnbyrtjp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hlufiefx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bqoqclzi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2osgsooya.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2dobxpnjs.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2bazufpmv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2iymlmelc.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2wmdshkxr.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2dpicwabn.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2hljwjdcd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2dcjzsnjk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2alnwewuz.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2hjxyllpn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2xcsbjnib.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2okyttgcg.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2vceimted.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2rnprcfqf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2tpycvmzc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2rtliolzf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vnhgouls.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wufezcui.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2alppzmaq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2lsjtzgxb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cqabjpyp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ojrhburv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2mdgnnpnw.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2tinkzjfx.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2xeropziy.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nhhyxbfq.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2utdomulf.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2winafnzb.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2urypwnce.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uvnhvdge.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xtbsolov.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ofujtkfn.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2wojhddlh.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2pipzsvoj.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2jqoydrsl.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jqtldegw.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2fbohvuxj.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2rdpnyrvx.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2qlxdmjwt.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zqzwazwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2arfuhxen.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2dlbnuttu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cifcriph.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2pcgzviwt.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2baevyzst.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2uxcrkvpt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcvsuxbc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pikiakna.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ccolpbsl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ouxaatzg.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2lemjbdoo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtysqlhs.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2yugymvjb.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2xfhsuuqe.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2wewbllek.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppdgehhq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2eekwrbwn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2inykpnds.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2pigckker.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2zfrmwlzj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2skfkjmzr.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2ithcapfb.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2yagwxpuh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2ylpiurww.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zqknewvg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2fyumfyhw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2bqqeruqt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2esnnlqfy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2xbkfztmb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2nbnvfizl.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2knmjperi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2dncgwbwa.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2tajvfriq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2zdwbnxkv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2gcttcedn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2stnloviw.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2qyzfjewx.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ashyioak.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kpdfesii.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2obwjlijr.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2hitmtmdi.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2nwakvyjd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2epwlmpll.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2mouzftjf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2rltjprbn.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2zotlrjys.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ekvxchig.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2xitwxdbg.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2yydtgsou.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2aegpjrtz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2yguabhfk.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2sowmfzqj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2swdvemeu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2nylrrrma.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2pfjmyucu.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2kxdtrcdn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2otxrhbgy.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2hqkyakum.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2fdjrqxpx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iepcoryy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2qrixtsvb.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ahggryiu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gityybsr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2feloimmh.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2ybvcfqvc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2zmnfziko.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2rmnqycqp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2xsryunql.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2diilvotf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jrxofgio.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2imsvqblg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2izrmuuuq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2smhscwny.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2pfjopuks.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibskkdzn.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2byjmqsqq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sxcyagjt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2dmypgziw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2awpieavb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2morymvco.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2dfvtquaj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2pyvpmlna.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pmlcktum.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jlarflav.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wkewprzf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2wcnjdymj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2dmjmbvdp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ptyzabwn.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2imfynlmi.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2nwcspqyy.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wlphzxfo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2rtmoniab.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mytdimhh.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2qxwyiejr.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2uzzywhtq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2oaeybpra.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2icqynmgq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2rvqoewuu.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2masprlfm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2oxyjwzjb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2jqjgsvze.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2yycoqykx.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2hwgpuotk.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2mzzchkqn.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2gfzlogys.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ruopypki.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2auwwskcn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2mtlyqaft.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2dcllcztz.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2xxtrigeq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2luebrtla.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ashwyxki.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dhxqrmzz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yifpzota.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2hnwwnbhm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2triecakm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2brbrgkdk.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2uhqcywvh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2gujshfre.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2pvvsfpoc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2mxcnnoyx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ebagwwed.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wzdflnyt.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kiuxfhns.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdhiumyl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2wbzshtgs.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2gpboptyc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2woxjffyv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2wtcsqizv.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2tnvogmnb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ijhiddil.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2guuqnvvd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2rrzdmspz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kbnzxiaz.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2phfxtoko.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2mionslav.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ybntyyfk.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ippireff.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2mjkjtswe.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2clvapizt.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2hllwbfkj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2taqhaevl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2dbcxibhc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2biayqkfl.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2whrjhyoa.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2wywrygyx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2plssdbgy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jylxodnz.html


<!-- 参考信息 -->