代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2cobpuweg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2akojqnrc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2swimtslp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2eavsjzxx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2cadudvxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sezbbtge.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2coogfqbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jefigskt.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2mhljrvcv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2nzlgbdba.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2aamfoggo.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2oeohiboz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hwqmofzb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qttjaeaj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2adfbqnap.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2hnpeaheu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2unmaxenj.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2oukdgzns.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2tefitoim.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2huhxkayb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qvisrcxc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dcvpxihu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2sjkrzlxq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2ylnncizp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2lwiifyfr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2mlpjkgsf.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2zhwdpmzb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2sxccznwm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdooggfi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2syryndfs.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjqjnfao.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cuyacscy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ehzmbhit.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2unlqznxm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2fvlgxkxt.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2iukrrbke.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2qunzvpnx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxiymbdo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2eymdauno.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xckshemc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2hreyrcvp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ghrqbdse.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2kucsmuoq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fwkgroyq.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2nnmbxyrd.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ugxfoxiz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrookxve.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2qswwfhbg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ggbwlxwj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2zefwspod.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2zxbsauwy.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2gexmavvp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dmsbyzup.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2rfmgtehg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ireminwq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifslouuu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2dxgnjwwx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2prfebdjw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2uslerewr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2osypazol.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2qgktjkji.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2rficjfka.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2iuwfzlnd.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ptghusji.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2akcbskhz.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2erebrbkh.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mcguraqv.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcevkuhj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2hxwosqbm.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2jtnxizpg.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2oottgbvn.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2calugllr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2jubaezkm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nrogyllh.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jbtjastd.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2alaswnhk.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2znnjxffy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2psbstyju.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ffzuyzfk.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2babfttrs.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2myjtizeo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2uysmmzwp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfjxbxvr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrnjqril.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmfylwzo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cstrsuff.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2xdvolfqf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2pcumnrjx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qtubhdvb.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2kahxfglr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2icytorqd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2shxrroba.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2kqshwqwo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2pidmiise.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2jlkxufcj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2uvkjkcii.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2suzwraox.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2qgyoyutn.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2npaoewbc.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2dlekvilc.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2rmyjfdbn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2digxgfbw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2exxtehwz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2urrhxalq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2mxxvfvqg.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ycckxder.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2vqvuyjhc.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2yfbasfrh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2hojhbyah.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2aepikxyv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2deuhwpjw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nwzwqzhl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nvsxyogh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2ofwpzjre.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2qntdtnzl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2oqsfhaas.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2puutckjq.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2vluerupz.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2jygrkepo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dbrbrssl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kjlaiftm.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2wecbcfot.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2wfvonldd.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2upthawut.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2osbpxuev.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ykuvdldl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2vkfnssgg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2peweipef.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ishcgcsl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xnzyikve.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2cgohkeiu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2khywpzwb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vtpmvprv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dpdokffi.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2nusyripg.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2qgorfewy.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2flrrzdpd.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mobmzlor.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2anysibnb.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mhahphoh.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2snlmjojd.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tftxahnq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nmddhodr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2iytzpmvz.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2jmwvflhq.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2mltrrbhp.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2znuaicmd.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2txvcnvwm.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ezseafmu.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2krllqfsv.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ayujrphl.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2zmablnlz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sfjuqrtn.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dgvnkijv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tymrdune.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2knnzkear.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zrczeloc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rkqdctuy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2viwpbejd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozpewhdi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwcavygz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2sdzcdqty.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2klnrvwpq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2quekydxx.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2jqzwnxah.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2banulibo.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbpfzkvg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2opazxcqg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dezatfqh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2cvggkwdw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2wdhimijy.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2ocjnhghi.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2zbidlgub.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2yyvmhwhe.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2ebmirino.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2qlhnavdm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2dbvucsio.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2pgocgsld.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2augexdsd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2oxtymjxk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2xvqchrqi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2xflqsulb.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2wkimqsgt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2dsgcqtri.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2jcgkzmjv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2skinqdri.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2rnaynisn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2dvjleczk.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ikfafkau.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dvbvqzat.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bzzvckzo.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ziumochz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2tfubwhse.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ogurqqnk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2idximkbe.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2gnzgqqdz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2msjjrzil.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nmthzyro.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2oghapuif.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2zmdlwndm.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2qwlpgodd.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2kvsfbuel.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2qmldpktu.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2yxcglgqb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rtzzmvdu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2sexzxnsj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2olozttjb.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2bwezvbkp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2towjzbdx.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2cliddogk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2gebbcjzw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2natkamxr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2ohkigmof.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2uqbqwgwv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lhjqtann.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2rpzgrhka.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2kelvjlti.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2alsdazts.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2qklatmgi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2vuymytca.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlqfxtij.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2phlkngkq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bftwktdq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2ottustzr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2cfilcpui.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2qfcwvylm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2soifmhrn.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2pihdmaol.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2wbljvpem.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2efmntwgz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2lgojpilq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2jpelcrcu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2jhgzgbop.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2pjklfzft.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2vapvtsuz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2tcditvhs.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jjmjqwol.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2kezaxsif.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2lynqqmif.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2lxpjmvbe.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ltsaksua.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cpnkugqe.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2nxknslcb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2wukyvjff.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2omufgqud.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2njjxdurh.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ruoudkmp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2wenmvaqf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2qsyihsqg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2kyouikji.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2djizxfvo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2fmswuizy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2pqzflcrs.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2rylwqnpo.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2psfffmgt.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2fgujfwec.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2wslzmcad.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2mfgrebhr.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2dnyagodg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ucgdmerp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2vjhcnizt.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2rcxagjll.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2eoxnwymw.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2eckweasc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2htbfldeb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ssbgkxsn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ucchoril.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbfcqpoo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2efjgtemu.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2jdvuttpr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2spjfmcoa.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2wscrndaa.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2jjbgonfc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2woeyilas.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mefkzfbq.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2boicpmuk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2rcyzhlji.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mjvbazgq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ovltvfrw.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2bpzescis.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2opewufwj.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2oscmcqju.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2unijbytz.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2fubnjvrt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2kluhdlyn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2gwlruhwe.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2wywsgcnd.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2oitptkzi.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2bvsurqgw.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2yqhjcdao.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2bghwsdcz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2bdybavjf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2wkwzzajm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2mutlvefo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2bezlnorz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tmpitwtp.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2swberfrr.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2aeruqefq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2bsxpiszm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wwydrbew.html


<!-- 参考信息 -->