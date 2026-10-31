代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cl.bookmarksfly.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fr.nicolike.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zc.shxzskj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xf.shtwfgs.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mq.nszjky.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://il.lnxyls.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ro.shxzskj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rm.wgjwhj.cn

[A18] 字符与 ASCII 码互转
来源：http://wb.huixiangedu.cn

Py:   ord("A"); chr(65)
来源：http://hl.newstarts.cn

PHP:  ord("A"); chr(65)
来源：http://ft.nszjky.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ro.gzmigu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kt.szxytkj.cn

Java: (int) 'A'; (char) 65
来源：http://jp.huixiangedu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vi.muxihuayi.cn

Ruby: "A".ord; 65.chr
来源：http://zd.szxytkj.cn

C#:   (int)'A'; (char)65
来源：http://pg.asd995.cn

[A19] 交换两个变量
来源：http://pl.bjjhwx.cn

Py:   a, b = b, a
来源：http://ry.muxihuayi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://gv.9csxet.cn

JS:   [a, b] = [b, a];
来源：http://lv.huanxung.cn

TS:   [a, b] = [b, a];
来源：http://oq.panjiajie.cn

Java: int t = a; a = b; b = t;
来源：http://fy.hahajie.cn

Go:   a, b = b, a
来源：http://ru.colortex.cn

Ruby: a, b = b, a
来源：http://px.szsharing.cn

C#:   (a, b) = (b, a);
来源：http://fq.chemitech.net.cn

[A20] 读取标准输入
来源：http://zc.asd995.cn

Py:   name = input("请输入：")
来源：http://kx.hnjuh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://jn.newstarts.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fy.9csxet.cn

TS:   // Node.js：readline 模块
来源：http://vj.haigaiapp.cn

Java: new Scanner(System.in).nextLine()
来源：http://si.newstarts.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ej.jianghongdianzi.cn

Ruby: gets.chomp
来源：http://bd.szsharing.cn

C#:   Console.ReadLine();
来源：http://jr.asd995.cn

[A21] 保留指定小数位输出
来源：http://vj.nicolike.cn

Py:   f"{3.14159:.2f}"
来源：http://ns.huixiangedu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gh.szxytkj.cn

JS:   (3.14159).toFixed(2)
来源：http://ed.muxihuayi.cn

TS:   (3.14159).toFixed(2)
来源：http://et.szsharing.cn

Java: String.format("%.2f", 3.14159)
来源：http://gr.newstarts.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xs.jianghongdianzi.cn

Ruby: format("%.2f", 3.14159)
来源：http://wt.9csxet.cn

C#:   3.14159.ToString("F2")
来源：http://ri.nicolike.cn

[A22] 获取字符串长度
来源：http://hj.haigaiapp.cn

Py:   len(s)
来源：http://xt.muxihuayi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nb.shxzukj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gg.colortex.cn

TS:   s.length
来源：http://fm.huixiangedu.cn

Java: s.length()
来源：http://gl.muxihuayi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nv.bjjhwx.cn

Ruby: s.length
来源：http://jg.9csxet.cn

C#:   s.Length
来源：http://mr.muxihuayi.cn

[A23] 大小写转换
来源：http://mh.huanxung.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://sb.yuntaijiaju.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://db.haigaiapp.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rt.jctech888.com.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://un.panjiajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yb.asd995.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cs.wgjwhj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zt.haigaiapp.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://db.yuexingan06.cn

[A24] 去除首尾空白
来源：http://gr.521024.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://uh.shxzskj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wi.nicolike.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gc.huanxung.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qx.huanxung.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fo.huixiangedu.cn

Go:   strings.TrimSpace(s)
来源：http://bj.haigaiapp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xh.yuexingan06.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tv.huixiangedu.cn

[A25] 字符串比较
来源：http://po.hnjuh.cn

Py:   s1 == s2; s1 != s2
来源：http://di.chemitech.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qz.newstarts.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bs.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ph.shxzskj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hi.hnjuh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kq.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qm.nszjky.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cq.shxzskj.cn

[A26] 类型转换总览
来源：http://sm.wgjwhj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bu.wgjwhj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mq.521024.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zr.yuexingan06.cn

TS:   Number() String() Boolean() x as number
来源：http://db.nicolike.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zg.nszjky.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xc.szsharing.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vh.bookmarksfly.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qk.jctech888.com.cn

================================================================================
来源：http://hx.colortex.cn

B. 流程控制
来源：http://pn.asd995.cn

================================================================================
来源：http://jb.huixiangedu.cn

[B01] 条件判断 if / else
来源：http://ey.bookmarksfly.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lg.shtwfgs.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bo.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ck.huixinmuqiang.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://og.lnxyls.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ee.chemitech.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nf.521024.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ah.521024.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xm.9csxet.cn

[B02] 多分支 else if / elif
来源：http://lu.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bb.jianghongdianzi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vj.huanxung.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ic.jianghongdianzi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ws.szsharing.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xa.wgjwhj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nb.jianghongdianzi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://el.lnxyls.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://it.huixinmuqiang.cn

[B03] switch / match / case
来源：http://pq.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wq.nicolike.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pl.wgjwhj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qz.yuntaijiaju.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ol.shxzskj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ac.wgjwhj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uk.9csxet.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xd.newstarts.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wj.szsharing.cn

[B04] for 计数循环
来源：http://qi.chemitech.net.cn

Py:   for i in range(10): print(i)
来源：http://iw.bookmarksfly.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ye.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hn.gzmigu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jb.jctech888.com.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wo.wgjwhj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lr.huanxung.cn

Ruby: 10.times { |i| puts i }
来源：http://ox.haigaiapp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dz.521024.cn

[B05] 遍历数组 / 列表
来源：http://qr.huanxung.cn

Py:   for item in arr: print(item)
来源：http://ek.asd995.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bq.huixinmuqiang.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vq.szxytkj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dg.nicolike.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sw.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ju.bookmarksfly.cn

Ruby: arr.each { |item| puts item }
来源：http://sv.jctech888.com.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ku.colortex.cn

[B06] 遍历字典 / 对象
来源：http://cd.jctech888.com.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qo.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wf.jctech888.com.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oi.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ak.colortex.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://db.huanxung.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ow.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jv.lnxyls.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qw.wgjwhj.cn

[B07] while 循环
来源：http://zq.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://cx.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rz.panjiajie.cn

JS:   while (i < 10) { i++; }
来源：http://mk.lnxyls.cn

TS:   while (i < 10) { i++; }
来源：http://ej.muxihuayi.cn

Java: while (i < 10) { i++; }
来源：http://tk.szxytkj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nw.newstarts.cn

Ruby: while i < 10; i += 1; end
来源：http://dn.nszjky.cn

C#:   while (i < 10) { i++; }
来源：http://bg.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://xd.nszjky.cn

Py:   # 无 do-while：用 while True + break
来源：http://it.nszjky.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xn.chemitech.net.cn

JS:   do { i++; } while (i < 10);
来源：http://dj.asd995.cn

TS:   do { i++; } while (i < 10);
来源：http://to.hahajie.cn

Java: do { i++; } while (i < 10);
来源：http://gk.szsharing.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://um.muxihuayi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://st.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://ac.hnjuh.cn

[B09] break 与 continue
来源：http://ed.chemitech.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hn.newstarts.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vh.gzmigu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://il.jianghongdianzi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pn.chemitech.net.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pc.chemitech.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xw.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mg.huanxung.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://io.hnjuh.cn

[B10] 遍历同时拿索引
来源：http://xm.nszjky.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vo.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hd.muxihuayi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://np.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kn.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fs.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wh.nicolike.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://df.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mj.huixinmuqiang.cn

[B11] 生成数字序列 / 区间
来源：http://ok.haigaiapp.cn

Py:   list(range(0, 10, 2))
来源：http://su.jctech888.com.cn

PHP:  range(0, 10, 2);
来源：http://sk.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lf.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cn.yuntaijiaju.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tr.szsharing.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xw.colortex.cn

Ruby: (0...10).step(2).to_a
来源：http://bg.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ls.newstarts.cn

[B12] 跳出多层循环
来源：http://ys.colortex.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tl.muxihuayi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://in.nicolike.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wy.yuntaijiaju.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://oq.hnjuh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hj.bookmarksfly.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ew.521024.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cf.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://as.hahajie.cn

[B13] 判断是否为数字
来源：http://zo.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://fr.gzmigu.cn

PHP:  is_numeric($x)
来源：http://su.panjiajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xi.haigaiapp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cf.yuntaijiaju.cn

Java: x instanceof Number
来源：http://pt.haigaiapp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bo.chemitech.net.cn

Ruby: x.is_a?(Numeric)
来源：http://gb.9csxet.cn

C#:   x is int or double or decimal
来源：http://ao.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://fn.jianghongdianzi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tw.muxihuayi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mo.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://fm.asd995.cn

TS:   [1, 2, 3].includes(x)
来源：http://cu.huanxung.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ep.shtwfgs.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rg.huixiangedu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tr.szsharing.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ue.chemitech.net.cn

[B15] 布尔运算与取反
来源：http://ck.wgjwhj.cn

Py:   a and b or not c
来源：http://st.szxytkj.cn

PHP:  $a && $b || !$c
来源：http://ly.shtwfgs.cn

JS:   a && b || !c
来源：http://nc.huixinmuqiang.cn

TS:   a && b || !c
来源：http://do.haigaiapp.cn

Java: a && b || !c
来源：http://no.yuntaijiaju.cn

Go:   a && b || !c
来源：http://zp.asd995.cn

Ruby: a && b || !c
来源：http://hx.shtwfgs.cn

C#:   a && b || !c
来源：http://mv.colortex.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dj.yuexingan06.cn

Py:   if not data: return
来源：http://dt.colortex.cn

PHP:  if (!$data) { return; }
来源：http://em.muxihuayi.cn

JS:   if (!data) return;
来源：http://uw.colortex.cn

TS:   if (!data) return;
来源：http://nm.nszjky.cn

Java: if (data == null) return;
来源：http://sc.huixinmuqiang.cn

Go:   if data == nil { return }
来源：http://lq.muxihuayi.cn

Ruby: return if data.nil?
来源：http://fs.gzmigu.cn

C#:   if (data == null) return;
来源：http://dj.newstarts.cn

================================================================================
来源：http://xs.hahajie.cn

C. 函数与作用域
来源：http://hx.hnjuh.cn

================================================================================
来源：http://cb.shtwfgs.cn

[C01] 定义函数
来源：http://vn.hahajie.cn

Py:   def add(a, b): return a + b
来源：http://rh.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qs.huanxung.cn

JS:   function add(a, b) { return a + b; }
来源：http://qs.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vz.nszjky.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jo.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ac.lnxyls.cn

Ruby: def add(a, b); a + b; end
来源：http://dp.huixiangedu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tt.haigaiapp.cn

[C02] 默认参数
来源：http://pf.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://zh.szxytkj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://uf.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://nt.lnxyls.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vh.colortex.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ko.lnxyls.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qk.hahajie.cn

Ruby: def greet(name = "World") = name
来源：http://jz.huanxung.cn

C#:   string Greet(string name = "World") => name;
来源：http://ir.szxytkj.cn

[C03] 可变参数
来源：http://tm.jianghongdianzi.cn

Py:   def total(*args): return sum(args)
来源：http://fj.huixiangedu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pf.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pb.9csxet.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ay.panjiajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ux.lnxyls.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://np.szsharing.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hr.lnxyls.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ye.gzmigu.cn

[C04] 命名参数 / 关键字参数
来源：http://yp.huanxung.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tc.huixinmuqiang.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dh.521024.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zj.hahajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yd.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://jy.jianghongdianzi.cn

Go:   // 无：用配置结构体参数
来源：http://im.wgjwhj.cn

Ruby: f(a: 1, b: 2)
来源：http://td.huanxung.cn

C#:   f(a: 1, b: 2)
来源：http://og.panjiajie.cn

[C05] 返回多个值
来源：http://lz.szxytkj.cn

Py:   return a, b
来源：http://ev.jctech888.com.cn

PHP:  return [$a, $b];
来源：http://ft.shxzskj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kb.521024.cn

TS:   return { a, b };
来源：http://bt.bjjhwx.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://el.shxzskj.cn

Go:   return a, b
来源：http://dk.jctech888.com.cn

Ruby: return a, b
来源：http://eo.asd995.cn

C#:   return (a, b);              // ValueTuple
来源：http://jb.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://jc.shxzskj.cn

Py:   square = lambda x: x * x
来源：http://os.gzmigu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rj.huixiangedu.cn

JS:   const square = x => x * x;
来源：http://sh.jctech888.com.cn

TS:   const square = (x: number): number => x * x;
来源：http://ho.shtwfgs.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ln.gzmigu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lx.huixiangedu.cn

Ruby: square = ->(x) { x * x }
来源：http://ft.muxihuayi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fu.yuexingan06.cn

[C07] 把函数作为参数传入
来源：http://qy.hnjuh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ny.bookmarksfly.cn

PHP:  array_map("strtoupper", $arr);
来源：http://no.colortex.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mp.asd995.cn

TS:   arr.map(String)
来源：http://se.panjiajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fm.bjjhwx.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zj.lnxyls.cn


<!-- 参考信息 -->