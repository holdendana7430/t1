代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://un.jianghongdianzi.cn

TS:   const value = data ?? "默认值";
来源：http://yh.jianghongdianzi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bd.chemitech.net.cn

Go:   if data == "" { data = "默认值" }
来源：http://mu.bjjhwx.cn

Ruby: value = data || "默认值"
来源：http://rz.chemitech.net.cn

C#:   var value = data ?? "默认值";
来源：http://qy.newstarts.cn

[A16] 真假值判断规则
来源：http://wp.wgjwhj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://sp.szsharing.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://oz.bookmarksfly.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xq.yuntaijiaju.cn

TS:   if (!x) {}
来源：http://ke.9csxet.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xr.9csxet.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bl.panjiajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://fp.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kc.szsharing.cn

[A17] 位运算
来源：http://pp.panjiajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bs.szsharing.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wl.jctech888.com.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jg.chemitech.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://si.wgjwhj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mp.chemitech.net.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://df.huixiangedu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xg.muxihuayi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://je.hnjuh.cn

[A18] 字符与 ASCII 码互转
来源：http://cz.9csxet.cn

Py:   ord("A"); chr(65)
来源：http://uc.wgjwhj.cn

PHP:  ord("A"); chr(65)
来源：http://oe.panjiajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lc.gzmigu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ej.huixiangedu.cn

Java: (int) 'A'; (char) 65
来源：http://oa.9csxet.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fu.szsharing.cn

Ruby: "A".ord; 65.chr
来源：http://ha.yuexingan06.cn

C#:   (int)'A'; (char)65
来源：http://vx.colortex.cn

[A19] 交换两个变量
来源：http://sm.asd995.cn

Py:   a, b = b, a
来源：http://ad.lnxyls.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://pw.gzmigu.cn

JS:   [a, b] = [b, a];
来源：http://fu.hnjuh.cn

TS:   [a, b] = [b, a];
来源：http://dv.gzmigu.cn

Java: int t = a; a = b; b = t;
来源：http://nh.huixiangedu.cn

Go:   a, b = b, a
来源：http://iu.huixiangedu.cn

Ruby: a, b = b, a
来源：http://us.wgjwhj.cn

C#:   (a, b) = (b, a);
来源：http://jt.nszjky.cn

[A20] 读取标准输入
来源：http://al.huanxung.cn

Py:   name = input("请输入：")
来源：http://rs.chemitech.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zk.newstarts.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hs.colortex.cn

TS:   // Node.js：readline 模块
来源：http://fj.szsharing.cn

Java: new Scanner(System.in).nextLine()
来源：http://lh.bookmarksfly.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yw.jianghongdianzi.cn

Ruby: gets.chomp
来源：http://wf.szxytkj.cn

C#:   Console.ReadLine();
来源：http://sz.shxzskj.cn

[A21] 保留指定小数位输出
来源：http://ws.bookmarksfly.cn

Py:   f"{3.14159:.2f}"
来源：http://an.jctech888.com.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rd.asd995.cn

JS:   (3.14159).toFixed(2)
来源：http://vu.shtwfgs.cn

TS:   (3.14159).toFixed(2)
来源：http://eg.newstarts.cn

Java: String.format("%.2f", 3.14159)
来源：http://fs.nszjky.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fo.huixiangedu.cn

Ruby: format("%.2f", 3.14159)
来源：http://xd.gzmigu.cn

C#:   3.14159.ToString("F2")
来源：http://iq.521024.cn

[A22] 获取字符串长度
来源：http://cf.hahajie.cn

Py:   len(s)
来源：http://hf.jctech888.com.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fv.muxihuayi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gs.chemitech.net.cn

TS:   s.length
来源：http://ns.521024.cn

Java: s.length()
来源：http://lu.bookmarksfly.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ru.chemitech.net.cn

Ruby: s.length
来源：http://jy.haigaiapp.cn

C#:   s.Length
来源：http://zj.nszjky.cn

[A23] 大小写转换
来源：http://tx.chemitech.net.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gm.bjjhwx.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vt.yuntaijiaju.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ti.panjiajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://au.szxytkj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ey.shtwfgs.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ot.muxihuayi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rz.chemitech.net.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://si.chemitech.net.cn

[A24] 去除首尾空白
来源：http://qo.shxzskj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ap.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ea.521024.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gp.yuexingan06.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gp.bjjhwx.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hg.lnxyls.cn

Go:   strings.TrimSpace(s)
来源：http://sf.muxihuayi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vp.shxzukj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qp.hnjuh.cn

[A25] 字符串比较
来源：http://cl.wgjwhj.cn

Py:   s1 == s2; s1 != s2
来源：http://qv.asd995.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://la.shtwfgs.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fz.haigaiapp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://or.9csxet.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ti.shxzukj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dw.nszjky.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://of.panjiajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://oc.newstarts.cn

[A26] 类型转换总览
来源：http://gm.521024.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hv.nszjky.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xp.shxzukj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ku.panjiajie.cn

TS:   Number() String() Boolean() x as number
来源：http://uc.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lm.bookmarksfly.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ei.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://og.bjjhwx.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://do.hnjuh.cn

================================================================================
来源：http://xq.bookmarksfly.cn

B. 流程控制
来源：http://ni.nszjky.cn

================================================================================
来源：http://bv.hnjuh.cn

[B01] 条件判断 if / else
来源：http://th.chemitech.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://oy.huixinmuqiang.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ul.huanxung.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dj.huanxung.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mf.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gc.panjiajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wi.muxihuayi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ex.521024.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://il.newstarts.cn

[B02] 多分支 else if / elif
来源：http://vn.lnxyls.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://aj.haigaiapp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bj.panjiajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yu.asd995.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://az.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ny.asd995.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ls.jianghongdianzi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lm.bookmarksfly.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tq.asd995.cn

[B03] switch / match / case
来源：http://jy.hnjuh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ko.chemitech.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ov.chemitech.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dh.shxzskj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dc.asd995.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xq.huixinmuqiang.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ev.nicolike.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gv.newstarts.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kn.szxytkj.cn

[B04] for 计数循环
来源：http://sk.9csxet.cn

Py:   for i in range(10): print(i)
来源：http://zs.newstarts.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://up.colortex.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wi.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ow.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mq.huixinmuqiang.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vi.jctech888.com.cn

Ruby: 10.times { |i| puts i }
来源：http://gw.shxzukj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lf.yuntaijiaju.cn

[B05] 遍历数组 / 列表
来源：http://fu.huixiangedu.cn

Py:   for item in arr: print(item)
来源：http://dq.hahajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lg.wgjwhj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bk.lnxyls.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rp.nicolike.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gb.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rh.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://lm.hnjuh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ux.huixinmuqiang.cn

[B06] 遍历字典 / 对象
来源：http://ho.wgjwhj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ja.haigaiapp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vd.chemitech.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aa.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xl.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hb.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ma.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mh.9csxet.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tp.bjjhwx.cn

[B07] while 循环
来源：http://ri.huanxung.cn

Py:   while i < 10: i += 1
来源：http://wv.szsharing.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bo.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://hx.bookmarksfly.cn

TS:   while (i < 10) { i++; }
来源：http://hr.newstarts.cn

Java: while (i < 10) { i++; }
来源：http://gw.shxzukj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dz.lnxyls.cn

Ruby: while i < 10; i += 1; end
来源：http://ay.shtwfgs.cn

C#:   while (i < 10) { i++; }
来源：http://kj.hnjuh.cn

[B08] do-while（至少执行一次）
来源：http://kv.haigaiapp.cn

Py:   # 无 do-while：用 while True + break
来源：http://ed.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ge.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://ys.shxzskj.cn

TS:   do { i++; } while (i < 10);
来源：http://ix.newstarts.cn

Java: do { i++; } while (i < 10);
来源：http://px.asd995.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vx.chemitech.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lv.shtwfgs.cn

C#:   do { i++; } while (i < 10);
来源：http://oh.hahajie.cn

[B09] break 与 continue
来源：http://od.bookmarksfly.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://og.huanxung.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uj.nszjky.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bc.nszjky.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lw.shtwfgs.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bp.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hd.yuexingan06.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nv.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zc.gzmigu.cn

[B10] 遍历同时拿索引
来源：http://zo.szsharing.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yg.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ts.yuntaijiaju.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tb.gzmigu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://me.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ta.shxzukj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wt.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xw.jianghongdianzi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://oo.huixinmuqiang.cn

[B11] 生成数字序列 / 区间
来源：http://zv.wgjwhj.cn

Py:   list(range(0, 10, 2))
来源：http://yv.nicolike.cn

PHP:  range(0, 10, 2);
来源：http://lh.9csxet.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://di.gzmigu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uf.asd995.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rj.chemitech.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ec.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://iz.asd995.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tp.shtwfgs.cn

[B12] 跳出多层循环
来源：http://mb.bjjhwx.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kb.9csxet.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ra.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dh.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bw.panjiajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ey.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bi.hahajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oj.yuexingan06.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zl.gzmigu.cn

[B13] 判断是否为数字
来源：http://tn.shxzskj.cn

Py:   isinstance(x, (int, float))
来源：http://yb.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://kj.jianghongdianzi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vc.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xc.shxzskj.cn

Java: x instanceof Number
来源：http://es.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cf.panjiajie.cn

Ruby: x.is_a?(Numeric)
来源：http://gy.hahajie.cn

C#:   x is int or double or decimal
来源：http://us.nszjky.cn

[B14] 判断值是否在集合内
来源：http://cg.newstarts.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://or.huixiangedu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oy.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://fw.huixiangedu.cn

TS:   [1, 2, 3].includes(x)
来源：http://ov.panjiajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ls.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mb.wgjwhj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nj.nszjky.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://up.szsharing.cn

[B15] 布尔运算与取反
来源：http://yo.hnjuh.cn

Py:   a and b or not c
来源：http://mj.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://fr.szsharing.cn

JS:   a && b || !c
来源：http://fb.bjjhwx.cn

TS:   a && b || !c
来源：http://xh.szsharing.cn

Java: a && b || !c
来源：http://to.jianghongdianzi.cn

Go:   a && b || !c
来源：http://zw.chemitech.net.cn

Ruby: a && b || !c
来源：http://yd.nicolike.cn

C#:   a && b || !c
来源：http://oz.gzmigu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gp.asd995.cn

Py:   if not data: return
来源：http://aa.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://uk.newstarts.cn

JS:   if (!data) return;
来源：http://ru.9csxet.cn

TS:   if (!data) return;
来源：http://mw.lnxyls.cn

Java: if (data == null) return;
来源：http://by.521024.cn

Go:   if data == nil { return }
来源：http://ip.haigaiapp.cn

Ruby: return if data.nil?
来源：http://sy.szsharing.cn

C#:   if (data == null) return;
来源：http://gr.wgjwhj.cn

================================================================================
来源：http://wr.haigaiapp.cn

C. 函数与作用域
来源：http://yc.jianghongdianzi.cn

================================================================================
来源：http://az.hahajie.cn

[C01] 定义函数
来源：http://xl.yuexingan06.cn

Py:   def add(a, b): return a + b
来源：http://vh.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tj.hahajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://hu.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rg.bookmarksfly.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://px.asd995.cn

Go:   func add(a, b int) int { return a + b }
来源：http://no.bookmarksfly.cn

Ruby: def add(a, b); a + b; end
来源：http://iy.huanxung.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pr.521024.cn

[C02] 默认参数
来源：http://ai.521024.cn

Py:   def greet(name="World"): return name
来源：http://ox.shtwfgs.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wz.newstarts.cn

JS:   function greet(name = "World") { return name; }
来源：http://bk.newstarts.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://os.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ri.521024.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://db.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://ad.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://qp.wgjwhj.cn

[C03] 可变参数
来源：http://wm.wgjwhj.cn

Py:   def total(*args): return sum(args)
来源：http://ww.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bn.haigaiapp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://be.9csxet.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gk.shxzskj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hq.gzmigu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xi.chemitech.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yf.bjjhwx.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://iw.jianghongdianzi.cn

[C04] 命名参数 / 关键字参数
来源：http://nx.muxihuayi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://my.colortex.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rs.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tk.nszjky.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ud.521024.cn

Java: // 无：用 Builder 模式或 record
来源：http://wx.9csxet.cn

Go:   // 无：用配置结构体参数
来源：http://xg.haigaiapp.cn

Ruby: f(a: 1, b: 2)
来源：http://gx.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://nw.newstarts.cn

[C05] 返回多个值
来源：http://mp.shxzskj.cn

Py:   return a, b
来源：http://uh.gzmigu.cn

PHP:  return [$a, $b];
来源：http://io.yuexingan06.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://si.chemitech.net.cn

TS:   return { a, b };
来源：http://vr.asd995.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ec.shxzskj.cn

Go:   return a, b
来源：http://vz.huixinmuqiang.cn

Ruby: return a, b
来源：http://ap.hnjuh.cn

C#:   return (a, b);              // ValueTuple
来源：http://sw.hnjuh.cn


<!-- 参考信息 -->