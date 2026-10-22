代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ywofphkx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kamrelmi.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2acgjzyvz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rsixmksg.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2lvymjysf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2kanblqte.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2guquttqy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2skfkqgam.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2vrocjdgh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2zmvhdmip.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2oghovnhy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2puajwycw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2dlhfzwvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wcubbxbr.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2wakqbjpa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2madfgztp.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2bznqpvve.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2korhkvdm.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkqjohgl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wnjgfrpw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zkkkukrr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2surgkmvj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2dyiufdew.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2dxkrdpec.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zifqhjga.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2cyfdzuhk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2wlvkcqgu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xifomfea.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2stdtugsu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hhjrifve.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ragcfisn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2odtevygk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2kuidjgpc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ridpofgw.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2hfdkdeyy.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2agljoyrq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iaecjydr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2skdawhut.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkjgniex.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xenezxgp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2lqwyfpjk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ismecnqc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2tijadter.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2cwsjhdqu.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2yaejmgxx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2rjnizxov.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ihmyzjhn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dmykjrsu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2arhrcaej.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2bkkdvtlh.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2mmdvtges.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2kezqklfb.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2pwelnscy.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2ugtytxzq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2qefbgpqi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2xamipnxc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2psrgwqvt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2lzmxzqin.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2lxybmwcy.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2cgllqwnw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xxmpfyrr.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2gwzphptz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2pzgljawj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2esrfgluj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2fdsukxyn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2pojvwjta.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2iblcgepc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2lgmimgcl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2rflssevb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2xxsoaecn.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2xmiootmt.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2rpmyvymi.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2pvldiwtf.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlvndcpm.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2reijnjjl.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gwvjkyim.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2rqvbsiyx.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2fvoipoqw.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eoscoesh.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2mbypkdvw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2gcnapcmz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wwwxjmwk.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wgzlotpf.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2eudrqupz.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vhqtddhh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zbmzjkeu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2yztiiudx.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zznrxoah.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2cdjwxluj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2etklbpum.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2enyznypg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ksdlgeip.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hymjuxmr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2sblsbstt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2qxttouel.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2kuroxgyg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ysubpbgy.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2hnpzxxsr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ldgtmvlg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2hvidkchg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2xeyvobmc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2tbsogmoh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2dwipkeqz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2qrlqzxvh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2wirykgkk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2orivvprq.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2zkcbzabu.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2njqlcchl.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ghbnionj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wwayntdi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vramvznd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jqmezyja.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2epzlmtxh.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2xmwtoglx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pmlppvlc.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2gdjfwqsw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2jjjhkjss.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2fqnqxhzm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hgxixmus.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2iyuxntmi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ykiuoohg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2oqhcqjto.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2tjqxkutl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2iukzjsyn.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2nyvcxkww.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2abazinux.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2mtbfqgfu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2pasgvpyj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2inowqlqk.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2vhgjmuyf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2omdeziuk.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2vjexwjjr.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ivbdgwky.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2ndsknygk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ghufrtcm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2wogctnum.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mxrundet.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nuddtzox.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2giqtkozy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pzirlekq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ddwatcsl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mhivwhuf.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2rtupxllw.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2wycjqqrc.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2pnsqamuk.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2oetcdwgx.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2upkronic.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fozgsuim.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dsqkzstk.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dvzivsuk.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2origmgzp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2jsjjxvxo.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2szsnaxwl.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2fywxvndc.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ucrqbpvc.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jizuaxop.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2zrjzeopv.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2nuxdtxjz.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2wcqabyqz.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2bsudtzpe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2irhcnyjs.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2lufbrmte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rhxskigv.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2fzxwqmld.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2cgntctse.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fddqkbuf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2azezlobu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2siiuoplx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mautjbrh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2plzxkjht.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2jurrfkmt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdtnqjvb.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ttgzsfrn.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ktlzpyzm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjrywapw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntbzwppa.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2roqlvoim.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ntcemgsu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2pclqoxqd.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2rpusvlvv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2azeeoffm.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2widlcufj.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2qrnkxjvo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2habmcean.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2htogezwi.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2xgksdsil.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2afvmnoot.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2bltkjnuz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2qnfehjwa.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2hxehoeer.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2jkiiarys.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2dmopvikp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2byfxdlhw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yvovduag.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2nkmargye.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2yqhqeuud.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2idpuibsi.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dwmecrch.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eroobdbv.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2veouhekw.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2abonscue.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2tovtdygh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2tbuoxjhw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2zskambhq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2dwgitsqh.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2tlyrxtje.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xsctedur.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2unurdtwq.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2rwgiicer.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2bfhffisl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2euhruhzq.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bjgsxcvk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wfvfbsee.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2ljckduxz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2oqrkrzuq.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2brdmkqpy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mvvtofpt.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2obnsieyt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2zaoixjhm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tmucjxem.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2hpizswyq.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2wblrfuhl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2eragmbax.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2drfchcgm.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2mgaupwlb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2wjoxdwjn.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2hlytlrve.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2aekaaimv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmujzclf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2leazdpku.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsgcdguj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2dnbxluyd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2jtoyjdkc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2ufecdete.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyhjexme.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2kefhfnxi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2anokgler.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2tpnodysl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2zjbkqyrp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ffondiez.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2vovkersh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2yaovvtaz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2snptagff.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2beyergfw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bykgixrh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2cyciyysr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2jqdzybyk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gyzgfbtv.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2fzmmdgqa.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dvxxhfgt.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wjelidyf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2tyurulhc.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wvvnwwot.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2dudlrrbn.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2bgdybzio.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2amzizhqt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2njuyxbtg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2umgrugyi.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2gurukagm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2zxxpgmov.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2kswtvhwl.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2cjrgpdwe.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2dugastrz.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2gvulusqf.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2oqgboxza.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ediglywl.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2fcouttdv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2txmteyxq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2jbomsqom.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2mrjxjsst.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2gaigjekn.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2xiyjclqj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2rkhcdyjo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2okibvfxc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2raksljry.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xsereicd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxydkqpi.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2kqwlchye.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2gdjhfbfp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ooqcfgvh.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2rmgthdul.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2qbnriote.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xqitzdgx.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2swilozrl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2asdruzzc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2cacsrosw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2qrosjwnc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wybyydxp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ujswkxgl.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2fcpdzcko.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2xwxammcq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2undhpwaw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2vmbqriqk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vfviwmpk.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zwhyfcrh.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2qizvfaxm.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2nryprdwk.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2uwhmhqdt.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2cfnmvaro.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2nihdhxal.html


<!-- 参考信息 -->