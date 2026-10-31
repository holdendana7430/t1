代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ip.asd995.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xx.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cb.bookmarksfly.cn

[A17] 位运算
来源：http://bq.shxzskj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://my.muxihuayi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mc.hnjuh.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xs.nicolike.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vn.haigaiapp.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qf.huanxung.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ec.colortex.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://us.hnjuh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ut.nicolike.cn

[A18] 字符与 ASCII 码互转
来源：http://qc.huixiangedu.cn

Py:   ord("A"); chr(65)
来源：http://fp.shtwfgs.cn

PHP:  ord("A"); chr(65)
来源：http://vi.szsharing.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kv.asd995.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wr.hahajie.cn

Java: (int) 'A'; (char) 65
来源：http://xq.jianghongdianzi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rq.szxytkj.cn

Ruby: "A".ord; 65.chr
来源：http://gj.yuntaijiaju.cn

C#:   (int)'A'; (char)65
来源：http://mf.haigaiapp.cn

[A19] 交换两个变量
来源：http://dk.muxihuayi.cn

Py:   a, b = b, a
来源：http://at.nicolike.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yw.gzmigu.cn

JS:   [a, b] = [b, a];
来源：http://wb.yuntaijiaju.cn

TS:   [a, b] = [b, a];
来源：http://sh.nszjky.cn

Java: int t = a; a = b; b = t;
来源：http://xa.wgjwhj.cn

Go:   a, b = b, a
来源：http://tg.asd995.cn

Ruby: a, b = b, a
来源：http://ge.jianghongdianzi.cn

C#:   (a, b) = (b, a);
来源：http://tq.521024.cn

[A20] 读取标准输入
来源：http://tp.shxzskj.cn

Py:   name = input("请输入：")
来源：http://ud.lnxyls.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ik.szsharing.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hf.huanxung.cn

TS:   // Node.js：readline 模块
来源：http://cb.wgjwhj.cn

Java: new Scanner(System.in).nextLine()
来源：http://hf.huanxung.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ka.wgjwhj.cn

Ruby: gets.chomp
来源：http://bk.newstarts.cn

C#:   Console.ReadLine();
来源：http://sg.huixiangedu.cn

[A21] 保留指定小数位输出
来源：http://wu.bjjhwx.cn

Py:   f"{3.14159:.2f}"
来源：http://jn.gzmigu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lj.jctech888.com.cn

JS:   (3.14159).toFixed(2)
来源：http://nb.newstarts.cn

TS:   (3.14159).toFixed(2)
来源：http://lt.jianghongdianzi.cn

Java: String.format("%.2f", 3.14159)
来源：http://is.shtwfgs.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vi.huixinmuqiang.cn

Ruby: format("%.2f", 3.14159)
来源：http://cx.muxihuayi.cn

C#:   3.14159.ToString("F2")
来源：http://rp.gzmigu.cn

[A22] 获取字符串长度
来源：http://cl.huanxung.cn

Py:   len(s)
来源：http://wh.jctech888.com.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://np.hnjuh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wj.bookmarksfly.cn

TS:   s.length
来源：http://ha.yuntaijiaju.cn

Java: s.length()
来源：http://he.panjiajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ak.asd995.cn

Ruby: s.length
来源：http://hf.jctech888.com.cn

C#:   s.Length
来源：http://xk.lnxyls.cn

[A23] 大小写转换
来源：http://cy.bjjhwx.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hp.bookmarksfly.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xf.shxzukj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qw.bjjhwx.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sw.9csxet.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kr.wgjwhj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yn.hahajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://oo.newstarts.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vd.lnxyls.cn

[A24] 去除首尾空白
来源：http://ec.shxzskj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bd.asd995.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fh.huanxung.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uk.chemitech.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lb.newstarts.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xy.hahajie.cn

Go:   strings.TrimSpace(s)
来源：http://gx.hahajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zc.521024.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xu.colortex.cn

[A25] 字符串比较
来源：http://xs.asd995.cn

Py:   s1 == s2; s1 != s2
来源：http://rg.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vm.jianghongdianzi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dk.521024.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rt.newstarts.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zx.bookmarksfly.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ug.panjiajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vu.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tq.muxihuayi.cn

[A26] 类型转换总览
来源：http://dl.colortex.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://me.yuexingan06.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cb.gzmigu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vi.gzmigu.cn

TS:   Number() String() Boolean() x as number
来源：http://dj.colortex.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cw.yuntaijiaju.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ih.panjiajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mn.yuexingan06.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wh.huixinmuqiang.cn

================================================================================
来源：http://ft.newstarts.cn

B. 流程控制
来源：http://dk.szxytkj.cn

================================================================================
来源：http://ib.hnjuh.cn

[B01] 条件判断 if / else
来源：http://zk.shxzskj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cq.gzmigu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zo.yuntaijiaju.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fh.shxzskj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xp.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sq.shxzskj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wf.jianghongdianzi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cc.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sw.haigaiapp.cn

[B02] 多分支 else if / elif
来源：http://el.shxzukj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zy.bjjhwx.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://aq.9csxet.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wv.newstarts.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pp.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://to.shtwfgs.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lt.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fq.panjiajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xi.muxihuayi.cn

[B03] switch / match / case
来源：http://mq.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nm.nicolike.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tf.panjiajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://so.9csxet.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rc.jianghongdianzi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tr.colortex.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vw.huanxung.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mo.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mz.nicolike.cn

[B04] for 计数循环
来源：http://km.nicolike.cn

Py:   for i in range(10): print(i)
来源：http://eu.huanxung.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uf.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mu.huixinmuqiang.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ek.521024.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://iw.shxzukj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cq.jctech888.com.cn

Ruby: 10.times { |i| puts i }
来源：http://mk.wgjwhj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ur.hnjuh.cn

[B05] 遍历数组 / 列表
来源：http://gd.lnxyls.cn

Py:   for item in arr: print(item)
来源：http://qn.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wx.hahajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qg.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://md.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hk.wgjwhj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pl.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://an.colortex.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jy.panjiajie.cn

[B06] 遍历字典 / 对象
来源：http://ad.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sd.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ji.huixiangedu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qp.bjjhwx.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ip.yuntaijiaju.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mx.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://iq.chemitech.net.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://te.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nc.yuexingan06.cn

[B07] while 循环
来源：http://ck.haigaiapp.cn

Py:   while i < 10: i += 1
来源：http://kz.huixiangedu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ld.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://fi.shtwfgs.cn

TS:   while (i < 10) { i++; }
来源：http://gs.chemitech.net.cn

Java: while (i < 10) { i++; }
来源：http://qp.shxzukj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zc.yuntaijiaju.cn

Ruby: while i < 10; i += 1; end
来源：http://su.huixinmuqiang.cn

C#:   while (i < 10) { i++; }
来源：http://eo.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://ov.shxzukj.cn

Py:   # 无 do-while：用 while True + break
来源：http://pe.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zc.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://cv.nszjky.cn

TS:   do { i++; } while (i < 10);
来源：http://nw.9csxet.cn

Java: do { i++; } while (i < 10);
来源：http://eo.asd995.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sr.haigaiapp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xt.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://xb.huixiangedu.cn

[B09] break 与 continue
来源：http://zp.hnjuh.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://oq.shtwfgs.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xu.colortex.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xu.hnjuh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gb.szsharing.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://au.szsharing.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rl.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kq.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vo.szxytkj.cn

[B10] 遍历同时拿索引
来源：http://sr.lnxyls.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fl.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pt.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xh.hnjuh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pq.bjjhwx.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rb.bjjhwx.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://av.jctech888.com.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://em.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bq.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://wm.jianghongdianzi.cn

Py:   list(range(0, 10, 2))
来源：http://kh.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://ea.huixiangedu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tc.yuntaijiaju.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ji.shxzskj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qm.shxzukj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wf.shtwfgs.cn

Ruby: (0...10).step(2).to_a
来源：http://gv.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ys.shxzskj.cn

[B12] 跳出多层循环
来源：http://lk.bookmarksfly.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fm.lnxyls.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yw.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jg.yuexingan06.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://py.huanxung.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wy.huixiangedu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bb.jctech888.com.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dq.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vr.colortex.cn

[B13] 判断是否为数字
来源：http://tm.wgjwhj.cn

Py:   isinstance(x, (int, float))
来源：http://vs.szxytkj.cn

PHP:  is_numeric($x)
来源：http://sg.haigaiapp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eh.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gb.muxihuayi.cn

Java: x instanceof Number
来源：http://sv.colortex.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tq.muxihuayi.cn

Ruby: x.is_a?(Numeric)
来源：http://ha.szsharing.cn

C#:   x is int or double or decimal
来源：http://tn.shxzskj.cn

[B14] 判断值是否在集合内
来源：http://qj.huanxung.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dp.panjiajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ti.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://hd.huixinmuqiang.cn

TS:   [1, 2, 3].includes(x)
来源：http://zv.szxytkj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ny.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gj.haigaiapp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ub.chemitech.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tn.huixiangedu.cn

[B15] 布尔运算与取反
来源：http://sd.gzmigu.cn

Py:   a and b or not c
来源：http://ml.yuexingan06.cn

PHP:  $a && $b || !$c
来源：http://oy.jianghongdianzi.cn

JS:   a && b || !c
来源：http://qu.jctech888.com.cn

TS:   a && b || !c
来源：http://yr.colortex.cn

Java: a && b || !c
来源：http://mt.shtwfgs.cn

Go:   a && b || !c
来源：http://qc.chemitech.net.cn

Ruby: a && b || !c
来源：http://ij.shxzskj.cn

C#:   a && b || !c
来源：http://mc.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yl.newstarts.cn

Py:   if not data: return
来源：http://zv.hnjuh.cn

PHP:  if (!$data) { return; }
来源：http://xm.huixinmuqiang.cn

JS:   if (!data) return;
来源：http://nq.jctech888.com.cn

TS:   if (!data) return;
来源：http://uy.jianghongdianzi.cn

Java: if (data == null) return;
来源：http://sg.colortex.cn

Go:   if data == nil { return }
来源：http://bl.yuntaijiaju.cn

Ruby: return if data.nil?
来源：http://ei.bjjhwx.cn

C#:   if (data == null) return;
来源：http://qi.szxytkj.cn

================================================================================
来源：http://bt.bjjhwx.cn

C. 函数与作用域
来源：http://bn.shxzukj.cn

================================================================================
来源：http://vv.shxzskj.cn

[C01] 定义函数
来源：http://mu.asd995.cn

Py:   def add(a, b): return a + b
来源：http://gi.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ql.colortex.cn

JS:   function add(a, b) { return a + b; }
来源：http://xe.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ns.bookmarksfly.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gw.haigaiapp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bo.haigaiapp.cn

Ruby: def add(a, b); a + b; end
来源：http://pl.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ah.shtwfgs.cn

[C02] 默认参数
来源：http://nx.panjiajie.cn

Py:   def greet(name="World"): return name
来源：http://uq.jianghongdianzi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yq.wgjwhj.cn

JS:   function greet(name = "World") { return name; }
来源：http://ci.lnxyls.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yf.asd995.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zc.newstarts.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ya.hnjuh.cn

Ruby: def greet(name = "World") = name
来源：http://nr.hahajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://rb.muxihuayi.cn

[C03] 可变参数
来源：http://ge.huixiangedu.cn

Py:   def total(*args): return sum(args)
来源：http://mu.jctech888.com.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bd.nszjky.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mw.shxzskj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vs.haigaiapp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vu.shxzskj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fo.nszjky.cn

Ruby: def total(*nums); nums.sum; end
来源：http://at.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ea.huixiangedu.cn

[C04] 命名参数 / 关键字参数
来源：http://sq.nszjky.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://au.szxytkj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xa.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ri.szsharing.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yz.szxytkj.cn

Java: // 无：用 Builder 模式或 record
来源：http://bw.chemitech.net.cn

Go:   // 无：用配置结构体参数
来源：http://ds.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://xi.asd995.cn

C#:   f(a: 1, b: 2)
来源：http://cc.chemitech.net.cn

[C05] 返回多个值
来源：http://rp.521024.cn

Py:   return a, b
来源：http://hn.9csxet.cn

PHP:  return [$a, $b];
来源：http://ht.jianghongdianzi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wc.szxytkj.cn

TS:   return { a, b };
来源：http://iw.shtwfgs.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qv.chemitech.net.cn

Go:   return a, b
来源：http://sz.huanxung.cn

Ruby: return a, b
来源：http://oi.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://jq.shxzukj.cn

[C06] 匿名函数 / lambda
来源：http://ns.newstarts.cn

Py:   square = lambda x: x * x
来源：http://zq.huixinmuqiang.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ct.hnjuh.cn

JS:   const square = x => x * x;
来源：http://st.bjjhwx.cn

TS:   const square = (x: number): number => x * x;
来源：http://xk.521024.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://di.bjjhwx.cn

Go:   sq := func(x int) int { return x * x }
来源：http://oz.jctech888.com.cn

Ruby: square = ->(x) { x * x }
来源：http://mn.haigaiapp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hp.muxihuayi.cn

[C07] 把函数作为参数传入
来源：http://it.bjjhwx.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ov.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bp.wgjwhj.cn


<!-- 参考信息 -->