代发 wailian999

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2yqukvdde.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ovfppmkq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2taucpefz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qgdopdoj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2acllzvor.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2koulnpnc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2mloeawlk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2ijianjzl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2cspwbazi.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2ldzowtzn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2xvgkazep.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2ydnyugsg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jkzsdpep.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tjxxwehk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wigcdlag.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2mmysbcnx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2lvnrzmgc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2aplyesvi.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2smmwwmnc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2cuuzpswl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2brexffcx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xttwficu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kkiuxnky.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kajtedax.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2qtpahwue.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2wlovyjsp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2xaedoqng.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2yayfmotz.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2fgenxrgo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2gnynddom.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2uvdhvrvu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jlrraacy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2nrtkched.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2rotmkhcm.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2fhwzejac.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2fzxipjun.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ysvwzvfw.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2pnairuee.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojkvdwkz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2carmmvju.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2pzknnucu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2zwffexyn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2pqsbznpp.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2rwbbvzsd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2vlsqrmcg.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2tmqbtllw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2oggixdqm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2rnpxcsbn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2qnnpcqqi.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2hggdwmhx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ydyidjii.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2ywnifwnv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2hquriobh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2dlnkgpwd.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2xvcinkid.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2mlvjzqxx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2uzupbtkd.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ddjtofdv.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2smvigodi.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fmrqatzx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2gzerpvci.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2mtqeavbt.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozcaaicl.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2uojfzyjb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2ecwafvec.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pwzxjduw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cosqzlxg.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ssngdfbq.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ipudbhws.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2qfjubvkq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2kkuikjfg.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dhqkvhio.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2keayngpb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2vzvuvutv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dpfoxegb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2eksyayxe.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nydxzcix.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ssumevzp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2rspiacuq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2bblbpdfg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2houbitmw.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2fpvglpfj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2psvkphpa.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2jxopjqmz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2yfnvdxgw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2hhiheklk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2kypyktvg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2bxtkjwim.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2kufssypo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2lsfzalpu.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2jolvygnr.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2zozvkxcg.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ewqukunc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2sdokjald.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2niyzwdtr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mqbawong.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2iblljltx.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2rqhkwbio.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lmxrwajf.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2xaoharuw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2nsmroztx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ugoaujfg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2pwxduioq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gyuukyhr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hrxujfmv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2tglhddag.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ikuqzjva.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2yeittwyt.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2lxhcwfeg.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2zhemrlto.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2xadkvyyp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ljnlluhf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2vnigcowb.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2vlslctus.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2rvgagkxu.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2rxoeavhw.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2tdfawena.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2igqqiyql.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2mtpfofnc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2vwrmkvtp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sboagojj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uvucxgdt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uhwcmwlw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2boibxywy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jswkxotw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xrczkrwk.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2cfkwfkaa.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2vqqdcsdf.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2boaypneu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qrwbgbne.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jxfhqnjh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2absxeixe.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cjovnotg.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2alhcbqff.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ycwxpsgu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2drnfijwt.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2aeqjpqcb.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2iuuhpxnj.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xnycptnc.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ubxcugpa.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2cxppdbnq.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ltfikwkr.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2rkpbbmhg.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2jhburksm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ueepfbbt.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2amfwmxyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yupwjotf.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2yljedmmh.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2djvymhur.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ciiidkqz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2czuxpkon.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zisstpwg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zpayhdcg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2swyawnbv.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2jrwujtdu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2czdipkbn.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2voxjzvzz.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2nkgeihbd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtljzgjv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylbsujrh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2oanftefl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2emmpqxxf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2pjokeohp.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2nowxfqww.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2drjtaxbn.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2xajovywx.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2scoyhzrw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2smelbtrk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ipojykot.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2kbiytsoe.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sxvlfvxg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2gplpsbmc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2dqjtyiew.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2njqccfuz.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2paegftvd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ewzmvwed.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2odhkkwfg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mlcnsdcj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2fctqusqq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2zdsxxvgz.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2qhxfzepr.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dosfmoyi.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tgqbdhpe.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2wxipmivt.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2tlswkwmw.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2qtpceffx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ipkubntc.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2vrzcwmrc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2dzkpbvfy.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wjypzgbo.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wotqoemo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2kuyryswu.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2yndfbwuk.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2xjydfkjw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2qhfxyemm.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bwcrdbdv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zcpyfkht.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2ovdixtlp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2vylliyct.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2opybcfkt.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ukpjgygi.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2urvnemsu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2rwnejrui.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sdmgdigv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2dushrgfk.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2uoqauxfb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2tmhskqly.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2wjqyhqxk.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2msivbvnj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2twstptyp.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2cepaqcsf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2gbjnrlof.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2gubfwopd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bghsmuep.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rfdeomho.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2sxuupxio.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2emzwlpyk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2svyvzotu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dcjzmjuu.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2gpaiapkh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ntaksexv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2chdqgezz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2bqzjhrkd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2dpqylctn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2popqpjlo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2yaceekek.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2mxfkmvpn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2dgnvlohn.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2ptiuqncs.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2dfqwdgqz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ktdbpsxc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2uwhxvisk.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2dyngsxum.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2khnziqyr.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ezhgcpzc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2pvabdrcp.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2knqwckbg.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2nwxntmog.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2hsjthjqx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2fuvfwtmv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2kcfgodfa.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2jlkmpjvz.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2enolituk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2hvdsxiws.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2wmnyrogq.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2pbhezewh.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2dunvfqtq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2pvezlitb.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2apemqbsv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2djxaszdq.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2qwxynstc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2fsbqwagg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2nfdbkrqa.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2risnxjid.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2guwaiqxu.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ntlfmtld.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2rcicbjyj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufgdvkya.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2lvpdoewl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xjzyknsx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zbmwawim.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2fizugbzi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2bpfnznkv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2hxlrpidt.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2bngrydbx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2slvqladm.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gjkzuymd.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2cztpnldu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2hcpzfopk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2slhizpth.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2qilhhflc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qaskmjeb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2vzovxuwy.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2tfcgwolj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2okmcjurm.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2cnwykdac.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qxssufhx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wfjczwfz.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2mcfxvtnn.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2qhhfvhsc.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2isduqxfl.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2zafvdafz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2baegvmhf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2jbflcwqs.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2fdsafvsd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2vsklowgk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2pmiifpeh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2iumiiuqi.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2srsjvhop.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2eqzkgyvx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ngornoaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pgeywdfz.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2golifctb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jnfuwyvz.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hgtkoksn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2frswokwo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2bzwxzrwn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ytmqbgac.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2wwsfzxmw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2qfbxmldu.html


<!-- 参考信息 -->