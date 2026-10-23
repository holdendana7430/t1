代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3ztqoozcr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3tzsfjnws.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3zshibwuf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3oksqxbtg.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3grgfborb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pkankohb.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3kfhuzqnf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pbxmllog.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3vqcbebes.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3mkwuahws.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3prjtsivc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3euhpubpq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3npwitdcm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nzclanhz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3rsssddsk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3bghfhnjo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jpeoqhen.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3wqzqpqsi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3xhrsmzse.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3zxsmnqrh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3siyvgjdt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gajirrsx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lagrtfuq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3wgbulwen.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3jdfqcrda.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wuwmkpih.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3nnmisikd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3hutdmpnz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdoavgmy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3utiyjxok.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bklqozij.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gmbpcnau.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3wacxjapp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3utcwdjtm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3eaysyvud.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3nhkxspdv.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3soosetkg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3xuemigwg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3jwywmgyj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3myxefduc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3caumnsqz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3zoqqnqhj.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3ewfpgury.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3gkvxmsau.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3xmwtqtam.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3oebnaaay.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3yovsvawy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3iryuxjiu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3vcsahhzk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3stxbygix.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3csrlpdxv.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3crzentsq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hheendlf.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3zaijapof.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3znyctaoq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfvmrupo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3qrlmdopz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ruxavgue.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ckmwljtr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3aiymmtyc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3njerfzpr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3rqoqrwgl.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3mzcyydyg.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3afxshlvj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3mzumpvqk.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lxxqsqap.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xahuhtfn.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xxokkrok.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ghqckegl.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3bdjcnjvs.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3sebgovus.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3opxvmkxy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3pgsigwaj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mlpksolo.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lrslbyav.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pcrbgrmw.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fzouojbd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3dghmllbw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ldpclqhy.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tesgvftt.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3vaeywxzi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3jrfokotn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kixdyady.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3feprsbyg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmpcdsjg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ckgccagy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3yvrjnpet.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3zcpstmnc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmafagor.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3qzsosjfm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3ikxejxvz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjvqhwaw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3qkpgafvp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3rawhzrhg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3jdocunjn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3qwvhghbu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3rjcqwvrs.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3jzymjfvn.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3dlgraueh.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3jrxtcjmk.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kdlhktgg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oydhflua.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3pxaglbsg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3rxqpcwly.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3azsznhod.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3qjlyyfaa.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3lbhtmbac.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3pnbgrzwd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3ilxvrpch.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3yiahlmbq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fxbvwjjo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3shxawwsl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fqxfknfj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3vohruqku.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3yqkvntao.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3hatijxlp.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3cszqqyrc.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3legoupdi.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3bsfgxxud.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3sabclthx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ugwldemk.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3ijlijglg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3laigmuvv.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3kjycoioy.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3cahosfxl.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3owapmrcu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3yflyxcbx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3yyajjvqm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3uqganlhy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mxddddqt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pddxljfl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gajqpnsr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xczbrhpb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eqpwvqfs.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3ajrevkrw.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3bmrjlhln.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ugwssymk.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mnfloqah.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yohayyop.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gmrsuigo.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ussdaiun.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nmicriuq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3aqyztuev.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3spkwxlfk.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3rxlfpurr.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmlecols.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xhsshcmg.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mbqdmbng.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gegxutav.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3wxyzlopr.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3hnjiydzn.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zjwobzdz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3efamulux.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sndaulli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wlaugolv.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3xrgbciut.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3htpafupj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3otfonrha.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bzrldhpr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrxoeceh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jjyfvlnk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3vzqsfctw.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3rsqmledf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lddlttat.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3tpngjhvr.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3znkdzrue.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3yzscnxei.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3sxdurefj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbuawdpj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3yjekboeg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3vfwqteal.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ggimoftx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3oqiyaepw.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3bsppbnhn.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3iarnggdb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ahschtyx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3bznsjlwx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3gqmcfuwy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3sgcirudv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3lhwkxzhi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3cvjnsvaa.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3vleaesta.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3uxycrgoa.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3tjxdogzw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3eltnlllk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ksbmljuq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3jjwvwryj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3wnysnwov.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3sxmppkwi.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pogysvam.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wdszxocy.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3oabohpyt.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3pmhrmhuz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3fkppesze.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3pfjvsqsi.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3xedueevi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3jahdguvl.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3zlomapyo.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3adbckhfo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3rcmuqhmh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3yhpeodpn.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3vyzgnjkd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3jejmmlyc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3inehzxot.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3edhxrcge.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ljowcdyp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3nsjwgwhg.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3ocpjwsdj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hhdpoijh.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3skvcipvt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3cjczqtko.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3effiraad.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ectbvuqv.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3pszwaczf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3bevdwhci.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3tjhsijur.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3mpzabago.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3jdwtbbit.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ieburlim.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3fdarziva.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbsgyzul.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvwkjgjn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3zhzzomle.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3czefjsrz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3tmbrymdq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3jxjfwshc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gdqjuvxc.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3boucwbop.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3dxeytjgw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3xkblcyxt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3fsdvhfqe.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3wcyjqscx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3rbrvrixy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3lxpsibxc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mawrxnng.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3gnancxrq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hagvdcig.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3tcvxvihr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3vcdhnpbo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3lxpshthu.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3xuxlhyhn.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3yqwflrhi.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3dvauxcqi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3flteigfb.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qikjhmlm.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3hynsorrk.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ormtqtdx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3gtftderk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3pnnxqndg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3wjfduyga.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3rwgkxqli.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3iakzmwcd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ihcfkqnm.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3mvtqpzik.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3xstdfldh.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3oimaylib.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3opknwpxe.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jttvcbcm.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3dqlqjtei.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3sljdwpfm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3kmenkjmb.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3yzkzxsiu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3mukuaaia.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3itcwemsb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3jorfqzbp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3txfajzwj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3wvdbland.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmlqnznu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3niyswiak.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3vqmebioy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3aphlefml.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3akyvjydl.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3nhmvochb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3cuoipqsr.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nvrclgxr.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xsvmdjua.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyvdfrkp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3iaiistad.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3maexvzzc.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rolzqoqb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3melesluj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3dyszmsvc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3andlpjij.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3symdlkfm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wlkffxst.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3xaiwtszd.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ulbmlxsg.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ezwyvcvb.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3lbccnqeq.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3lojzmgxb.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3uvaqxvrk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3beesrtdh.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3zivjxicx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3wcjjlunf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3mehoimoo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ytvpjznm.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3zebqtugs.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3xszaecud.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3lyeuosbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jbkhalwl.html


<!-- 参考信息 -->