代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nu.jctech888.com.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xo.szsharing.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ib.jctech888.com.cn

[A17] 位运算
来源：http://ks.hnjuh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sg.muxihuayi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://su.huanxung.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fi.colortex.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://or.gzmigu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sj.huanxung.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://er.nicolike.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xw.gzmigu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bs.huixinmuqiang.cn

[A18] 字符与 ASCII 码互转
来源：http://dj.jctech888.com.cn

Py:   ord("A"); chr(65)
来源：http://ff.szsharing.cn

PHP:  ord("A"); chr(65)
来源：http://wd.yuntaijiaju.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vz.yuntaijiaju.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gr.colortex.cn

Java: (int) 'A'; (char) 65
来源：http://eg.chemitech.net.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wi.chemitech.net.cn

Ruby: "A".ord; 65.chr
来源：http://zi.lnxyls.cn

C#:   (int)'A'; (char)65
来源：http://nd.shxzukj.cn

[A19] 交换两个变量
来源：http://xv.gzmigu.cn

Py:   a, b = b, a
来源：http://jl.yuexingan06.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ou.shtwfgs.cn

JS:   [a, b] = [b, a];
来源：http://ps.szxytkj.cn

TS:   [a, b] = [b, a];
来源：http://qn.bookmarksfly.cn

Java: int t = a; a = b; b = t;
来源：http://gw.haigaiapp.cn

Go:   a, b = b, a
来源：http://va.shtwfgs.cn

Ruby: a, b = b, a
来源：http://wq.shxzukj.cn

C#:   (a, b) = (b, a);
来源：http://xg.shtwfgs.cn

[A20] 读取标准输入
来源：http://hg.szsharing.cn

Py:   name = input("请输入：")
来源：http://fi.huixiangedu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://pq.szxytkj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fb.gzmigu.cn

TS:   // Node.js：readline 模块
来源：http://ux.panjiajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://bz.hnjuh.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ub.huixinmuqiang.cn

Ruby: gets.chomp
来源：http://db.nicolike.cn

C#:   Console.ReadLine();
来源：http://ux.yuexingan06.cn

[A21] 保留指定小数位输出
来源：http://hf.muxihuayi.cn

Py:   f"{3.14159:.2f}"
来源：http://ai.panjiajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zq.wgjwhj.cn

JS:   (3.14159).toFixed(2)
来源：http://fk.nszjky.cn

TS:   (3.14159).toFixed(2)
来源：http://uv.chemitech.net.cn

Java: String.format("%.2f", 3.14159)
来源：http://zd.521024.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://oe.haigaiapp.cn

Ruby: format("%.2f", 3.14159)
来源：http://gh.shxzskj.cn

C#:   3.14159.ToString("F2")
来源：http://wg.jianghongdianzi.cn

[A22] 获取字符串长度
来源：http://lj.colortex.cn

Py:   len(s)
来源：http://bw.szxytkj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xc.szxytkj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tp.huixinmuqiang.cn

TS:   s.length
来源：http://mt.chemitech.net.cn

Java: s.length()
来源：http://vn.chemitech.net.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ch.colortex.cn

Ruby: s.length
来源：http://ql.shxzukj.cn

C#:   s.Length
来源：http://lw.colortex.cn

[A23] 大小写转换
来源：http://aq.521024.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hf.hnjuh.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lx.yuexingan06.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ca.panjiajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://du.nszjky.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mk.szsharing.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ed.hahajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cm.szxytkj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://iv.nicolike.cn

[A24] 去除首尾空白
来源：http://nn.shxzukj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://av.newstarts.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zo.lnxyls.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nz.hnjuh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ap.nszjky.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://iu.lnxyls.cn

Go:   strings.TrimSpace(s)
来源：http://ft.muxihuayi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ui.huixiangedu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ym.wgjwhj.cn

[A25] 字符串比较
来源：http://ql.szxytkj.cn

Py:   s1 == s2; s1 != s2
来源：http://eq.hnjuh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gv.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ne.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rc.szsharing.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tw.nicolike.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hm.nicolike.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hm.haigaiapp.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lz.panjiajie.cn

[A26] 类型转换总览
来源：http://yj.shtwfgs.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fk.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ge.chemitech.net.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rz.wgjwhj.cn

TS:   Number() String() Boolean() x as number
来源：http://me.haigaiapp.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gl.asd995.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vu.lnxyls.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mz.colortex.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zz.nicolike.cn

================================================================================
来源：http://fv.hnjuh.cn

B. 流程控制
来源：http://mf.chemitech.net.cn

================================================================================
来源：http://rt.hahajie.cn

[B01] 条件判断 if / else
来源：http://ai.jianghongdianzi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jk.szsharing.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sh.shxzskj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dn.haigaiapp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ys.szxytkj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tw.huixinmuqiang.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nq.szsharing.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fa.nszjky.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jj.newstarts.cn

[B02] 多分支 else if / elif
来源：http://vi.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://an.521024.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zl.colortex.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://js.newstarts.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hd.shtwfgs.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ym.bookmarksfly.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yq.521024.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://em.panjiajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://op.jctech888.com.cn

[B03] switch / match / case
来源：http://hm.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ae.lnxyls.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uv.gzmigu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nq.chemitech.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yr.bookmarksfly.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lu.huixiangedu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jv.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wc.shxzskj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ei.hnjuh.cn

[B04] for 计数循环
来源：http://zf.shtwfgs.cn

Py:   for i in range(10): print(i)
来源：http://bw.jctech888.com.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fi.bjjhwx.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ar.haigaiapp.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sf.wgjwhj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jk.bjjhwx.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wi.huixinmuqiang.cn

Ruby: 10.times { |i| puts i }
来源：http://ub.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tt.jianghongdianzi.cn

[B05] 遍历数组 / 列表
来源：http://dq.yuntaijiaju.cn

Py:   for item in arr: print(item)
来源：http://fq.bookmarksfly.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ky.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ix.panjiajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xf.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fx.haigaiapp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ed.chemitech.net.cn

Ruby: arr.each { |item| puts item }
来源：http://pn.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jn.shtwfgs.cn

[B06] 遍历字典 / 对象
来源：http://aw.jctech888.com.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://so.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ri.muxihuayi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oa.gzmigu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hq.bookmarksfly.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dy.hnjuh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ir.szxytkj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kd.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pe.szxytkj.cn

[B07] while 循环
来源：http://lr.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://uk.asd995.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nb.nicolike.cn

JS:   while (i < 10) { i++; }
来源：http://dx.521024.cn

TS:   while (i < 10) { i++; }
来源：http://cc.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://wh.szxytkj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ok.huixinmuqiang.cn

Ruby: while i < 10; i += 1; end
来源：http://pl.521024.cn

C#:   while (i < 10) { i++; }
来源：http://es.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://fa.521024.cn

Py:   # 无 do-while：用 while True + break
来源：http://jm.nszjky.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rj.newstarts.cn

JS:   do { i++; } while (i < 10);
来源：http://cy.bjjhwx.cn

TS:   do { i++; } while (i < 10);
来源：http://sb.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://at.nicolike.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pk.bookmarksfly.cn

Ruby: begin; i += 1; end while i < 10
来源：http://we.shxzskj.cn

C#:   do { i++; } while (i < 10);
来源：http://yo.521024.cn

[B09] break 与 continue
来源：http://cz.yuntaijiaju.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yk.nicolike.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qx.shtwfgs.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kh.bookmarksfly.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ly.521024.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tr.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kb.yuexingan06.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yo.wgjwhj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ut.panjiajie.cn

[B10] 遍历同时拿索引
来源：http://te.yuntaijiaju.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bj.szxytkj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zu.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yz.muxihuayi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cx.shtwfgs.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ym.521024.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jd.9csxet.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tj.nicolike.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uk.521024.cn

[B11] 生成数字序列 / 区间
来源：http://mo.nicolike.cn

Py:   list(range(0, 10, 2))
来源：http://my.szsharing.cn

PHP:  range(0, 10, 2);
来源：http://mb.521024.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xu.colortex.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yv.colortex.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yn.gzmigu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cp.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://sx.bjjhwx.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xq.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://kh.newstarts.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wt.asd995.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mz.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bz.wgjwhj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gw.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bl.muxihuayi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gc.haigaiapp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ci.jctech888.com.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uq.huixiangedu.cn

[B13] 判断是否为数字
来源：http://vs.jianghongdianzi.cn

Py:   isinstance(x, (int, float))
来源：http://lj.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://dq.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sv.bookmarksfly.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lu.huixinmuqiang.cn

Java: x instanceof Number
来源：http://jf.yuexingan06.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wj.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://gp.asd995.cn

C#:   x is int or double or decimal
来源：http://wg.chemitech.net.cn

[B14] 判断值是否在集合内
来源：http://hw.bookmarksfly.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vc.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ue.bookmarksfly.cn

JS:   [1, 2, 3].includes(x)
来源：http://dt.shxzukj.cn

TS:   [1, 2, 3].includes(x)
来源：http://en.shtwfgs.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wr.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ri.shtwfgs.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ay.szsharing.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vz.szxytkj.cn

[B15] 布尔运算与取反
来源：http://pi.chemitech.net.cn

Py:   a and b or not c
来源：http://ae.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://jz.bookmarksfly.cn

JS:   a && b || !c
来源：http://yg.asd995.cn

TS:   a && b || !c
来源：http://ro.huixinmuqiang.cn

Java: a && b || !c
来源：http://js.haigaiapp.cn

Go:   a && b || !c
来源：http://ho.muxihuayi.cn

Ruby: a && b || !c
来源：http://tb.jianghongdianzi.cn

C#:   a && b || !c
来源：http://ux.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ut.9csxet.cn

Py:   if not data: return
来源：http://sn.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://lb.jctech888.com.cn

JS:   if (!data) return;
来源：http://co.hnjuh.cn

TS:   if (!data) return;
来源：http://kx.newstarts.cn

Java: if (data == null) return;
来源：http://ez.9csxet.cn

Go:   if data == nil { return }
来源：http://xs.yuexingan06.cn

Ruby: return if data.nil?
来源：http://om.bjjhwx.cn

C#:   if (data == null) return;
来源：http://zr.jianghongdianzi.cn

================================================================================
来源：http://uu.9csxet.cn

C. 函数与作用域
来源：http://oe.9csxet.cn

================================================================================
来源：http://qq.haigaiapp.cn

[C01] 定义函数
来源：http://ln.shxzukj.cn

Py:   def add(a, b): return a + b
来源：http://ar.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bd.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://tf.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mp.bookmarksfly.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sk.hahajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cq.jctech888.com.cn

Ruby: def add(a, b); a + b; end
来源：http://yp.colortex.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dk.hahajie.cn

[C02] 默认参数
来源：http://rm.yuexingan06.cn

Py:   def greet(name="World"): return name
来源：http://pq.huanxung.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://px.9csxet.cn

JS:   function greet(name = "World") { return name; }
来源：http://ec.jctech888.com.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xc.newstarts.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xh.yuntaijiaju.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pi.muxihuayi.cn

Ruby: def greet(name = "World") = name
来源：http://xb.shxzukj.cn

C#:   string Greet(string name = "World") => name;
来源：http://se.shxzskj.cn

[C03] 可变参数
来源：http://xt.hnjuh.cn

Py:   def total(*args): return sum(args)
来源：http://uw.nicolike.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ag.chemitech.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rz.huixinmuqiang.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wx.shtwfgs.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gc.huixinmuqiang.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://of.wgjwhj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://sb.9csxet.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fs.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://fh.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cq.asd995.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vx.chemitech.net.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zp.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qg.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://ki.szxytkj.cn

Go:   // 无：用配置结构体参数
来源：http://ik.bookmarksfly.cn

Ruby: f(a: 1, b: 2)
来源：http://po.huanxung.cn

C#:   f(a: 1, b: 2)
来源：http://ic.521024.cn

[C05] 返回多个值
来源：http://fj.521024.cn

Py:   return a, b
来源：http://us.hahajie.cn

PHP:  return [$a, $b];
来源：http://br.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kt.szsharing.cn

TS:   return { a, b };
来源：http://ji.huanxung.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xg.huixiangedu.cn

Go:   return a, b
来源：http://up.shxzukj.cn

Ruby: return a, b
来源：http://qg.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://ow.shtwfgs.cn

[C06] 匿名函数 / lambda
来源：http://uk.shxzukj.cn

Py:   square = lambda x: x * x
来源：http://fu.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ia.gzmigu.cn

JS:   const square = x => x * x;
来源：http://kp.szsharing.cn

TS:   const square = (x: number): number => x * x;
来源：http://ou.jctech888.com.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gv.huixinmuqiang.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yq.jctech888.com.cn

Ruby: square = ->(x) { x * x }
来源：http://xx.hnjuh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xv.nszjky.cn

[C07] 把函数作为参数传入
来源：http://tn.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qt.lnxyls.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jz.gzmigu.cn


<!-- 参考信息 -->