代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dx.521024.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hq.huixiangedu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ki.yuexingan06.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ox.szsharing.cn

[A18] 字符与 ASCII 码互转
来源：http://sq.haigaiapp.cn

Py:   ord("A"); chr(65)
来源：http://fw.nicolike.cn

PHP:  ord("A"); chr(65)
来源：http://uu.szxytkj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nm.huixinmuqiang.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nj.yuntaijiaju.cn

Java: (int) 'A'; (char) 65
来源：http://xe.huanxung.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pm.nicolike.cn

Ruby: "A".ord; 65.chr
来源：http://gq.huanxung.cn

C#:   (int)'A'; (char)65
来源：http://wg.huanxung.cn

[A19] 交换两个变量
来源：http://xh.huixiangedu.cn

Py:   a, b = b, a
来源：http://ic.nszjky.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://cs.chemitech.net.cn

JS:   [a, b] = [b, a];
来源：http://zn.yuexingan06.cn

TS:   [a, b] = [b, a];
来源：http://ag.shxzukj.cn

Java: int t = a; a = b; b = t;
来源：http://yp.yuexingan06.cn

Go:   a, b = b, a
来源：http://tn.newstarts.cn

Ruby: a, b = b, a
来源：http://qz.wgjwhj.cn

C#:   (a, b) = (b, a);
来源：http://ql.newstarts.cn

[A20] 读取标准输入
来源：http://co.wgjwhj.cn

Py:   name = input("请输入：")
来源：http://sd.yuntaijiaju.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://pg.wgjwhj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://og.nszjky.cn

TS:   // Node.js：readline 模块
来源：http://pi.bookmarksfly.cn

Java: new Scanner(System.in).nextLine()
来源：http://mt.szsharing.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pq.gzmigu.cn

Ruby: gets.chomp
来源：http://qt.newstarts.cn

C#:   Console.ReadLine();
来源：http://lf.hahajie.cn

[A21] 保留指定小数位输出
来源：http://rc.shxzskj.cn

Py:   f"{3.14159:.2f}"
来源：http://nm.szsharing.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://al.bookmarksfly.cn

JS:   (3.14159).toFixed(2)
来源：http://yy.yuexingan06.cn

TS:   (3.14159).toFixed(2)
来源：http://wo.szsharing.cn

Java: String.format("%.2f", 3.14159)
来源：http://iq.newstarts.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wj.yuntaijiaju.cn

Ruby: format("%.2f", 3.14159)
来源：http://rt.panjiajie.cn

C#:   3.14159.ToString("F2")
来源：http://be.asd995.cn

[A22] 获取字符串长度
来源：http://jd.muxihuayi.cn

Py:   len(s)
来源：http://yl.shtwfgs.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cx.szxytkj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ug.521024.cn

TS:   s.length
来源：http://kz.shxzukj.cn

Java: s.length()
来源：http://zy.lnxyls.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dw.521024.cn

Ruby: s.length
来源：http://ut.wgjwhj.cn

C#:   s.Length
来源：http://cm.muxihuayi.cn

[A23] 大小写转换
来源：http://qx.haigaiapp.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wv.yuntaijiaju.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cb.jianghongdianzi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ha.huixiangedu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qb.bookmarksfly.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xt.huixiangedu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ho.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yg.bjjhwx.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wd.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://aj.newstarts.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tm.wgjwhj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kh.hahajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lk.hnjuh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nj.yuexingan06.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rb.bookmarksfly.cn

Go:   strings.TrimSpace(s)
来源：http://hb.shxzukj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mz.jianghongdianzi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tv.szxytkj.cn

[A25] 字符串比较
来源：http://tl.yuntaijiaju.cn

Py:   s1 == s2; s1 != s2
来源：http://es.chemitech.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yh.haigaiapp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ol.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ox.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xa.521024.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qo.bjjhwx.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rl.shtwfgs.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dv.wgjwhj.cn

[A26] 类型转换总览
来源：http://ho.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yv.chemitech.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ev.asd995.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wa.yuexingan06.cn

TS:   Number() String() Boolean() x as number
来源：http://cf.szsharing.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hh.nszjky.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gr.panjiajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pa.wgjwhj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jo.shxzukj.cn

================================================================================
来源：http://yn.shxzskj.cn

B. 流程控制
来源：http://dd.jctech888.com.cn

================================================================================
来源：http://uj.lnxyls.cn

[B01] 条件判断 if / else
来源：http://ze.yuntaijiaju.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nt.szsharing.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://st.wgjwhj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vq.huixinmuqiang.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ui.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zb.hahajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yq.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gk.huixiangedu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gs.hnjuh.cn

[B02] 多分支 else if / elif
来源：http://hx.szsharing.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qp.huixinmuqiang.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gj.9csxet.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gc.nicolike.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cu.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://as.hahajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gt.huixinmuqiang.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ry.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ma.szxytkj.cn

[B03] switch / match / case
来源：http://bj.huanxung.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://up.panjiajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qk.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cn.hnjuh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nk.colortex.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zl.szxytkj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zt.yuexingan06.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bn.hnjuh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yh.shxzukj.cn

[B04] for 计数循环
来源：http://kg.lnxyls.cn

Py:   for i in range(10): print(i)
来源：http://ip.wgjwhj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nc.nszjky.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://md.szxytkj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ws.nszjky.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oo.521024.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ol.haigaiapp.cn

Ruby: 10.times { |i| puts i }
来源：http://ku.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://or.jctech888.com.cn

[B05] 遍历数组 / 列表
来源：http://hf.hnjuh.cn

Py:   for item in arr: print(item)
来源：http://ec.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dd.hnjuh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mi.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tt.haigaiapp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ta.bjjhwx.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tg.nszjky.cn

Ruby: arr.each { |item| puts item }
来源：http://gs.bookmarksfly.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pl.huixiangedu.cn

[B06] 遍历字典 / 对象
来源：http://cv.9csxet.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qr.newstarts.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ua.shtwfgs.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sc.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iy.nszjky.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zb.muxihuayi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wi.haigaiapp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fz.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://da.chemitech.net.cn

[B07] while 循环
来源：http://cg.szsharing.cn

Py:   while i < 10: i += 1
来源：http://uk.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wz.szsharing.cn

JS:   while (i < 10) { i++; }
来源：http://ol.bjjhwx.cn

TS:   while (i < 10) { i++; }
来源：http://uk.hahajie.cn

Java: while (i < 10) { i++; }
来源：http://it.haigaiapp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://va.szxytkj.cn

Ruby: while i < 10; i += 1; end
来源：http://ar.panjiajie.cn

C#:   while (i < 10) { i++; }
来源：http://ik.shxzukj.cn

[B08] do-while（至少执行一次）
来源：http://yf.huanxung.cn

Py:   # 无 do-while：用 while True + break
来源：http://hj.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wg.szxytkj.cn

JS:   do { i++; } while (i < 10);
来源：http://ji.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://js.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://xf.shxzskj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cg.shxzskj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://by.newstarts.cn

C#:   do { i++; } while (i < 10);
来源：http://fn.colortex.cn

[B09] break 与 continue
来源：http://di.newstarts.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lr.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ml.huanxung.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uo.szxytkj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pw.shxzukj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bd.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ky.yuexingan06.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://at.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jctech888.com.cn

[B10] 遍历同时拿索引
来源：http://ah.shxzskj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wy.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://on.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://la.521024.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ev.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kk.nicolike.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zr.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bn.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ck.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://gr.bjjhwx.cn

Py:   list(range(0, 10, 2))
来源：http://zh.wgjwhj.cn

PHP:  range(0, 10, 2);
来源：http://so.gzmigu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://li.hnjuh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pf.521024.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ds.jctech888.com.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jd.wgjwhj.cn

Ruby: (0...10).step(2).to_a
来源：http://bm.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cg.nszjky.cn

[B12] 跳出多层循环
来源：http://no.lnxyls.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nj.huixinmuqiang.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ee.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lc.nicolike.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jf.9csxet.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yd.shtwfgs.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ob.shtwfgs.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uf.haigaiapp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://if.huixiangedu.cn

[B13] 判断是否为数字
来源：http://ah.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://bn.nicolike.cn

PHP:  is_numeric($x)
来源：http://au.huixiangedu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oq.jianghongdianzi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uh.asd995.cn

Java: x instanceof Number
来源：http://jz.nszjky.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uv.shxzskj.cn

Ruby: x.is_a?(Numeric)
来源：http://wv.hnjuh.cn

C#:   x is int or double or decimal
来源：http://rj.jctech888.com.cn

[B14] 判断值是否在集合内
来源：http://rr.shxzukj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gb.haigaiapp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qw.panjiajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://mw.jctech888.com.cn

TS:   [1, 2, 3].includes(x)
来源：http://ff.jianghongdianzi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ii.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nk.hahajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rp.szxytkj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kb.szsharing.cn

[B15] 布尔运算与取反
来源：http://og.nszjky.cn

Py:   a and b or not c
来源：http://zv.hahajie.cn

PHP:  $a && $b || !$c
来源：http://wz.bookmarksfly.cn

JS:   a && b || !c
来源：http://ii.huanxung.cn

TS:   a && b || !c
来源：http://wu.panjiajie.cn

Java: a && b || !c
来源：http://ep.jctech888.com.cn

Go:   a && b || !c
来源：http://jx.yuntaijiaju.cn

Ruby: a && b || !c
来源：http://oh.yuexingan06.cn

C#:   a && b || !c
来源：http://xt.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ze.huixinmuqiang.cn

Py:   if not data: return
来源：http://uq.asd995.cn

PHP:  if (!$data) { return; }
来源：http://ke.jctech888.com.cn

JS:   if (!data) return;
来源：http://yw.bookmarksfly.cn

TS:   if (!data) return;
来源：http://bx.shxzskj.cn

Java: if (data == null) return;
来源：http://vr.huixiangedu.cn

Go:   if data == nil { return }
来源：http://fb.bjjhwx.cn

Ruby: return if data.nil?
来源：http://iw.hahajie.cn

C#:   if (data == null) return;
来源：http://jw.huanxung.cn

================================================================================
来源：http://pg.hahajie.cn

C. 函数与作用域
来源：http://jb.hnjuh.cn

================================================================================
来源：http://at.huixinmuqiang.cn

[C01] 定义函数
来源：http://ce.hahajie.cn

Py:   def add(a, b): return a + b
来源：http://ya.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://th.wgjwhj.cn

JS:   function add(a, b) { return a + b; }
来源：http://lr.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hl.chemitech.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hp.bjjhwx.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hl.huanxung.cn

Ruby: def add(a, b); a + b; end
来源：http://sb.shxzukj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yh.jianghongdianzi.cn

[C02] 默认参数
来源：http://vh.haigaiapp.cn

Py:   def greet(name="World"): return name
来源：http://gr.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bj.lnxyls.cn

JS:   function greet(name = "World") { return name; }
来源：http://sg.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xb.hnjuh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cy.shxzukj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yd.bjjhwx.cn

Ruby: def greet(name = "World") = name
来源：http://mz.hahajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://vy.nszjky.cn

[C03] 可变参数
来源：http://vj.hahajie.cn

Py:   def total(*args): return sum(args)
来源：http://cg.wgjwhj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zr.colortex.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yr.9csxet.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ir.nszjky.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cg.haigaiapp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sn.521024.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ze.lnxyls.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://he.hahajie.cn

[C04] 命名参数 / 关键字参数
来源：http://qz.huanxung.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vk.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cd.hahajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rt.521024.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://od.asd995.cn

Java: // 无：用 Builder 模式或 record
来源：http://da.haigaiapp.cn

Go:   // 无：用配置结构体参数
来源：http://sw.muxihuayi.cn

Ruby: f(a: 1, b: 2)
来源：http://ol.bjjhwx.cn

C#:   f(a: 1, b: 2)
来源：http://sk.shtwfgs.cn

[C05] 返回多个值
来源：http://jq.shxzukj.cn

Py:   return a, b
来源：http://eb.nicolike.cn

PHP:  return [$a, $b];
来源：http://yj.shtwfgs.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hi.haigaiapp.cn

TS:   return { a, b };
来源：http://vj.szxytkj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ys.9csxet.cn

Go:   return a, b
来源：http://rf.nszjky.cn

Ruby: return a, b
来源：http://es.huixinmuqiang.cn

C#:   return (a, b);              // ValueTuple
来源：http://gc.nszjky.cn

[C06] 匿名函数 / lambda
来源：http://rw.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://en.521024.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://my.newstarts.cn

JS:   const square = x => x * x;
来源：http://iz.9csxet.cn

TS:   const square = (x: number): number => x * x;
来源：http://vo.lnxyls.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ym.jctech888.com.cn

Go:   sq := func(x int) int { return x * x }
来源：http://po.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://iz.asd995.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hd.jianghongdianzi.cn

[C07] 把函数作为参数传入
来源：http://gy.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://og.huanxung.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ov.bookmarksfly.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qu.lnxyls.cn

TS:   arr.map(String)
来源：http://af.nicolike.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tp.gzmigu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kf.shtwfgs.cn

Ruby: arr.map(&:upcase)
来源：http://dr.huixiangedu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fy.yuntaijiaju.cn

[C08] 闭包
来源：http://xq.colortex.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rx.chemitech.net.cn


<!-- 参考信息 -->