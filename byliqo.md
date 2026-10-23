代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3mnxqezrw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3odnpufkm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nmipknuv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3gujghwee.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3ouvkmhxr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3dwucgmdm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3tmzrrvac.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3lxxtqcpo.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3ibtwyxen.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3srhchbbf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3uvgpeqfw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3xyyzsdqc.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3eznbullb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3gvtlwaon.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3qvmoiekc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3hzacyqnn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3fhojrcae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xyzkuwqb.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3vbboxnmu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qtjmdlfv.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3qxoyfxgk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3fkjyprox.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3nlczoakp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3licgtncq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3dcgbnmbv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3nvivqkjm.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3qhwjpnbl.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3wlojxbmd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ytyluhdd.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3lultvfrt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3chhvwmbn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3osevnlyb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rfjhhzhu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3oavqsugi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gppbvyfv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3fozajfmb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ulaiiyon.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3aukaobuw.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3tudqnimn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3sokzqvje.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktdcjfbh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjpakqkq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxrzarpt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cjzwfwbp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ihkvzqwz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3junnesdm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3yzizfpyb.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3esnoxqde.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3gthydrms.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbbpbipp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3zetrxzxv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ekxtivod.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fznnamtv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3sghceumx.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3igximsrf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3zthegbko.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3kqpabaxv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3fzikctsa.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3ufxpebqh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3hncrnxbf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hvivesdw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uvymacin.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3lqqtwjiz.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3mcbdqrmd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3yuatujlu.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3yqlnglik.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3qmfftehb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrenjaak.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3thsihnsx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3bnjzrudo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3jftengcq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3qsocjkdk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3vaozdxnx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3wcltirut.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3rsvacfxu.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3fhbernwb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tifntiex.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xoasybif.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xppkyruw.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rfynulsa.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3sphyppuy.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3acmtihpg.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hvlhskrb.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3qcpseccc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3joapewzp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xnnbndef.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ghelrptz.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rzhndwow.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mgqnwrgg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3gibirthe.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3dqldzlzk.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3crfdalgt.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3iqxrqgac.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3zjryxhui.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdevytxw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vilkcnlu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrrlvcfr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3evfzrxia.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ddtdfqfm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3qxcfacie.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzgfzown.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3fxesguee.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3jraagozr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3jyxoebkv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3kbuztdtl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ifdbmynr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3dvcamcyy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3vtbchnht.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ggabsvxe.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ynkhnsvd.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3pwrjlesl.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3ddlnbhit.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xtbdbtkq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3fpejyfaq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bxmonpdr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3xkukyidq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ezdgsfux.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3wkadhoce.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3fkiqgxhc.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3fdiakktg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3sdjwfcxu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3gacbssxj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vufxxkrw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ojjczald.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3migmvgwt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3kkkdypyh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3irpwwglv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3vqxtftdx.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3rqlttzhf.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3vcbslzxf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3bowefyhb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3utwclsue.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xucrzwpw.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3mxwkfbzz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ejipffku.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3skkelhyy.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3kynqirtf.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3txfwgkxj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3fuontjbd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3vginixoz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fwfjivfx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3slkuphly.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lersoylt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lcabyaqu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sfvtowmi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gpcpjkrb.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3cbppntyo.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3hvymhdba.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ulyqrycn.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vwmoyhtq.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rdvjlllg.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3oydirjan.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mqnciwur.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ocqplrso.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3drouopzh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3fetvvdab.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3mtudqtle.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdsnocrt.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3zilnykmo.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3qjcizlwg.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dnzehwbh.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3rrnvshgb.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3gohvqaso.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3yiznhwxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sbaomnhp.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jjnmrfex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3upvcxsff.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3itksrqtp.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3byrvaikl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmkoaaqb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yisfwvdz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dijqookn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpsawipf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3amttijzj.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3bweddian.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qubkhigr.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3lvhrxxtb.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3vjnuydyu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3niqfjqoc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cyznzfuh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rufxzive.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ljtpgubo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3wjffadmy.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3tnqmmztu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3hvfmxbvf.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3wbywoztv.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3pbkdptvo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3egmopxfz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3eiqgrkru.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxesmmrq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3rjpravpm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3oorbkzvp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3civkufls.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3mfrrzlcb.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3zxzeroud.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3weowchkl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ofgwvehe.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3waoaufrq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3fkaazecc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3yeoralxd.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3onoiyxkz.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ueakfjme.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3egwcmysh.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3mwfkkmvg.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3aktozxeh.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3zzkmdnzj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3vsbjwphq.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3wggxvopg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3rsyiesfr.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3chxnhasi.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pebqprrs.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3kseenoqi.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3ddinvyxw.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3cgzcdmhb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3dtagpftb.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ymapvbmo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qbosmdnn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3rmpmkjht.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3rgtbkdrb.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3xiaereix.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3szhvhflo.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3yvdbxywv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3zdvhuzot.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3zswilvch.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3zezyxhfd.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3bmzlkbvd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uemizsac.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ovxrvesq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3imtfwlxb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3yyfzonlr.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3bmrgfori.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3oeblvplh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3dwnbecwx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pkugtzbi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3aiuzxesv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3amqyymrv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3mmswincc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ksephofl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3opzdayxg.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3kyiqqkhp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3aijlaogx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3qvrbbyrq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3usrjhdfc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3pfyadeus.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3bibusivh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3aitgmqan.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wenyvbxn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3eafdyjwc.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3zyklpsnn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3jtuxiran.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3gvfvzzth.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3ddpweirk.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3mpszdlzt.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3okxifqay.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vjefkyoh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3bdtfporh.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kdugntzj.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3sxtpmcpo.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3pwpjxhsh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ypewkwws.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3wvjydjwd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3ztnukxsw.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3sdggteco.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3wiugscaw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3rxtoqwxs.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3sneswshb.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3pvxxgwhe.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3helftfms.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3bimujhin.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3hjqzlfie.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3dhydlxmh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3pkdbmeez.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ozbriapq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3nvyajdyf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3zbnjvpck.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3qfgnuyec.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3dzsmtjci.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ozcqydtn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3lcwiysob.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wwpwifmn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3grugjzaf.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3npdeuedl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3vpvoskld.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3phoyvruh.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3hgmusjkw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3pauroeie.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3esxeihhb.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nwpnpmxt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3hjakccid.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3suxttzoe.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3bbxaczib.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3pxmemsip.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3fhvfcmga.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3vxunijmy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3aiqicfhe.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3giogffyt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oudtjbgg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bfjlqgfs.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3lqibeppd.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3dwblinwb.html


<!-- 参考信息 -->