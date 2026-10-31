代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://gg.shxzukj.cn

TS:   const value = data ?? "默认值";
来源：http://ya.szsharing.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yj.521024.cn

Go:   if data == "" { data = "默认值" }
来源：http://vr.bjjhwx.cn

Ruby: value = data || "默认值"
来源：http://vq.hnjuh.cn

C#:   var value = data ?? "默认值";
来源：http://kc.hnjuh.cn

[A16] 真假值判断规则
来源：http://fr.hnjuh.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wi.hnjuh.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://la.521024.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tb.jctech888.com.cn

TS:   if (!x) {}
来源：http://jy.haigaiapp.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fl.hnjuh.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yw.shtwfgs.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lw.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ng.chemitech.net.cn

[A17] 位运算
来源：http://gt.szsharing.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rw.nicolike.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://or.chemitech.net.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cx.huanxung.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://se.jctech888.com.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pj.nszjky.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vb.panjiajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xd.gzmigu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cu.chemitech.net.cn

[A18] 字符与 ASCII 码互转
来源：http://ny.bookmarksfly.cn

Py:   ord("A"); chr(65)
来源：http://sc.szsharing.cn

PHP:  ord("A"); chr(65)
来源：http://tx.bookmarksfly.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mt.shxzskj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oy.yuexingan06.cn

Java: (int) 'A'; (char) 65
来源：http://xl.shtwfgs.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://il.hahajie.cn

Ruby: "A".ord; 65.chr
来源：http://tl.szxytkj.cn

C#:   (int)'A'; (char)65
来源：http://bt.nicolike.cn

[A19] 交换两个变量
来源：http://nz.bookmarksfly.cn

Py:   a, b = b, a
来源：http://xa.chemitech.net.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://aq.gzmigu.cn

JS:   [a, b] = [b, a];
来源：http://rw.yuntaijiaju.cn

TS:   [a, b] = [b, a];
来源：http://yc.shxzskj.cn

Java: int t = a; a = b; b = t;
来源：http://zz.521024.cn

Go:   a, b = b, a
来源：http://uz.gzmigu.cn

Ruby: a, b = b, a
来源：http://lt.shxzskj.cn

C#:   (a, b) = (b, a);
来源：http://so.521024.cn

[A20] 读取标准输入
来源：http://vg.shxzskj.cn

Py:   name = input("请输入：")
来源：http://re.wgjwhj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://xk.shxzukj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lr.colortex.cn

TS:   // Node.js：readline 模块
来源：http://os.yuexingan06.cn

Java: new Scanner(System.in).nextLine()
来源：http://uu.yuntaijiaju.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://px.521024.cn

Ruby: gets.chomp
来源：http://nz.wgjwhj.cn

C#:   Console.ReadLine();
来源：http://hp.huixiangedu.cn

[A21] 保留指定小数位输出
来源：http://ie.9csxet.cn

Py:   f"{3.14159:.2f}"
来源：http://zi.chemitech.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yf.shtwfgs.cn

JS:   (3.14159).toFixed(2)
来源：http://qi.asd995.cn

TS:   (3.14159).toFixed(2)
来源：http://mb.shxzukj.cn

Java: String.format("%.2f", 3.14159)
来源：http://xx.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ih.yuntaijiaju.cn

Ruby: format("%.2f", 3.14159)
来源：http://hz.chemitech.net.cn

C#:   3.14159.ToString("F2")
来源：http://py.huixinmuqiang.cn

[A22] 获取字符串长度
来源：http://tc.shxzskj.cn

Py:   len(s)
来源：http://fi.huixiangedu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cw.bjjhwx.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cp.bookmarksfly.cn

TS:   s.length
来源：http://gp.9csxet.cn

Java: s.length()
来源：http://mx.chemitech.net.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cq.nszjky.cn

Ruby: s.length
来源：http://ip.yuntaijiaju.cn

C#:   s.Length
来源：http://fw.521024.cn

[A23] 大小写转换
来源：http://cp.bookmarksfly.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://in.hnjuh.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ie.nicolike.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.huixinmuqiang.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hr.panjiajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gd.nicolike.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mm.newstarts.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://at.asd995.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jh.panjiajie.cn

[A24] 去除首尾空白
来源：http://bf.hnjuh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kw.lnxyls.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vm.panjiajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dr.nicolike.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ie.521024.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hr.newstarts.cn

Go:   strings.TrimSpace(s)
来源：http://wi.chemitech.net.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://os.wgjwhj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yj.9csxet.cn

[A25] 字符串比较
来源：http://dk.shxzskj.cn

Py:   s1 == s2; s1 != s2
来源：http://hu.szxytkj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vn.nszjky.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ai.521024.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://az.shxzukj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fz.gzmigu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://il.hnjuh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wi.muxihuayi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fv.lnxyls.cn

[A26] 类型转换总览
来源：http://we.jianghongdianzi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zd.huanxung.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ls.gzmigu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kd.colortex.cn

TS:   Number() String() Boolean() x as number
来源：http://aw.bjjhwx.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jx.bookmarksfly.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rv.yuexingan06.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zp.bjjhwx.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pw.huixinmuqiang.cn

================================================================================
来源：http://ol.521024.cn

B. 流程控制
来源：http://dy.colortex.cn

================================================================================
来源：http://pw.yuexingan06.cn

[B01] 条件判断 if / else
来源：http://mr.huixiangedu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jb.shxzskj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rt.hahajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vp.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ux.szxytkj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://kj.9csxet.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ls.shtwfgs.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ck.szxytkj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ln.wgjwhj.cn

[B02] 多分支 else if / elif
来源：http://zu.lnxyls.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wt.jctech888.com.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ri.muxihuayi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cg.szxytkj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ch.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oz.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bs.bookmarksfly.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://no.hahajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wc.gzmigu.cn

[B03] switch / match / case
来源：http://iv.hnjuh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qr.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uh.yuexingan06.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gp.shxzukj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ac.huanxung.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://og.szsharing.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pb.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kz.colortex.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zb.huixiangedu.cn

[B04] for 计数循环
来源：http://aj.9csxet.cn

Py:   for i in range(10): print(i)
来源：http://ve.gzmigu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mx.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lb.gzmigu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rx.shxzskj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ha.bjjhwx.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kn.hahajie.cn

Ruby: 10.times { |i| puts i }
来源：http://ut.shtwfgs.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cp.hahajie.cn

[B05] 遍历数组 / 列表
来源：http://wg.9csxet.cn

Py:   for item in arr: print(item)
来源：http://wv.jianghongdianzi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mo.hahajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://pm.yuexingan06.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gd.gzmigu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rm.haigaiapp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kz.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://oc.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dw.jianghongdianzi.cn

[B06] 遍历字典 / 对象
来源：http://gq.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cj.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wa.shxzukj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pl.shxzukj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yt.hnjuh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uo.chemitech.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ng.bjjhwx.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yh.panjiajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://az.wgjwhj.cn

[B07] while 循环
来源：http://ud.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://xd.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tn.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://nu.nicolike.cn

TS:   while (i < 10) { i++; }
来源：http://ha.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://ay.nszjky.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tj.wgjwhj.cn

Ruby: while i < 10; i += 1; end
来源：http://qr.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://fl.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://yk.hahajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://iw.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ar.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://rs.hnjuh.cn

TS:   do { i++; } while (i < 10);
来源：http://st.muxihuayi.cn

Java: do { i++; } while (i < 10);
来源：http://sc.yuntaijiaju.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://eq.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mm.wgjwhj.cn

C#:   do { i++; } while (i < 10);
来源：http://jd.muxihuayi.cn

[B09] break 与 continue
来源：http://ml.9csxet.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nu.nszjky.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ol.huixinmuqiang.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wo.szsharing.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cu.bookmarksfly.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eo.szxytkj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qa.bjjhwx.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xo.9csxet.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ff.chemitech.net.cn

[B10] 遍历同时拿索引
来源：http://tr.bjjhwx.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ev.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ma.bjjhwx.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nv.bjjhwx.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mq.panjiajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ip.newstarts.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://eb.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://if.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://di.shxzskj.cn

[B11] 生成数字序列 / 区间
来源：http://qc.gzmigu.cn

Py:   list(range(0, 10, 2))
来源：http://oq.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://ni.bjjhwx.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ub.gzmigu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vn.nszjky.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pf.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ip.hnjuh.cn

Ruby: (0...10).step(2).to_a
来源：http://wd.521024.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gc.newstarts.cn

[B12] 跳出多层循环
来源：http://lg.jianghongdianzi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wk.lnxyls.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vb.colortex.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oo.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zq.521024.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wy.shxzskj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sh.wgjwhj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yo.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zv.szsharing.cn

[B13] 判断是否为数字
来源：http://vx.9csxet.cn

Py:   isinstance(x, (int, float))
来源：http://fm.nicolike.cn

PHP:  is_numeric($x)
来源：http://vx.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pk.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fu.521024.cn

Java: x instanceof Number
来源：http://xq.huixiangedu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fy.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://su.bjjhwx.cn

C#:   x is int or double or decimal
来源：http://xi.lnxyls.cn

[B14] 判断值是否在集合内
来源：http://kt.szxytkj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ci.huixinmuqiang.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://du.chemitech.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://md.hahajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://yu.colortex.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fk.huixinmuqiang.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fb.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wk.szsharing.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qs.colortex.cn

[B15] 布尔运算与取反
来源：http://pc.hahajie.cn

Py:   a and b or not c
来源：http://dk.huanxung.cn

PHP:  $a && $b || !$c
来源：http://rx.huixiangedu.cn

JS:   a && b || !c
来源：http://tr.szxytkj.cn

TS:   a && b || !c
来源：http://iw.jianghongdianzi.cn

Java: a && b || !c
来源：http://jc.lnxyls.cn

Go:   a && b || !c
来源：http://ty.bjjhwx.cn

Ruby: a && b || !c
来源：http://ag.bjjhwx.cn

C#:   a && b || !c
来源：http://nb.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nu.lnxyls.cn

Py:   if not data: return
来源：http://fq.panjiajie.cn

PHP:  if (!$data) { return; }
来源：http://ie.colortex.cn

JS:   if (!data) return;
来源：http://lb.shxzskj.cn

TS:   if (!data) return;
来源：http://ai.shxzukj.cn

Java: if (data == null) return;
来源：http://ow.chemitech.net.cn

Go:   if data == nil { return }
来源：http://ug.haigaiapp.cn

Ruby: return if data.nil?
来源：http://lq.szxytkj.cn

C#:   if (data == null) return;
来源：http://np.521024.cn

================================================================================
来源：http://mu.huanxung.cn

C. 函数与作用域
来源：http://pt.lnxyls.cn

================================================================================
来源：http://vh.wgjwhj.cn

[C01] 定义函数
来源：http://nl.chemitech.net.cn

Py:   def add(a, b): return a + b
来源：http://kw.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qz.lnxyls.cn

JS:   function add(a, b) { return a + b; }
来源：http://vb.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xz.muxihuayi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pn.nszjky.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gv.521024.cn

Ruby: def add(a, b); a + b; end
来源：http://fe.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nj.yuntaijiaju.cn

[C02] 默认参数
来源：http://vn.chemitech.net.cn

Py:   def greet(name="World"): return name
来源：http://eq.colortex.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://de.szsharing.cn

JS:   function greet(name = "World") { return name; }
来源：http://jl.muxihuayi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ey.bookmarksfly.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kz.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qz.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://jf.yuntaijiaju.cn

C#:   string Greet(string name = "World") => name;
来源：http://xj.huixiangedu.cn

[C03] 可变参数
来源：http://zv.muxihuayi.cn

Py:   def total(*args): return sum(args)
来源：http://bo.9csxet.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tz.521024.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ud.lnxyls.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://su.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ie.huixiangedu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lx.jctech888.com.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rh.gzmigu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ug.shxzukj.cn

[C04] 命名参数 / 关键字参数
来源：http://dk.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sg.nszjky.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rm.szxytkj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xd.yuexingan06.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xc.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://ya.panjiajie.cn

Go:   // 无：用配置结构体参数
来源：http://je.yuntaijiaju.cn

Ruby: f(a: 1, b: 2)
来源：http://pq.panjiajie.cn

C#:   f(a: 1, b: 2)
来源：http://yk.yuntaijiaju.cn

[C05] 返回多个值
来源：http://xk.shxzskj.cn

Py:   return a, b
来源：http://il.huixiangedu.cn

PHP:  return [$a, $b];
来源：http://bm.newstarts.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ge.bookmarksfly.cn

TS:   return { a, b };
来源：http://iu.hahajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lv.haigaiapp.cn

Go:   return a, b
来源：http://un.jianghongdianzi.cn

Ruby: return a, b
来源：http://yx.asd995.cn

C#:   return (a, b);              // ValueTuple
来源：http://tu.gzmigu.cn


<!-- 参考信息 -->