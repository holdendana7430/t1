代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jorwtfhl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2dsrzmfdu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2fjzniqul.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gubceqpa.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2dhzmkxyb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2hwbedxyk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2mblrjtus.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2fajofvwp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2kpgitbfe.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2rzexnzsk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2wogzwtmk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2jhaedccd.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2uumwnoki.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2aiugsdow.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2drikvnah.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2gwhklyck.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2yjcllkeb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2taesilem.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2yrnhsxpg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2sylmeman.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2cvkyonyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tvrdjihw.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2odsnuvld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mppszygn.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2rizeyvaj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2csdrgwoj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgwxdckw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2fgqjbuje.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2sqhteoif.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2shilbofr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2uotnzxza.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2azhuhbny.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2lhjmywkq.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2ftdykuvc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2gyzperxc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjnfkppl.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fwdrfdgp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2spzqqavj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ccmnqazw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2hmxmpkpb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2exazsgvk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jqzrdvzf.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2bxryhdgm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2kbedffim.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ndkcvksh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fevhttfe.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hizdurni.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vhzvyssv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2bvhzjnse.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2opmgttvo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2abxtdiof.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2jgpxjndb.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ttigfogf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2agvdegda.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2igzqezfv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qfnqeamr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2rdoockls.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2nijisvtr.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2odrfzsvl.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2bhnjyzjx.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2xvwtlhpu.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2rfixjwjj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2veaqozqw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qhwypugv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2duwkxufi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2zsrbllps.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ddbtfkvh.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2usjfdecw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2aehjqutr.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2turidtoq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2jgwgaqdm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2rquuoeez.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2fnigmzia.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2mwgyfbqe.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2fhrocwum.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2nwxpdzsr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2qcwoiqmd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2clqjacen.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2bjyojjeg.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2lwwmuzvt.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsmdhpdl.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lselywhu.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kyrgwzwi.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhgrjqxm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2kucvqpbf.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2wfntynqp.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bevtqslu.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2xgmecynb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2oovbzkco.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pbvdpndr.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tshkuuet.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kkyligfb.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rdtbgflm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2nttybgnd.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2rlcgiglf.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ktfuydzv.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2oinnwmwz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ronmtnqx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mfxbptzb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ckjmeyjw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dtazmqdf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rdujznso.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ewxarsyi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2tsgiodai.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lekttfuj.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2lurheaaj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2minkvcvg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2csllvtlq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2rxpalgic.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2crrnyoft.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2nkrxiurt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2nwhrpgkr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2yuixfhgc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2fxvuklmt.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2fszbcvpt.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2uaxcjdvc.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ftkmislj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tsrxhqfo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nfvhwkcq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tbhlrasi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2hcywridl.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2tbzwqpho.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2erjtdqpz.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2xcddvorp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2afwzggat.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2rcotjgfs.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2lbgnhjeo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kvgmjqcq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nsceosjp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2drslsreu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2dtizdpmy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2gvgbzpyk.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2axnublyt.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2rtltfspj.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2wrhpbwtd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2gxrkkhbg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ejkuyohy.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2pldwessv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ugxcyjtt.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ojlssrcn.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2fwuebphm.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2eargpzjy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2wikkpuce.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2pskjmfos.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tgzzywxp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2aztrcovf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jcuaquba.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2dtyecgpt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2bdxsyrev.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2shdyvvtp.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2olpyurwq.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2ozooktot.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2bknamuki.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fqlutipa.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hmcagtrq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jpjilhbq.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jpmpagdn.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qmfnkbjz.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yztqvqfp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2mxcqrxjp.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2kbaqrbnf.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2oruymmgr.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2mxkilnbc.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qdyrpuoe.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vrydatcy.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2qsduqxme.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2horqnyop.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2cvfqilpt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qfqzvvpe.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2phuhqzyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ihllyfkq.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2sfqgnpsy.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2slwgzhlr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qyidfsrr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnqenrmj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2luncgkbq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlqnnffg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2vnmmzqfe.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2htnlrsto.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgewubwg.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ixmygcat.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2uicxovjo.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2asmlngue.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cevxhbxc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hoqdfbey.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2cuacdqzi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2gbmbncto.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ewvjvwvs.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2siwnvaso.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2aywotpfz.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2lujhclgl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2anycwfsb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2zaorqmus.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2lqlkfynq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2brldnxpu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ikokqhzg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2hllgsudi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2rwalmkic.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ugkhpdqc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2kbgmrfih.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2aoczljkd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2lbvmqrdk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2misbtdmf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2klimjjin.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2dhhhlhms.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2nextimud.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rgoaupkv.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2cxsrwkrs.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2octuzdfz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2rficljbq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2mtmfqvge.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2mehhciwb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2pfiboocz.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ywusrxxs.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2agzphegd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2zxaccxrf.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2zaaugaqn.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2ijhsjhqk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2prmibtjm.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2axgfbjye.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mdwcczps.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xgswxyhf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2ovguwset.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ifniotvk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gfqkneqc.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2rqdslqmq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2kvzdbzgy.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yrzcxovn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2zbkqfmam.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2olnpgdhm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2jrrvhpjg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2bakorvcu.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2tblhjvrv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2hasadein.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ynyueshw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2pzbkvoym.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcmvibhm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2shnwxqub.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdmjzkzs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2tpyhdomc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2plrlfrfs.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ajbufarg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2czjqwkvl.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2xqjcxdbk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2hftaxycc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwwmfxlm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2dvjixmwm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ktzixqxa.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2mhdpyljw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2cgaocfil.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ibefsulg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fmcxoizr.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gxebvdyo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2xfalpjzb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2imldegua.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2axejswyl.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2fsulegow.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mysoihpd.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ocdgmmel.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2pjahmeqg.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2tmlhndmi.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2dnbbsyse.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2twgqyqpg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2jkfrklks.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ebvrkton.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ivyqbldt.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2falutduz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2vqwbuocz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2hwvjnvuu.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2syqadqxd.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2xhoznnbn.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2icfxofbi.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2pwinzkqa.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2pypdvwqz.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2hwusjqbb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2fwsdncan.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ctwuckmp.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2bdygzrmz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2muvunljd.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2wkvtmoup.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2oftgbtyn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ewwgcefr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2psjfgxgc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjpnhasp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixdyvrly.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2rxoqryat.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2xpnyirrz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2smfsbcbj.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2phkohlic.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2esrphwzp.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2iewymiqi.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2uqcotlqc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2spvcjzws.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2njahpola.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ohxhsmmp.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wucetkls.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2oivsppxj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ztdjoguu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2fwrglcmv.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2lmwnakri.html


<!-- 参考信息 -->