代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3jibrvhpn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3aeohxrmf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3fsqlipfa.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hbpdvbit.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ngxmzzdo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3twdbxzbh.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3rmfpnjrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qkczvjhr.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3clufurep.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3gymizarf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3zakhduls.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wbpcjoev.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3kbybwdnz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zodsfqfa.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3egpgqwcw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3ekrwxigq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jgargduw.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3fvydzacp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3didqscgv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3barkbxxi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3msiupjcb.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mfcbzyrq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3nvpwjdea.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3kdzuwotf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3nvkuhvos.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ltkzirtd.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3eqwvumqn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3gduhaqow.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bzbaxgas.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsuyzfbj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rkjvdinz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gkqdrtoz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3vandyhcs.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3biltetyn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3syrofsyb.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3gmcojfqv.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3plbaknub.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3chneoszv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3jtiiagtt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxonytxt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3qcukucum.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3xabbjucu.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3kzmkrmgz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3zsubwqmo.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3dypmrugc.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ycrmpukb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfilxdlb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3zcychhsf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vhnppptm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3mktwyqje.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3qggkvrhu.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3nhbrvfmn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3cdwicddi.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3mwltsrwk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3gmekcwtk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfswlest.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ceizxjaz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3hfedzleb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3nylcrzph.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3jerfidst.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3aijnufvg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3fmjjhpbw.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3ixdttheh.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3vadnyaxi.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnddzqtm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nobhkliy.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ponnbeek.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzyulrtf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3pttpmdhn.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3tttzsoln.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3afnuyfig.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3qhwfibvi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3jcmxeeun.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jfsiogmr.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mvrkbytt.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kbbnfmqc.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xgvzzmdl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3aehhsbng.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3kwtnfvyf.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vemorfzf.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ulfekrhr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3zxikqdwn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3iptzngrh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nppdktdp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ccqbgakl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikvjilay.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3capfpcjs.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3prsadrkq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ouxcdzev.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3wbsknpfc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3dkqtdqsk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahxauhgt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3aknjgpzq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3glmevfer.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ynbzvwko.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3lpwhsvav.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3yuxedeaf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3dollqvlq.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3njpoixcc.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3zzpxzdui.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aucgcncs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ggacbsew.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yrmgkbie.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3skntgdgi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3bsixkhsv.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hmlpvmst.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3grvrpepj.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ecfhvnlg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3gsneeztp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3tsrmoqmg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3foybcdtk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ibmghulm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hnruvpca.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3cyeyknwg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3xdnltbui.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3aowjulcy.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ktysqbjs.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3spvplzrl.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3friamryy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3rumuprxo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3pagfflja.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3mijfxstn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3sfextnjn.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3okildtuz.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3cuyftyex.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3qbcfawww.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3wihousrm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3fyenavux.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ajnuwbvx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tgvykxky.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gazewngt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3hsjxgaea.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bbanomyf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tokwlhyi.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3obotgknb.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3tynngpvk.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3azrsdfgx.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bfrfituc.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pespqxle.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vgeoiwid.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wtmyujxe.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hypgpjog.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gjadwtgx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3oyzpmigh.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3yovhqpaa.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3dqhbvuyx.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ugumulnk.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3cfimrjfj.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uucxzuva.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3nnzyewff.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3btfclssx.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3saarhbrr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yxnzneko.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ckaoddpv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bylxlzjs.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3efzscsuk.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wehsavpf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wqbqbsru.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3skfhxebc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3emvmqzma.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3usubeput.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3jkjfahku.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3fxcmhxje.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ufbrqowl.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3vgwptnnb.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3vvriqfgp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3gyujeypv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cafgotvo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vzfuplvh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3ocfvbrqu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3vfsglikv.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3fothqmez.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3rjcqblri.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ixdtihqr.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3pddqctrg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3czuoyfgc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3vflthlln.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3obuhhjpj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3bnkclwxu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3hcmkslxe.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3bqiadbpw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ftjpdeui.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3yesvbwrq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3jkkrpxlr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3dssnqvik.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3yepcfmcv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3sqmfvqrc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3jqdtaezy.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3riwbcdjv.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3zgeiieph.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hygpszxd.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ugrykxxu.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jvvgugnc.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3dzndhxcg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3wbibaicc.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3culjwilk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3aqkaxcka.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3mjvyhtnp.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3yhnwczir.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3udbjyrhj.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3kbectuso.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3shinwchg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3zjzxfsja.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bwqhtdfb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ddknlkrx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3wigzsuca.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3tfcygjxy.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3aqtopypb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ysgbjesr.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3vswgbxae.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3lxftkpta.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ofbgvhxv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3vegrubbm.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3cbodkjgi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3psqrmcsw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3pgefefkq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3qaabyyyy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3jlcrdryb.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3tuqgjhbo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3dvsmedmp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihaocnku.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hbthihde.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3fspntbbs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3efgouzsm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3dqjbzflr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3wbfwjidl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjckhmxz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3ckoztzrj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rynwpfjd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3klnzxbnf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3gduduqtc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3mjmdhfqz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3tcwgcqah.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3gywiflly.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3umkxgssf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hharimur.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jacrmmec.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3jbsxxjwh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3rwoxmhth.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nzwwjmzs.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3lxbawkfd.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pivbqpve.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wvapuxob.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3fhgnmnmi.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xrgupzos.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3gjnpcear.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3sfempfzg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3afsawmhk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3sdtwmklw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3azbliroz.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3csixdwpz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ukbembew.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3wmdmsnxr.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3djdmxish.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3xeajmbcu.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3hirusuei.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3ndslsffi.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3carbsbsu.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3wrxdueou.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3becnsdme.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3gembdezz.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3dqaopufy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kurionuo.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3nlrsxalf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3hycxjgzh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qwoqmapt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3yyhokpxc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3iknpmicm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3eljowrpw.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ganldclk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3wmbnkavr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3fnqcvblt.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3btbrhlfm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3dyjjlyxp.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kckaokvz.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3lzbabotd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3hkloqtjp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rwhspjzp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3sztvnsnv.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3trkeqqwq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3zemaxwsh.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3fqfyqoff.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3jowgmupk.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3szvyjmog.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3dwzrvlhy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xpzcowfx.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3fuugeuce.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3bpfjljwv.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3rjyfcpye.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3wmgslcnw.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3doevrlkk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3sbznsbgp.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ibmayqge.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3dhggrlpb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ecnnrfsv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3elfnxlid.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3zsbsfory.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3qjmzfnpq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lbeurljw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qtjhfhfu.html


<!-- 参考信息 -->