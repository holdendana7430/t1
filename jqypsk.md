代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3qjxokvdr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3gmfcqdun.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3ktrnmmwb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3oiiiupbc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3vfmfbajk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ebpwljxi.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3lmjnaraj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rgtgyrgy.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3fdrgwoib.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3cffuqrcg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxlpqvpc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3oktegiab.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ompekgcc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xqfkcyfv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3hsyqmuyv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3mvahhwsb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vnqhzgjw.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3yvoqrpfm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3jxahprmw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcagcvpd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3tvdjxoje.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mducemtn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3feagpbfh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3vykruzth.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3xttegegc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3dbmogcrv.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3soaiumoi.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3zfvgclgo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3quavkjgt.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3sqdffxbs.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkjbjnvx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3weucajon.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3raamxpul.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3apgprcsc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3jyizhkzz.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3pdgirkwb.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3dkhhbowj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzcttwgv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3etcdqqwg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3yyisabba.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3csayonro.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3yytvkvzi.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3edbxfbrk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hcvyxakq.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lrfucvsd.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ylvdwzpv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnjuuuwv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3dkprtriz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3bryrbzbj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3rotjechx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3besghiha.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3hlxwzizk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3pozzixre.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ntswmuwg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ohqtfqcf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ztocwhbj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3layuzebg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3rsophyoc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3edbigbyb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3gxuemjdg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3zncnhkkf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3eojpbsia.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3clznhkih.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3cwxlnoyr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3odyeyqfd.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjbxtqhq.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ekjekbjz.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmifurnl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3ttcxddeq.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3qipeyyco.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhpsvbof.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3qpkvhaab.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3dhstjrlc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3oxolxubg.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yisbibcq.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mzregczk.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tedmuwgy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3xdgvgvxs.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3wsvrocqt.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tysdfbvu.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3tbspercf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3bdfbyauj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3urvnmwph.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzozannj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixwecizn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kzvpfjew.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3qqyspzrc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3exdtvtgx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zafvkkcj.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3vynqlrmt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3yrxuigje.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3koovexij.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3avulnrgq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3bonspoib.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3kpkhkwlw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ignjxahu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3bmrcomuo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3gvfgnuyk.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3boihrdyk.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3npmqbkjx.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3pqhlzuma.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ymlnluep.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3jjfhhzik.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3khzugynt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3vrlwizqb.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3lhnkdmtm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yopunsgs.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3pcawqosu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ppttdssy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ruubkjak.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wydyitls.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3tjkliyew.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bajzgrth.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3xsaznhha.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3fmjtzhwe.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3utepvyvi.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ykkrfslm.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3gqpyjyrx.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3cuovyzrl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tqzlhwrp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3thqvklee.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ljrcqmci.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3dvijzstf.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3klmfpavc.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3oheysqxg.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3tfydsdit.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3bzaenxfv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3gemjnkys.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3begowkta.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lktwrwyt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wfepjvnz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sppgtwjh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3bowwpytb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3shyzbygb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3cwasvqtn.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3iwpabtrw.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3bjncjhtp.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sopkjhbi.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ebntylwt.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dugulpzc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zlfzsilr.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jwkfaeik.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lphvbcdt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3wemplqml.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3cboswsth.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3isswigcd.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3pgifiwnq.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3mfcuvzok.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3emnjnbwd.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3hpkmdxpa.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3zelvhotu.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rxgemfjr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ejansdjk.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3qdztzjov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3skqowgeg.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3gabftlvg.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3pnhpsdth.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfiniqir.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zpdpmzqn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxzevfrg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aitydhha.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wrxqqtol.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3gznmczmy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pskixoas.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ujuxyfet.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3mxfxwtww.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkgxepiy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qoyvghyi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vyofcdry.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3soplgsye.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3yywrlden.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3gawxdxmj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3rwmcdyhe.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3fmclxxdu.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3isvudxrx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3dnlvfjyd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ogsgqyvu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3muhzsnkn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ohpkzkhy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3lsdxoayt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3vfrvoiek.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3yrzsklnq.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3qkxxraze.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3ifzlzhfb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3oaalojnl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kaxbtxtr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3jitzidfv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3hqzszcqq.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3jkkcnlhc.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jwsyprgl.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cpnhpnou.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3vokoncvy.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3dnjrywpk.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3kcyhrcbv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3tqlitcec.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3owfijewt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3feqnstst.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bpjwuddh.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qmrrpxmu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3nslgegyu.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3sqskqcnw.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3pekzhuad.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3cdqcdwhb.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3emnjgfsl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dlzupdkf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bkjopaam.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3fzhsidpr.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3jtsnfhai.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mzisnwyl.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3ngzunzck.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3guvtxuid.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hjssrxnu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3wwptmjof.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3wmmzdrho.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jblledry.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3dxwnjzbk.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3asnyqxof.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3wunbdhqr.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3cqorgbej.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3zkorbxxh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvzaqgpu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ssdhffsf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3okkoaykq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3zvcvwxil.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3nlvdwhlm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3koqzxhdr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qzpboomk.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3gagxbxjo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3sigyehkj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3sjawygoj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3kylbgyex.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3oofqyhii.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3drnijcjb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3zmhjnnrw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nsxgcuwp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3kutmoizm.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3xkrzbzpd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3znzruphc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3xbwferap.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fyeorzjx.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hkzpltbq.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xheuvluk.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bsypyukt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3oiqfmckx.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3djsiphib.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3sdarukeq.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3zceqqtvz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3nwgydztc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3obwmltsh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3dxwebjav.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3jvjjbggz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3gyxumioy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3rurbpqhc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ajhsuqma.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3iezlucku.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3rzdilqmu.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3eijhepne.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3apyannlm.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3pzbiodph.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3eosieawh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3fxocnrrp.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3rttrdofh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zakaeasx.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3vyevrsxx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3wpoqsznp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tgaysqke.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3vqwqdsiq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hxviucam.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cgmazedq.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3vnczehdt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3htgmvqjt.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3mlqyjvjq.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ytfdjiiq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3vvdiljos.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3twckkdwr.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xkygibzl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3amkutnkw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3tzbqmkkk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3bayqvqgq.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3yyylobfv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3xkvyieae.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3gfsoklfz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3bnpmfahl.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3mljnlgwu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3kkciuxcf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qrwvqxvw.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3dmqlmngc.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3cabzhhrp.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3gcbhfats.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3loccjact.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3phrxanyt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3grquzots.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3axfvsstt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3qphugyla.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3qiwivlfi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xatispkk.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3eqbnyjyb.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3klfqvugg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qgtvmope.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dlfurqvl.html


<!-- 参考信息 -->