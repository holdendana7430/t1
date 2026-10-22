代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2ewkaerve.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2coomifzd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fpabappa.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2afgjxigl.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2nwxcpxac.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2kgtoigmy.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2pymrtgfr.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bhpipveu.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2ittirbjg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2qcnxtpbe.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2lvmckoto.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2npcvrtce.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zxpnliyf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2iyhffuud.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2rcrpagbb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cvxqbcem.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2iyraseah.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2yozblhid.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ufzmzpca.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2hemobvin.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2tzjupcfu.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2cszmkcoj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2gymcesgp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2uprpowwg.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2gpoqzmpa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vsyudhut.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2qgaoycbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ffmzhlic.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2qqvblrds.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2eewiviod.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2kfmdymre.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2znmeliyk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ychdclpn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2lyjsuubp.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2uavkrtcm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2mdvjwocr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2orabkjea.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2entauyne.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2sjssbooe.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmhpplwu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2krpycwqm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bbqupayt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fkipxnnv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2rdljbfmo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2gzuaynau.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vtgzmvlm.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2vkvzpkox.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2tlecvwku.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dunjjjif.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xppfutaa.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbouinok.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2exxsqbgw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2pxhctbhz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2eplezqha.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2jknstwcy.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2iilfgiao.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2udcbcoem.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2xwmceyai.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2kdpvrgvc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2npltlhew.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ezhtjizh.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2daxfqwef.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2hbbxkiwg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2pwsmptdz.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2yqiwkpws.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2kfxgxnnn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2pglbsvmm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2xanoxfwv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2zvpmnzqp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2smlenjup.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2exlrxfkh.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2dsxpgmjz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2jkiybdgd.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2nvhgnikw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2dqcncvrz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tusxgvqk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wjzqrjgj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2iwmapqed.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2lsilwlws.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2vlfwrjqz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2uzaxztoq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2cggsslmv.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2wfipipxv.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2esetnopm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkhzjwtd.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xqahdkvv.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qkzlsxix.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjfhbcvp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2uulotaqw.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ekusyxxe.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2prjprsvo.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2macggfrw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2pczuzyvv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ahoycexo.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gfaotapa.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pidwpdkv.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ltblctqs.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2kifkxtnw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2effcnplp.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vawdzsdr.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ybtbghgn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2jzlspomo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpjmcgwz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nrwwhhts.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtdpwhwp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zwliddyi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2rmpicnuy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2kocxjoot.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2voxllpes.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2dwzawzdu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2nxunxhzb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjrmhwme.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2nbqxztks.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2fzqeqbms.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ryqqelat.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2zoqthbus.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2iobhvqca.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2vkvwniac.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2okuecofx.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2tdlfryaz.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2iaqpaqdl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2nsfdewpj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mdwvsysf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2qcxynsxv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ljsyscws.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2wrmfirhx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2duqdzjmk.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2igcbkhzo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2mcpqrnip.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2xdjgqiey.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2fnmrskrz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nhdnzwda.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zwrevxci.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2vszediil.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2hxjsppeo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2xsyzhiqy.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2vdklqlyr.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2hmaylirc.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2vsoqvdwe.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2osexahvq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2vqnyfuba.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2lbmxtibt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2caqsljph.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2dkeulded.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2uawlpzph.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2talvsxzl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2fhglysdn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2nykwzvpl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2muejjzge.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2flbztvop.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zjfeykzc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2iiplkbtb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2jcrroixm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lvrvfyuc.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2lbsfeiby.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2jjwbeiix.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2eghrfqek.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pbzdbmne.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gtygxfap.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qtwfnchk.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oxgichdz.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2smewefdp.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rzuqoyhl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2kvriaoks.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2onirxmsh.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfprjfwh.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bydqizwz.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2uyascjle.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ybazsiws.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2jmwwwumc.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2dtgfaoge.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wzjwdnda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hoidrmde.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2scplvadf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cpbwiskh.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2zgvuzabv.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2fqnepgpg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jqapxgfa.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2idezhvxj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2buhuaful.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2moqckukw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2yckwjdwq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2wsgvaqds.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgbctcro.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2xblbitul.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2gzxgxdrz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2alivyzde.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ievyqhax.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2axgadkzy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2hqqscgry.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2wyoulbqn.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2qpcvggum.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2rzyhptai.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2wwusklij.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2atdegufx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2mewhxfmd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rdqbljeq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2hfjsqzpw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2zyzukuso.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2gsynmwfe.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2cdgjsmon.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2hhmkcxfm.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2lgbakaaz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2dlbbeala.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2zmhztbhw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2khjwgwak.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2maknzytc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2zaisuero.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2anrwfuab.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rahlawua.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dxaieyjk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2idtbmydn.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2hqfdqxgx.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2rmzxxfsn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2fhfwfrfz.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2rhfygnhg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2hnzjfkdj.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fbhrgscp.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2iqkqghpz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ahlqcoos.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2qdqpzsby.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2yeesgtfh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2zjijwshq.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2frpamlap.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lusvgbwz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2arcrkhqu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2wsexvxey.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wcbqhlkj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fsyebgsa.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2vhmcduod.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2nkrtqcuu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2paqfmlqw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2uxrhqnin.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2bydrftjd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2halowuqu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2hpqxifsk.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2bnwnymdg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2mmrilcpn.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2msubclcy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2zjjdgjix.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2txglynky.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbvgqiwl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2flsqoarn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2oscuqmux.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2egirzexv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2jnkiuzqz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2tarrlvsc.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2xvgjzpea.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2cddupsfl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2pnxqxvpr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2zjtwjxns.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2cgvhnbkn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2vgbdqnou.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2tfvvlnha.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2hxrmrbwd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xczpxjmi.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rjwuisnm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2mzisqnnj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2tkbwydoy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2etjsvwqs.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2gtvkhauj.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wrvivvod.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2inghednk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2huaazwbb.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mhattsgj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2kkmdupem.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2fswtihha.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2xwhtxizw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2uiagpxup.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ooxrtwty.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2alvytzsc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2cjoaajwv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2zjjinfyx.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2amuqpqph.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2wlbejyys.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2tdabyuqx.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2jmsrxlde.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ivijmcxr.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ehdejhyy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2wpyrcvqb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2qbpxhetq.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2rrxrdbme.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wakuplxt.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2cjsfaprn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bzrcmqvc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2torndkza.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2pthisdek.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjkpagqy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkvcuieg.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2idvtfpgo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2jvbefzng.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2mfyarrqf.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2krdzjjeo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2pfderige.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gajkqprq.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nrycowka.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2qyzhdvns.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2odydrenr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2raferiyz.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rcoyuyhh.html


<!-- 参考信息 -->