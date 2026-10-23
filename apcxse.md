代发 wailian999

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3wpmtveof.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3svybgzxn.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3rxavxtci.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3qwudolhi.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3agmmedqm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3mdodmbdj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3lyqwuuqa.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rpsumzqr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3mmfcvzja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xfjuuezd.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3ratfmome.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yfaszbqm.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3drmzyusa.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3aiplvgnk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3ozvjkwiw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kbrqpzjk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ajyghekn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hfpcqphr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ilqsmaaq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3gtmbbqel.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3sqpmgndn.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3yhpazelk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3hiqvpwjn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3krydwsdu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3yzvnfrac.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3getrujyz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xykdmpjo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3vzfltfls.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3zwrntbsj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3evlhcfmy.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ahedogge.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3lvfxfavb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nmuciuoo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ylmgihsj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lxhvcgqw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgawtegi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3xkigxfqm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3nriruvmp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3hlydsjfv.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3laewpiao.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3lfbjyzan.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3dntayqvn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3jufqpihi.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3vdxkckrc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lhppgasp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3kzlxvdnb.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3nuisejtv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fyycxfak.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ezisphiu.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3aoqwxpro.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3atfcipka.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wsnajlpt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ljgdzcge.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3mdcwpppt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3mbjzqvbo.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3cgbcphsc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3kjxqzrjj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3qrwqimol.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3lcbidspd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3daujmzuz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3jqhkcbwu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3hruiqhst.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3omszzoyy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3uafxhhcp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3qcfgbgqk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3bsuqvftj.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3bsdcygcb.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3vlpdpzle.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3mdubnatu.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vqyphayg.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lteusvus.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kwgxksgl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3ldtgmxah.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3nlsctrmf.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3auddqamz.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3coftjimj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3uuztjqbx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kigydale.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3banenajh.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3udzxhsdp.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hsasblhl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3jfcmstsg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3lvizjjjy.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gfjrjsuh.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3yawzxexv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3qmjxvdgg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwgrhpwc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3oyuieeot.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kozbhxbh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3irtbzrvt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3evvzybze.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3eryfyseq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mnblfrhk.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3qnlzfauz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3eebtqdbx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3spzjovcw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3vxczufhs.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3dqzveykl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3vqgruttv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3asomrrnc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3equosnsn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3smdjgsev.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3vlfglteh.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3fiiszuqb.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3yovhdais.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qcabvsjh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3fkvixwni.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3drfzumea.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3jvbhgsfv.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3mhdndwlj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3zpbhxsbk.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3mggavyip.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3wdzvdmxr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3rfjkiyyn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3txrbmnwr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bxkuekbu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3pcsnuyhz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3zywblqqu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3bkmpwxih.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3dgclogbh.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3rsymcgke.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3vvbaewzk.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3zuocmvdw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dtbeanpy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qxznimgd.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3vtbucwxq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3ulkorosy.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3qvbrrgis.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3rrnavytj.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3mshygapp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3llpomktt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3zohcjevc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fxsqpdhg.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3agsgrxqu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3slrtikrb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3npqreqrg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qjidkahe.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zufppmns.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3vntjuoji.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3tfdmxzac.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3jifmbsqh.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3htegatdg.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3otxfqlxf.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kwjoatak.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ksfldktp.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qylhdgji.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yxvovknw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3pgyhjcdy.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3qeluahcs.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldilwrml.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kcvgupek.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3utqymrjj.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hbnfchfu.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3plzeksym.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3rrsdsnbo.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ynznvfes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qvodxvej.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lrcdxdrr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zghprlgc.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ewkndepe.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3bhriuoly.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccbtqwdi.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hktyqpux.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uegjvaia.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hpkzbked.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3mpqlowds.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3dpziopsa.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vedetwzb.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3sffhlwql.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3vtwnrbpe.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aivmbety.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubfnmtqx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vhtjffgs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3dlwihblt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3belsufqs.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3cfqrbfoh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3daujmxhc.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3dcyczoyk.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3aaiuqrjg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3bfmrnjni.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hgnjslre.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3fiqjyudh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3rvvvdnas.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ybcpjstx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3dggeybnu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3rzynzcoz.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3narffwjs.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3zfurrhdx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3sbgdvofz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3atiizgbc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3tcmzfpol.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3blasbwdp.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3emklwxyp.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ajjbnaga.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3mwpphbjd.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3mhmdxcvq.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3lbrhbzzm.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3zdcbrawc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3kaksklgf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3lyydybxa.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3mrowcvbq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3omzssgaq.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pvnebgts.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3bcszyrjw.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3jtrlhzwl.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3lxlnnith.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3dwdrhfoj.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wevmhjzq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wwqasrmw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3luvqxfsn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3quexdmnq.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3rfywryua.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vsnwifyn.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3isfauhnc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3irzydnxr.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3qdqfznyg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3vlctjtkd.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3mirucxbt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vvmcqgvl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3dckcogco.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3dvmwzgbn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3mfjtuvvs.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3shmzucdh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3ipfxsfpy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3wayccfni.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ivqqicgp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mygdbsbg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3yydstuhj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3ebelxsat.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3nrtevvmp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bactrxqk.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3bbxbetza.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3llswoctf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3szqhozpl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3hqvezjrf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3pgfypnhz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3eacuurwt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3pppgxtqs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3qnblxbnz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3kmeopgyw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qrbesbzl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3vfmiankb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3tjuhsscq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3dqglosww.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3nrypmsgk.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gfoufikv.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uhonwcch.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3lgnuomyj.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3lysqkmrd.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3zmbzltzp.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ahwlezll.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3pctpwtkw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ikpzogvd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3gjlfteho.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3wsqqwhns.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3vjsqyeft.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3cgnxxwpo.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3viigbega.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3vfhyyasx.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3qjwmjobh.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3uwmcitgf.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3dplrewdr.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3snziudos.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3xtwiarlf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3mwvgwtiq.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3prjjmshv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3pmtgpxcn.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3bzsgsyde.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3gtrzhklw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzzkwcgs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3gsqrtxkb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgpykqqa.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ybpgxmhs.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3yjssiijg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3vsdqmjay.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3bswjuvid.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ezjkcull.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3pzxpbyts.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xjueuznb.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3uiwgpmcx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3jrreqjgf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3oartzfnv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3wyztlrre.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ohmcyuwh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3gbdgbnud.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3lkflgsxh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3qpzhchtl.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3eyexohfp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3linjebzt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3tkoptkqg.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ufjcilrl.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3fvviiqnt.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3oqebsnfu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3sdykecav.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3kxmfdkjz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3fteqeiol.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ktfauedn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3lfiqxazm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3oaaziuhr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3usfjuzfw.html


<!-- 参考信息 -->