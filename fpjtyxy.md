代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ko.bookmarksfly.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jq.huanxung.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qn.hahajie.cn

[A17] 位运算
来源：http://wk.yuntaijiaju.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yj.wgjwhj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hb.haigaiapp.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://li.bookmarksfly.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dr.521024.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yy.shtwfgs.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://so.jianghongdianzi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kl.hnjuh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wt.hnjuh.cn

[A18] 字符与 ASCII 码互转
来源：http://ph.gzmigu.cn

Py:   ord("A"); chr(65)
来源：http://tf.shtwfgs.cn

PHP:  ord("A"); chr(65)
来源：http://sj.haigaiapp.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kc.szxytkj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oh.haigaiapp.cn

Java: (int) 'A'; (char) 65
来源：http://ss.hnjuh.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zz.huixiangedu.cn

Ruby: "A".ord; 65.chr
来源：http://pk.bookmarksfly.cn

C#:   (int)'A'; (char)65
来源：http://dx.huixiangedu.cn

[A19] 交换两个变量
来源：http://of.yuexingan06.cn

Py:   a, b = b, a
来源：http://wl.szxytkj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jn.shxzukj.cn

JS:   [a, b] = [b, a];
来源：http://be.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://uf.colortex.cn

Java: int t = a; a = b; b = t;
来源：http://cr.szxytkj.cn

Go:   a, b = b, a
来源：http://db.hahajie.cn

Ruby: a, b = b, a
来源：http://qx.bjjhwx.cn

C#:   (a, b) = (b, a);
来源：http://sj.nicolike.cn

[A20] 读取标准输入
来源：http://rj.muxihuayi.cn

Py:   name = input("请输入：")
来源：http://yu.bjjhwx.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://wz.huixiangedu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ux.szxytkj.cn

TS:   // Node.js：readline 模块
来源：http://qy.szsharing.cn

Java: new Scanner(System.in).nextLine()
来源：http://ch.huanxung.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xq.gzmigu.cn

Ruby: gets.chomp
来源：http://dm.asd995.cn

C#:   Console.ReadLine();
来源：http://vk.bjjhwx.cn

[A21] 保留指定小数位输出
来源：http://zy.haigaiapp.cn

Py:   f"{3.14159:.2f}"
来源：http://hh.muxihuayi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zs.nicolike.cn

JS:   (3.14159).toFixed(2)
来源：http://uj.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://ay.lnxyls.cn

Java: String.format("%.2f", 3.14159)
来源：http://pu.huixiangedu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nb.huixiangedu.cn

Ruby: format("%.2f", 3.14159)
来源：http://og.521024.cn

C#:   3.14159.ToString("F2")
来源：http://nf.lnxyls.cn

[A22] 获取字符串长度
来源：http://jl.hahajie.cn

Py:   len(s)
来源：http://rc.shtwfgs.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zt.szxytkj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bv.bjjhwx.cn

TS:   s.length
来源：http://pj.asd995.cn

Java: s.length()
来源：http://yk.asd995.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://aq.lnxyls.cn

Ruby: s.length
来源：http://gb.szsharing.cn

C#:   s.Length
来源：http://am.asd995.cn

[A23] 大小写转换
来源：http://pt.colortex.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://lo.chemitech.net.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://db.9csxet.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rh.hnjuh.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sf.muxihuayi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fr.huixiangedu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kt.shtwfgs.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qc.yuexingan06.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dc.huixiangedu.cn

[A24] 去除首尾空白
来源：http://rm.huixinmuqiang.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://af.asd995.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cs.chemitech.net.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xq.colortex.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ge.panjiajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vf.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://jv.hnjuh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://az.colortex.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://od.wgjwhj.cn

[A25] 字符串比较
来源：http://pt.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://yg.szsharing.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://as.chemitech.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://co.szsharing.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://my.jctech888.com.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pl.newstarts.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qx.huixinmuqiang.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zx.gzmigu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ba.bjjhwx.cn

[A26] 类型转换总览
来源：http://ve.colortex.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://he.bookmarksfly.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yl.hnjuh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hh.szsharing.cn

TS:   Number() String() Boolean() x as number
来源：http://vt.haigaiapp.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://da.asd995.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kc.haigaiapp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fh.asd995.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://da.huixiangedu.cn

================================================================================
来源：http://qi.muxihuayi.cn

B. 流程控制
来源：http://xj.shxzukj.cn

================================================================================
来源：http://gj.colortex.cn

[B01] 条件判断 if / else
来源：http://bt.jctech888.com.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jy.shtwfgs.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xw.colortex.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://oi.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fx.9csxet.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ex.haigaiapp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tf.yuntaijiaju.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fm.huixiangedu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ft.haigaiapp.cn

[B02] 多分支 else if / elif
来源：http://qk.hahajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rx.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://va.shxzukj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ab.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uq.szxytkj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dw.szsharing.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://oc.chemitech.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fk.shxzskj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://of.hnjuh.cn

[B03] switch / match / case
来源：http://zr.nicolike.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zt.9csxet.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hk.chemitech.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gy.asd995.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xx.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pk.colortex.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://et.gzmigu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ui.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tf.asd995.cn

[B04] for 计数循环
来源：http://yn.yuexingan06.cn

Py:   for i in range(10): print(i)
来源：http://rp.jctech888.com.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://iq.jctech888.com.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ik.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pu.haigaiapp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bz.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jd.yuexingan06.cn

Ruby: 10.times { |i| puts i }
来源：http://xa.jctech888.com.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jp.huixinmuqiang.cn

[B05] 遍历数组 / 列表
来源：http://zf.nszjky.cn

Py:   for item in arr: print(item)
来源：http://fq.lnxyls.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vb.hahajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tj.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ad.szsharing.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ny.haigaiapp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cc.hnjuh.cn

Ruby: arr.each { |item| puts item }
来源：http://he.hahajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rz.chemitech.net.cn

[B06] 遍历字典 / 对象
来源：http://fe.nszjky.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lz.bookmarksfly.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vf.huanxung.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ho.panjiajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lm.hahajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jr.haigaiapp.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ef.gzmigu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uz.hnjuh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lv.bjjhwx.cn

[B07] while 循环
来源：http://ef.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://ga.lnxyls.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zu.bjjhwx.cn

JS:   while (i < 10) { i++; }
来源：http://op.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://dw.jianghongdianzi.cn

Java: while (i < 10) { i++; }
来源：http://uf.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qb.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://tm.wgjwhj.cn

C#:   while (i < 10) { i++; }
来源：http://fb.asd995.cn

[B08] do-while（至少执行一次）
来源：http://nl.huixinmuqiang.cn

Py:   # 无 do-while：用 while True + break
来源：http://yx.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tq.gzmigu.cn

JS:   do { i++; } while (i < 10);
来源：http://ts.yuexingan06.cn

TS:   do { i++; } while (i < 10);
来源：http://zm.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://ln.szxytkj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://oe.yuexingan06.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jv.yuexingan06.cn

C#:   do { i++; } while (i < 10);
来源：http://mj.jianghongdianzi.cn

[B09] break 与 continue
来源：http://pv.yuexingan06.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fi.nicolike.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eq.521024.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zp.gzmigu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jf.wgjwhj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ud.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zb.bjjhwx.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qb.wgjwhj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fl.lnxyls.cn

[B10] 遍历同时拿索引
来源：http://ts.nszjky.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jo.huanxung.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fm.nicolike.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://su.bookmarksfly.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pi.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fh.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wc.yuexingan06.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ci.newstarts.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fg.colortex.cn

[B11] 生成数字序列 / 区间
来源：http://wz.nszjky.cn

Py:   list(range(0, 10, 2))
来源：http://tp.haigaiapp.cn

PHP:  range(0, 10, 2);
来源：http://ta.asd995.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zn.jianghongdianzi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jc.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cr.wgjwhj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jb.shtwfgs.cn

Ruby: (0...10).step(2).to_a
来源：http://ex.9csxet.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ql.muxihuayi.cn

[B12] 跳出多层循环
来源：http://tm.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://if.shxzskj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cv.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wb.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ic.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kg.9csxet.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kj.jctech888.com.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ox.haigaiapp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ou.hahajie.cn

[B13] 判断是否为数字
来源：http://xr.wgjwhj.cn

Py:   isinstance(x, (int, float))
来源：http://jl.nszjky.cn

PHP:  is_numeric($x)
来源：http://sf.9csxet.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zb.szxytkj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dv.wgjwhj.cn

Java: x instanceof Number
来源：http://od.shxzskj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rx.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://tc.bookmarksfly.cn

C#:   x is int or double or decimal
来源：http://sm.bjjhwx.cn

[B14] 判断值是否在集合内
来源：http://wu.gzmigu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wt.nszjky.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rv.jctech888.com.cn

JS:   [1, 2, 3].includes(x)
来源：http://oz.yuntaijiaju.cn

TS:   [1, 2, 3].includes(x)
来源：http://wb.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://uy.huixiangedu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kb.bookmarksfly.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vb.jianghongdianzi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nl.huixiangedu.cn

[B15] 布尔运算与取反
来源：http://bc.colortex.cn

Py:   a and b or not c
来源：http://yx.wgjwhj.cn

PHP:  $a && $b || !$c
来源：http://yb.panjiajie.cn

JS:   a && b || !c
来源：http://hw.jianghongdianzi.cn

TS:   a && b || !c
来源：http://ij.huanxung.cn

Java: a && b || !c
来源：http://vu.hnjuh.cn

Go:   a && b || !c
来源：http://jp.haigaiapp.cn

Ruby: a && b || !c
来源：http://up.bjjhwx.cn

C#:   a && b || !c
来源：http://gv.wgjwhj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lx.asd995.cn

Py:   if not data: return
来源：http://hz.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://be.newstarts.cn

JS:   if (!data) return;
来源：http://bf.hnjuh.cn

TS:   if (!data) return;
来源：http://cu.wgjwhj.cn

Java: if (data == null) return;
来源：http://vl.yuntaijiaju.cn

Go:   if data == nil { return }
来源：http://po.colortex.cn

Ruby: return if data.nil?
来源：http://jz.asd995.cn

C#:   if (data == null) return;
来源：http://xv.shtwfgs.cn

================================================================================
来源：http://pm.jianghongdianzi.cn

C. 函数与作用域
来源：http://xk.shtwfgs.cn

================================================================================
来源：http://jz.muxihuayi.cn

[C01] 定义函数
来源：http://sv.gzmigu.cn

Py:   def add(a, b): return a + b
来源：http://oc.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nn.asd995.cn

JS:   function add(a, b) { return a + b; }
来源：http://vd.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dr.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://km.bookmarksfly.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nx.haigaiapp.cn

Ruby: def add(a, b); a + b; end
来源：http://lv.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wu.szxytkj.cn

[C02] 默认参数
来源：http://ym.lnxyls.cn

Py:   def greet(name="World"): return name
来源：http://aw.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://oc.lnxyls.cn

JS:   function greet(name = "World") { return name; }
来源：http://cd.bjjhwx.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ze.hnjuh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gs.nszjky.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hi.yuexingan06.cn

Ruby: def greet(name = "World") = name
来源：http://vo.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://wc.lnxyls.cn

[C03] 可变参数
来源：http://ei.shxzukj.cn

Py:   def total(*args): return sum(args)
来源：http://hx.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mk.huixiangedu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fk.colortex.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xr.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ns.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://do.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yb.9csxet.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rt.huanxung.cn

[C04] 命名参数 / 关键字参数
来源：http://iq.nszjky.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kg.szxytkj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bc.hahajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ga.gzmigu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ye.shxzukj.cn

Java: // 无：用 Builder 模式或 record
来源：http://et.huanxung.cn

Go:   // 无：用配置结构体参数
来源：http://ow.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://qm.newstarts.cn

C#:   f(a: 1, b: 2)
来源：http://jm.bookmarksfly.cn

[C05] 返回多个值
来源：http://tn.yuntaijiaju.cn

Py:   return a, b
来源：http://ak.panjiajie.cn

PHP:  return [$a, $b];
来源：http://za.newstarts.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ed.shxzukj.cn

TS:   return { a, b };
来源：http://se.gzmigu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xe.shtwfgs.cn

Go:   return a, b
来源：http://qs.9csxet.cn

Ruby: return a, b
来源：http://aw.jianghongdianzi.cn

C#:   return (a, b);              // ValueTuple
来源：http://xp.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://mu.szxytkj.cn

Py:   square = lambda x: x * x
来源：http://xf.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xp.nicolike.cn

JS:   const square = x => x * x;
来源：http://sm.haigaiapp.cn

TS:   const square = (x: number): number => x * x;
来源：http://xb.nicolike.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zy.nicolike.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ez.9csxet.cn

Ruby: square = ->(x) { x * x }
来源：http://vb.9csxet.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pr.shtwfgs.cn

[C07] 把函数作为参数传入
来源：http://he.huixiangedu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gl.asd995.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ub.shtwfgs.cn


<!-- 参考信息 -->