代发 wailian999

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2irseditb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2hxguehvk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2uijovktu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2jrlmwtiw.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2rpmptnsf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2jrbynvlo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2bwhfrflb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rvmdgywk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2viknkxeo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qcakhvze.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2dfonniyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sfxbbonq.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2plkjnrpt.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2ylddowhj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjmegqns.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wffxlkrr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2htkanpaw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2cnatscea.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2okdwobxl.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2fnbdnrsy.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ygqkzcte.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2voxgrzno.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2ieuatxia.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2qyokhzat.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2aupdbczb.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dhgfdlfq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fgyawobo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2ssyzyfqt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2pdevsbmp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2flrtrmqs.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2tkoytglj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2knckmduc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyxilssa.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdirwgof.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdmkiaag.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rpbtkncz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2lamtqueb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2kvxproee.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2jondcxhy.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2hpbucczn.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xgxawwil.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2hnpvwhsc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dolevaop.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2seqcrwic.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2wvhkfbbz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2slzcstwv.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ycmfcvxo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2dklrfcws.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dpndrqkc.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2efeuwcte.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsxrwgzx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2foxfvviq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2dvusyqfk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wuynlgig.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2fnhmumko.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ykmstbpq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rpzyqmnv.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2ndczdibg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2qwelegrg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2bkbcpupa.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ckybhanv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2boycweze.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2zkocptpu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2tbcdhnzu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2optbzylg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2cggqcdgt.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2adljkmti.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2qhvzrxff.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqlnhegy.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmxaqpnv.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzargqmq.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fxtlkkjx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2vmzdfxxu.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2dtalfbnv.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2abdebais.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2fuxtuqhh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2axchmdtq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uvvcsfoj.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xjkvtnzd.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yoqgbmqs.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2stpvrdok.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ehkowclz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2dghrqosv.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gkbgxpce.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2xccgkqqx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ykfkphgy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2auefiyjl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqvmeadt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wwwsntuz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bfpxcaxd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2xerdgafq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2bfiotpez.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2upiwtrxi.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2bekcvqyd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2mcsjebkz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2ggotuenh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2dkfictmx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ujrboboz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2stsdowqf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2puanyuvc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2udipkvau.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2mwjgmedi.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2lczqpwji.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2vcwpjqyz.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2grrouamz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2pwxxaric.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pqratuhm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lxwroxbb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2vsmpbdfh.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2tptunzem.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ihiglqsf.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2fmqifcqi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2gnqgjjsv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2bfyhqpvy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2imjyxawa.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zqkyicck.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zqekaupr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2eznvljaw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2gythhopj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2vukhzkew.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2fdhwngny.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2nqizjokx.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2zimqmaya.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2salyzcti.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2jnhofnsw.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2mdpewjym.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2japzgdof.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2cmqcrrwc.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2xddyuorb.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2zoczglgw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2mhnnyeoz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2klgbraei.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xfkxbvdm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nbqynqfv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jrmzdkme.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2cddoeeqg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2vlimadxo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2anhberai.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2hzzlzfkv.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2riefsvqh.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2prkqicec.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rijlzqty.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2eaaeglwv.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ejsmapcy.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cekbpvad.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qobduljw.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bwmqbejs.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2htlwnkwh.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2rvubbysv.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2qooqaixh.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ufmtuezd.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2gubjrpul.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hsoopscd.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ubyaavqr.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2xqouhcnp.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2heagovpr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pxpmeego.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2zxzuyvgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xcracvzd.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2uzuwupcs.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2hqjzqwvg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2sagvopjt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kibywfpq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dydgsjds.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcacrhfp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2kvdiyhip.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2fkdirvmp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkpdqium.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2uhmddsjs.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2dmyataux.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkbkxrra.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgboszzi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rljjzjks.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2qvmszaid.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2lqasfyyp.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2mqizusll.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2jkfdecno.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2tuubkckq.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2idsjqcge.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2vpvcogdt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bsizpkof.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2wyyxggzc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oluhtewm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2oawlfuli.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2jjrrcmrp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2xbjznrsf.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2hemsoflc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ugzgtqpe.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2mpedteqs.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2tqepwuku.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2jtrcmkvl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2bjllnnuc.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2jbzzrumz.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wmkbabnj.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rfvigzip.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2eilmqsrz.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2yowxouuj.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2eshdvizo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2auufsjhi.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2gjvkvhbe.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2pnmgkhwd.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ijqzmgud.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2yvlerjks.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2sakuiqse.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2crwixxwv.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2ngpycidv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2dsfacjwc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ftjkjyhp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gwjawexx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mjvznhbi.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2gddswuhh.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2kdtveyzm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2belujbon.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2pamiepmi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2mzuakazo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vcaflbth.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2inmzzupp.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2odwfbxgy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ueligpzh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2qacaybgn.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ietlbtca.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ezccdico.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2soqdtgac.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2umpcyzon.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofelvaev.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mczasyyl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnyzlohi.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2qvapwwys.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ontfhmbx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2osuuoboz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dpkpajfe.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2apfatpdx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2iegqfocx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ehzflqfj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ehubroib.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2phhqxycp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2hialowgw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2xplgmfzz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2klmsyfnq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hruulchv.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2qgpubhec.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2pdtaishi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2mpxdukxg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jtvclsyu.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ozkzjriq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ggsyewix.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ahsfgter.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2etterzwq.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hxthsnmo.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ywnyvbhu.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2zuycotur.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2crfvajyf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jnpywats.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2nrmhjpsl.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2snzzpnpz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ypxqpbpx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2imzwawdr.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2mbzssrdc.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ogesabil.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2lpbbigmb.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2udxxhqvh.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2jynznwsl.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ydmwrswk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2qddastfz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2qgehxbuo.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2aqfvrmii.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ektmljhq.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2nfmywjbt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lthuomcv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2syfkjrby.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2lywkhwoz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfdyugzb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxlbjxlq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2vjvizqas.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2bygzjyzr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2vqqqylod.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2xsrajiie.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ixwvikqd.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ggwfglby.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2brovixhc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2wmirffaf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2vhpfemhk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ncimscjv.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wvwsinnm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ucldhqwn.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2bvizuigr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2uwlvdfaj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2drqnpbxi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2dvcnpxdr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ailocrkp.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2djyhmnyu.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2xbkknakt.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2gwzkxupi.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2radgwehn.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2isdenbef.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2zekllkvn.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2woijfpbv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2goozkktu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2mkkeufzy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2biyeqyhq.html


<!-- 参考信息 -->