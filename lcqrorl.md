代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gn.szsharing.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mb.nicolike.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rq.521024.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://im.huanxung.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bv.shxzskj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jn.yuntaijiaju.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mo.yuexingan06.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fo.gzmigu.cn

[A18] 字符与 ASCII 码互转
来源：http://uy.jctech888.com.cn

Py:   ord("A"); chr(65)
来源：http://ee.nicolike.cn

PHP:  ord("A"); chr(65)
来源：http://bo.szxytkj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fx.lnxyls.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://el.muxihuayi.cn

Java: (int) 'A'; (char) 65
来源：http://vr.szsharing.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fk.huixinmuqiang.cn

Ruby: "A".ord; 65.chr
来源：http://jh.newstarts.cn

C#:   (int)'A'; (char)65
来源：http://fg.gzmigu.cn

[A19] 交换两个变量
来源：http://qa.muxihuayi.cn

Py:   a, b = b, a
来源：http://ji.panjiajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://nr.bookmarksfly.cn

JS:   [a, b] = [b, a];
来源：http://jn.gzmigu.cn

TS:   [a, b] = [b, a];
来源：http://lq.yuexingan06.cn

Java: int t = a; a = b; b = t;
来源：http://ox.bjjhwx.cn

Go:   a, b = b, a
来源：http://vj.haigaiapp.cn

Ruby: a, b = b, a
来源：http://bb.muxihuayi.cn

C#:   (a, b) = (b, a);
来源：http://vy.lnxyls.cn

[A20] 读取标准输入
来源：http://ro.bjjhwx.cn

Py:   name = input("请输入：")
来源：http://rh.shxzukj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://tc.nszjky.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ro.chemitech.net.cn

TS:   // Node.js：readline 模块
来源：http://vl.huixinmuqiang.cn

Java: new Scanner(System.in).nextLine()
来源：http://ot.jianghongdianzi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ym.bookmarksfly.cn

Ruby: gets.chomp
来源：http://dq.newstarts.cn

C#:   Console.ReadLine();
来源：http://zt.haigaiapp.cn

[A21] 保留指定小数位输出
来源：http://lf.jctech888.com.cn

Py:   f"{3.14159:.2f}"
来源：http://fp.asd995.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ez.huanxung.cn

JS:   (3.14159).toFixed(2)
来源：http://uh.521024.cn

TS:   (3.14159).toFixed(2)
来源：http://gp.huixinmuqiang.cn

Java: String.format("%.2f", 3.14159)
来源：http://iy.szxytkj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xu.chemitech.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://eg.colortex.cn

C#:   3.14159.ToString("F2")
来源：http://fv.521024.cn

[A22] 获取字符串长度
来源：http://tq.yuntaijiaju.cn

Py:   len(s)
来源：http://mt.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vj.jianghongdianzi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pr.newstarts.cn

TS:   s.length
来源：http://zo.nicolike.cn

Java: s.length()
来源：http://ry.gzmigu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dq.hnjuh.cn

Ruby: s.length
来源：http://fs.nicolike.cn

C#:   s.Length
来源：http://aw.huanxung.cn

[A23] 大小写转换
来源：http://rk.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ou.szsharing.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://re.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lh.chemitech.net.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lm.huixiangedu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zr.muxihuayi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ak.haigaiapp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://eo.bjjhwx.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://de.shxzskj.cn

[A24] 去除首尾空白
来源：http://gx.nicolike.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ti.shxzukj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dg.huixinmuqiang.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zv.hnjuh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ph.haigaiapp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tx.yuexingan06.cn

Go:   strings.TrimSpace(s)
来源：http://jg.yuexingan06.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kt.gzmigu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ah.bjjhwx.cn

[A25] 字符串比较
来源：http://ra.newstarts.cn

Py:   s1 == s2; s1 != s2
来源：http://da.shxzukj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bf.jctech888.com.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wa.newstarts.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zp.nicolike.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tn.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://be.huanxung.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bs.chemitech.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wr.gzmigu.cn

[A26] 类型转换总览
来源：http://nq.9csxet.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yx.colortex.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uj.shxzukj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://iw.gzmigu.cn

TS:   Number() String() Boolean() x as number
来源：http://so.shxzskj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bq.shtwfgs.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lf.muxihuayi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://py.lnxyls.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zj.shxzukj.cn

================================================================================
来源：http://po.shtwfgs.cn

B. 流程控制
来源：http://ox.newstarts.cn

================================================================================
来源：http://gc.muxihuayi.cn

[B01] 条件判断 if / else
来源：http://ro.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zh.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yq.panjiajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nt.panjiajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ob.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ld.shxzukj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fv.hahajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pj.huixinmuqiang.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://so.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://gh.muxihuayi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xu.newstarts.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fx.huanxung.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://el.nicolike.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lk.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iu.gzmigu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hb.huixinmuqiang.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vz.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bs.szxytkj.cn

[B03] switch / match / case
来源：http://sv.bjjhwx.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ym.asd995.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jo.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ep.muxihuayi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xw.bjjhwx.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kc.colortex.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://se.asd995.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://av.hnjuh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nu.nicolike.cn

[B04] for 计数循环
来源：http://hg.521024.cn

Py:   for i in range(10): print(i)
来源：http://rv.chemitech.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fo.hahajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zq.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xn.9csxet.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cj.chemitech.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oq.huanxung.cn

Ruby: 10.times { |i| puts i }
来源：http://oo.wgjwhj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pu.jctech888.com.cn

[B05] 遍历数组 / 列表
来源：http://dj.gzmigu.cn

Py:   for item in arr: print(item)
来源：http://gm.yuexingan06.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bu.9csxet.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jh.newstarts.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pa.newstarts.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vl.huixiangedu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://te.wgjwhj.cn

Ruby: arr.each { |item| puts item }
来源：http://si.bookmarksfly.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ct.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://qf.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fn.bookmarksfly.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hs.szxytkj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ar.newstarts.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rx.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fz.huixinmuqiang.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://db.yuexingan06.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uh.panjiajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tp.gzmigu.cn

[B07] while 循环
来源：http://kz.jianghongdianzi.cn

Py:   while i < 10: i += 1
来源：http://ua.szsharing.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wk.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://vi.szxytkj.cn

TS:   while (i < 10) { i++; }
来源：http://uo.9csxet.cn

Java: while (i < 10) { i++; }
来源：http://ul.lnxyls.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://eu.newstarts.cn

Ruby: while i < 10; i += 1; end
来源：http://ov.asd995.cn

C#:   while (i < 10) { i++; }
来源：http://jh.huixiangedu.cn

[B08] do-while（至少执行一次）
来源：http://vh.colortex.cn

Py:   # 无 do-while：用 while True + break
来源：http://zy.panjiajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://td.huixinmuqiang.cn

JS:   do { i++; } while (i < 10);
来源：http://bw.521024.cn

TS:   do { i++; } while (i < 10);
来源：http://yl.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://ba.521024.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ka.szsharing.cn

Ruby: begin; i += 1; end while i < 10
来源：http://na.yuntaijiaju.cn

C#:   do { i++; } while (i < 10);
来源：http://ul.haigaiapp.cn

[B09] break 与 continue
来源：http://qa.szxytkj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ai.newstarts.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://iw.huanxung.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ur.haigaiapp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mm.chemitech.net.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://to.asd995.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://du.hahajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sm.newstarts.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lw.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://vn.nicolike.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ud.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jx.nszjky.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ft.bjjhwx.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xv.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rm.hahajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://se.szsharing.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ps.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tf.hahajie.cn

[B11] 生成数字序列 / 区间
来源：http://gt.shxzskj.cn

Py:   list(range(0, 10, 2))
来源：http://jw.colortex.cn

PHP:  range(0, 10, 2);
来源：http://bn.panjiajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://et.newstarts.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zv.huixinmuqiang.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ui.szsharing.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qk.huanxung.cn

Ruby: (0...10).step(2).to_a
来源：http://bf.nszjky.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yy.huanxung.cn

[B12] 跳出多层循环
来源：http://gn.bjjhwx.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mv.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ud.huixiangedu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://is.muxihuayi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://oa.9csxet.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ok.521024.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wx.shxzskj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vn.521024.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ra.wgjwhj.cn

[B13] 判断是否为数字
来源：http://yk.szsharing.cn

Py:   isinstance(x, (int, float))
来源：http://ou.colortex.cn

PHP:  is_numeric($x)
来源：http://tw.szxytkj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uj.jctech888.com.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rs.hahajie.cn

Java: x instanceof Number
来源：http://uc.muxihuayi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ka.szxytkj.cn

Ruby: x.is_a?(Numeric)
来源：http://yk.newstarts.cn

C#:   x is int or double or decimal
来源：http://fn.huixinmuqiang.cn

[B14] 判断值是否在集合内
来源：http://bj.lnxyls.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wp.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dv.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://by.panjiajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://ey.jctech888.com.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ok.shtwfgs.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xb.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fj.shtwfgs.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yx.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://it.huanxung.cn

Py:   a and b or not c
来源：http://qw.huixinmuqiang.cn

PHP:  $a && $b || !$c
来源：http://wh.huixinmuqiang.cn

JS:   a && b || !c
来源：http://iu.9csxet.cn

TS:   a && b || !c
来源：http://ix.hahajie.cn

Java: a && b || !c
来源：http://ef.nszjky.cn

Go:   a && b || !c
来源：http://un.9csxet.cn

Ruby: a && b || !c
来源：http://km.bookmarksfly.cn

C#:   a && b || !c
来源：http://fp.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://en.521024.cn

Py:   if not data: return
来源：http://eb.bjjhwx.cn

PHP:  if (!$data) { return; }
来源：http://mv.haigaiapp.cn

JS:   if (!data) return;
来源：http://si.hnjuh.cn

TS:   if (!data) return;
来源：http://js.colortex.cn

Java: if (data == null) return;
来源：http://gf.szxytkj.cn

Go:   if data == nil { return }
来源：http://tl.gzmigu.cn

Ruby: return if data.nil?
来源：http://ey.newstarts.cn

C#:   if (data == null) return;
来源：http://le.9csxet.cn

================================================================================
来源：http://ss.colortex.cn

C. 函数与作用域
来源：http://jd.chemitech.net.cn

================================================================================
来源：http://fo.huixinmuqiang.cn

[C01] 定义函数
来源：http://hm.colortex.cn

Py:   def add(a, b): return a + b
来源：http://jd.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wc.jianghongdianzi.cn

JS:   function add(a, b) { return a + b; }
来源：http://lx.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ga.hnjuh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ac.gzmigu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ez.panjiajie.cn

Ruby: def add(a, b); a + b; end
来源：http://ss.huixinmuqiang.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://re.haigaiapp.cn

[C02] 默认参数
来源：http://yz.jianghongdianzi.cn

Py:   def greet(name="World"): return name
来源：http://sl.nszjky.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vq.hahajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://cn.wgjwhj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fk.lnxyls.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sp.colortex.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ou.chemitech.net.cn

Ruby: def greet(name = "World") = name
来源：http://bh.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://tx.chemitech.net.cn

[C03] 可变参数
来源：http://xs.wgjwhj.cn

Py:   def total(*args): return sum(args)
来源：http://xk.9csxet.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ih.huixinmuqiang.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ou.bookmarksfly.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pw.haigaiapp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hh.hnjuh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hq.chemitech.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://sf.shxzskj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fw.newstarts.cn

[C04] 命名参数 / 关键字参数
来源：http://cn.9csxet.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://by.hnjuh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dc.shxzukj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gg.jianghongdianzi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bb.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://vq.colortex.cn

Go:   // 无：用配置结构体参数
来源：http://au.wgjwhj.cn

Ruby: f(a: 1, b: 2)
来源：http://oz.asd995.cn

C#:   f(a: 1, b: 2)
来源：http://ya.lnxyls.cn

[C05] 返回多个值
来源：http://hp.hnjuh.cn

Py:   return a, b
来源：http://ua.szxytkj.cn

PHP:  return [$a, $b];
来源：http://yx.bjjhwx.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yv.gzmigu.cn

TS:   return { a, b };
来源：http://gr.chemitech.net.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ez.hahajie.cn

Go:   return a, b
来源：http://fz.nicolike.cn

Ruby: return a, b
来源：http://lh.shxzukj.cn

C#:   return (a, b);              // ValueTuple
来源：http://ac.lnxyls.cn

[C06] 匿名函数 / lambda
来源：http://xl.huanxung.cn

Py:   square = lambda x: x * x
来源：http://ni.panjiajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pl.9csxet.cn

JS:   const square = x => x * x;
来源：http://qh.bjjhwx.cn

TS:   const square = (x: number): number => x * x;
来源：http://gt.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mb.yuntaijiaju.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kw.jianghongdianzi.cn

Ruby: square = ->(x) { x * x }
来源：http://ib.nszjky.cn

C#:   Func<int, int> square = x => x * x;
来源：http://or.wgjwhj.cn

[C07] 把函数作为参数传入
来源：http://us.newstarts.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://at.hahajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lz.muxihuayi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pd.haigaiapp.cn

TS:   arr.map(String)
来源：http://qz.9csxet.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zn.bookmarksfly.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ux.colortex.cn


<!-- 参考信息 -->