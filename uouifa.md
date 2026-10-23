代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3snovzndu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3xvolnsyj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3fweononx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dbeyagyh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ewdbgjwi.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3ionirrcm.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3bqzpivvt.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3jwbyxzbi.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3kkehxkpu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3zkipndlj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3xuiqqucx.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3bprgbqtn.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3ewqejnsl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3pemncxfk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3jjhdindv.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wvqmzvpb.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3yddqmnxd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ntoshaay.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3zbohhcbn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3cvnvcdfw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bvwckyir.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dkeicilq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3hbdjcshj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3spqqaaxr.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3pfoabuyv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3nottuehd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3pgpmyxkh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3aasxvwjx.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3ndoihsol.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ngsozegi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3aofgpkig.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3phvlcqco.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3aeovwbzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3olosjgkl.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3yrvuwmwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3himvohmk.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3mjhervwy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ulcjceuy.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3obgfzfrz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ziuuzuhd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3fzrixhwl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lzrqzquq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3tqlzwngn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3pcnsmcll.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3tykfwkxk.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3alfsghmh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3oxveypyx.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3cquyafue.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ewwpcsrv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zffujhvk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zondptwz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3pcohsfyq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3mnnuyoch.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3yroibaxd.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3wewqbaqg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3hlwpkvfl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vqcvjkul.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgweefoq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3icdbnmbn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufsynaeu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3jsvjvfph.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3ukhkomxa.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3cviahowi.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ihtwofhq.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zbhxmoqz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmqnecra.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ymnmcutl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3njgrwbqb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3oalkugjv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3sggwwnhx.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3nareqfti.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3knugqxjh.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rwpzrmvg.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3usdklias.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjrlxolb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3sqcrqtwr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3moeqxkyn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3qpnqhozt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3ttmolhyk.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3ogqqlilq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3nidhrmcg.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3wqfxwhux.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3incdbrxz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3wpqitsmf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3yijhlerk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ozaxltiv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3zcwpejzj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ftkrlkdy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3fyvnjhlc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3boremouz.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3ozcdovbp.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3gevkpsom.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3eslpplmg.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjmzfgcl.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3guhgnfyy.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnwudwut.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3jbscuunu.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3jkhpynme.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kugmnubw.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ngypfedt.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3fgygsaql.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3njgtnpyu.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3krbfufan.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ihqvohms.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tcoeoazh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ezhbllie.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3kizpvngk.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3cdseiydu.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3xtkzejwv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3mrijlggr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ituhgeog.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yvfhgben.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxlsnmlr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lnxslmkp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3rnenjfsh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3cqcnozht.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3pidmdlvu.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3wjjdshjt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3hgkblibm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3wehakizz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3wehvalvw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3yexfqipo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3jowfbdhz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3nikpksga.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3zivejzom.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3mruvtkve.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3ztbqiktt.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3ibsuubob.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3rmqwegnx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3trfztznf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hisglona.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3iqwllkbh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3slcjvkrj.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3edohvjmq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3jpeuzofd.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ujywmlbv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3bfqumgjl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3qezpglia.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3icpoybla.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kwdrlxxt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vzpfveyt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3vzfrssud.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3rixpadnd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3nswjicjf.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3cocvxvzd.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3tdasgvqr.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3qumosukg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3kcvvrqfq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cauxjeug.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3noxnavwh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3zdvewjwi.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3jzlwosmv.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3jtzgwemh.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3zhoxdxhc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ivzqfqem.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3yquoyunf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3huucctsk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lvvhxbkn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qlbemdny.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ckahsmrr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wyktrktu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qnibjiux.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3pmgfjbuv.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3wllzdmvf.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3aqlrlbrp.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ehrinoos.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hflvbeyu.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3etkoxlph.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pusuhtkg.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yaazigrz.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3peezxxpz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3euydryhw.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3fzpzwyvs.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3pyxydcdl.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hweuryxa.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dhajbrwu.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3yviwycdi.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3mdztifjh.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3idsienby.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3cjqhvjob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iuxdtsdr.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lmoihkvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nvygidiu.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3gpqnwmrp.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3jkjvlwwj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3janflcsy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3buihlltf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zjpgtcgc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3myyarbtc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3rnffywcv.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3hpaudugl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rujyqgsd.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3pwuofxyn.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3gtihktvo.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qosffitn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aobnyxsi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3khlmzrjf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3bipfwbmq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3guzmmusf.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3kyxptulu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3mojkvqoy.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3iklydobe.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3laixklkt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3lmkegcgo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gqieqyqe.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3kfehgfoj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3qadavhpn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3nnrcdhai.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3wdmpkjxo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3dzrivffb.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3qpzfoete.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3loegucqi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3evnmdhmw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3cjlbfjfz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3jjlexhen.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3tezeoosy.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3udvvlarj.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3eenkgnee.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mjwqysro.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3gayxujdv.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3helngqwj.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3qjrlwaoj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3tbbzukzm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3anzusswn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3fhbnejlw.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3rxndlexs.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3agaofmhn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3vgjeevdy.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3lljxogek.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3itnnpjyt.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3upyvgnix.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3venvebjt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3yxuognkt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3abwymxxa.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ixeqphaq.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3kznhwfcz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bzejxrme.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3sqrbkler.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3rupctobg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ypvfdzua.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3edsnzuen.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3auymdtrm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3reuglcbn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3jnvyccyi.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3vkjwypug.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3kogosiej.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3wuxzcree.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3jouxixjb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3hjdwskok.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3owzuoyee.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3zgbxkvxq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3jhmuqevk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3nknnnxmq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3mcmwxdvf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzwgxvco.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3lhhidfes.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3pgctabco.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3cesvbtkb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3syrduxqm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3kbpuavaa.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3fxynquhg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3tpcyjzbn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3desmuxcb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3orwnxbdm.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xfwxmncm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3icrbunmb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3copxtmdb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tslkarkk.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3axajjvav.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mjjzyapn.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fraeltgr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3uhdgtoci.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ocwkskbu.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3vhqmkhwm.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3okqseeon.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3lcwqnjvg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3lqzonyqw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3arkvwoxg.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3nnhvbkwl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3xpfrnqlx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3amtzvybb.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ediwygwd.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3vzwnlild.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3yjdwafem.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ohanwuua.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3seapjyyg.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3kgivyhgm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3xrcpkmrk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3jnsljkpk.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3lgosfxcw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jovoigqe.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ildbtuzy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hayamsmh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ssinraoe.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3gbjzswuz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3prwggakw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tvchnlud.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3pphystsw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3wmyhkbur.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3djhgaokl.html


<!-- 参考信息 -->