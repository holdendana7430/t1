代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2ffrxnfzq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ehrmmoki.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2abgyyqhi.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wrtflymk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2zzrjooxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2foebxqpd.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2rucycxuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hftrzyun.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2zhkresha.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2qzuvvzpi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2tkzvquqh.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2lzegnqjb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tgnxwwmz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2cbrcktnv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2iahzxgij.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2xnzdqckj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yktynfxs.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2tjkalzwk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2mwkpdgmo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2bmdzwpqj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fyedkdnz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xqgprwcr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hbkwjcpm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ruspqdpp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2nswvgoor.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bgvuikez.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2fssoioev.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2znrvsnvj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2miubwihs.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgskzoab.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojsynbjs.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2csiefpoa.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2rzbzaiaw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2hbyzeoav.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2wwogkzla.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2cpjeijwc.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bwxwkcxh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2furropzy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2slekrtjh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ijileugz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2bmjajzum.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2yrujzhng.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2esohpjzq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qqmpxvfm.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2exwwqrhp.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2dckqlldz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2bdminrwg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gkjotfld.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2tghicycm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2imcufluv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2zrdemgib.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2publwwxp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2pbndloqz.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2jahksytu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2iggmumps.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eytegvro.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2kopsuyit.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2scehksoh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2lohyotij.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2qlgflgoj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2mcnffaox.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2qpedysru.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2tlwwkdpj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2obqgnjsv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxzvnjcf.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rbphuvtn.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlfzicnq.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qgwqllok.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2equujabq.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2asvnfjpo.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bofbvqyu.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2ddfoiclc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2dycldrmi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bzfgdmln.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2oxskcouj.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hoeabzmg.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dtkaqpsm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ehxvbstw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2aougaufq.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dgontzit.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2pegkevfh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2xhegdegi.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbddpgcw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcfwbzej.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqctqjoi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vorihier.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ciwdlbsj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2debeynha.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdpsolnf.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2uuwihzhe.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2oyqqnieb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2pkobwcfc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2aappixwi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2dlsrxrhl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2guahrsrr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2lfwmjuzs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2uaxfujdp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2asrmdkzm.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2auuvjtel.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2mfvssxiz.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2wmhtrvoo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2fzzjvscr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2fwkxzinx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pyjrnlvy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2vvhfsvuo.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2gokjgozg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2uqwpzjmd.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2qfasvdsw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ptosbgez.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ncjggxjp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2wvgwtewp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vllrddnf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ywxfnfap.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2egihjeoe.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2isnhshvb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2axwhtxlw.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2qesfzjko.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2bylxnfdx.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2yrjnumxb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2arrdbqxx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vjhbvlbu.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ppbhzlkz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2wntplhfi.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2otgjtsjt.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2hvyzzpsv.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2mjctrdwy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2afugbeln.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2cnmiurlt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zthldkpx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2johgggsn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nkbpkshy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2euaqjftv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qdahniyz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2cmngphsu.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2dofzuvwl.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ntgjutgf.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2tfirplow.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mrbvynfi.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kduixazy.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jjjlztcm.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jmskyqkc.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wvsauuiq.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ucytiiqg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2tkbwqmrb.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2stieuyuv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2cgnjrpaz.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2azapyefk.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zxyaovgb.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2dbzvcfqp.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ilmzzhmz.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2xtyggqig.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2pzfddlku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oyqoeyxc.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vuatdgit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hrvhaoiv.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2qzzgysns.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2rxiouquc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzjllalr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnaeyabq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fxitxedy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqimkksk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2mpfkhsyt.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2qsfgauxr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2guewhqju.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2uossylej.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2fmninymw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2jvyjavdg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bxrmeztp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2diqvdjde.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2vbyhnyoa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2akustbmh.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2lafsynsd.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2iltrgujl.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2avuzpabh.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2bqmznrxo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2uwieocbb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2fpqmkoez.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2kpjaegdn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tcyeevgv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2fgkeqhsn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2jvzkyyme.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2evittjex.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2tiepuzfz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2dpghazdk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ngsxgsaq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mrkfagdh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2gsvemric.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2mnoymmvn.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2osfywpfp.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mdfpzijh.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pqjwaqvi.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2fboukzqq.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2lwsiklxc.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2hsetgxjt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2fdfvzush.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2mfhuykmb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ybxppoil.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2soolbduy.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2widyctcv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2hmnpsocs.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2snubljsf.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2djmzmeci.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2eggdftkm.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pabqfgzx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lamgiluj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2avhvgmqs.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2jiryijil.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2mwusbgqa.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2eyyeydfm.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2bvaavljg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2txiaqjff.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2rzlzftoi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2xojgetty.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2yptdiddl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tlrdjntf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2ykycigkb.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2kfltbofo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2aszulncg.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2bdfiojmc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2vasghcjo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2crsoqozw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2esznjrhi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2tisnvoin.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2wmrgmgcz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2nmjjthna.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2evfbzifq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2iryahsmk.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2xgmoyhke.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2isdiinht.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2llwzplrh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vicbedig.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2scjjavkq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2owgfjhmx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2sairhirs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xwuxgazx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2njuaqxyh.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2rfjkyfrr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2pbiyquvh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2klaetkfh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2hctxcruh.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2oqtepmsm.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ghiiuyhw.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2aaunvwvg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2yqoavdpw.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bxojnrko.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2gjydpgvp.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2suuvorrb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2ledimlkc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2kgnotnuu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2twoidido.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2yqndddja.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2evgsjdmk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2lqtzaolc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2rygfojyc.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2bjsypcdw.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2cihfrilv.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2bttxiqtk.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2kjtzwlfw.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2fztsvdhp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2zinnyrma.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2gbopzwvi.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2fmwpxgbv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2dohocqcy.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2jibiobqn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2cwnipfek.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2yktkrxlg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2rhxrllgz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hamiasqk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tdwckyxa.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2btydlpiv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2fseoyune.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2iowzcnpy.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2auqrjyfv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ihqqmwxi.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mqlvnrme.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ktyavpxz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2gbjhzred.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2zyhfwvbo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2bkomakzq.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2folmtrjr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2pyhopgfv.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2xjeqiibi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2dsrpebux.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2uzssaitu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2txrhowrt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wjieutzh.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2akjnfqih.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ayntarfz.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2hdralpwp.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wojpecpn.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2fqfgnpnr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ljwehwrh.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2styonefo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2jaiztgjm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2prryugjh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kewlpveg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2curzawdy.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2knjbszqb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mdexejdd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dqjibxyk.html


<!-- 参考信息 -->