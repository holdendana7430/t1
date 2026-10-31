代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zg.colortex.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ao.szsharing.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jc.gzmigu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xk.yuntaijiaju.cn

[A18] 字符与 ASCII 码互转
来源：http://eu.huanxung.cn

Py:   ord("A"); chr(65)
来源：http://el.szsharing.cn

PHP:  ord("A"); chr(65)
来源：http://nr.bookmarksfly.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kj.9csxet.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rs.huixinmuqiang.cn

Java: (int) 'A'; (char) 65
来源：http://rx.nszjky.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wg.bjjhwx.cn

Ruby: "A".ord; 65.chr
来源：http://rr.jctech888.com.cn

C#:   (int)'A'; (char)65
来源：http://pf.jctech888.com.cn

[A19] 交换两个变量
来源：http://ar.szxytkj.cn

Py:   a, b = b, a
来源：http://ra.shtwfgs.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vq.huanxung.cn

JS:   [a, b] = [b, a];
来源：http://lj.haigaiapp.cn

TS:   [a, b] = [b, a];
来源：http://sf.jctech888.com.cn

Java: int t = a; a = b; b = t;
来源：http://sl.szsharing.cn

Go:   a, b = b, a
来源：http://nu.panjiajie.cn

Ruby: a, b = b, a
来源：http://hz.huixiangedu.cn

C#:   (a, b) = (b, a);
来源：http://pw.muxihuayi.cn

[A20] 读取标准输入
来源：http://ww.bookmarksfly.cn

Py:   name = input("请输入：")
来源：http://wr.521024.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gf.huanxung.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pc.nicolike.cn

TS:   // Node.js：readline 模块
来源：http://wv.haigaiapp.cn

Java: new Scanner(System.in).nextLine()
来源：http://hd.huanxung.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ch.muxihuayi.cn

Ruby: gets.chomp
来源：http://kp.chemitech.net.cn

C#:   Console.ReadLine();
来源：http://lp.wgjwhj.cn

[A21] 保留指定小数位输出
来源：http://on.bjjhwx.cn

Py:   f"{3.14159:.2f}"
来源：http://rs.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zh.521024.cn

JS:   (3.14159).toFixed(2)
来源：http://xe.chemitech.net.cn

TS:   (3.14159).toFixed(2)
来源：http://db.hahajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://qc.panjiajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yh.bookmarksfly.cn

Ruby: format("%.2f", 3.14159)
来源：http://pp.lnxyls.cn

C#:   3.14159.ToString("F2")
来源：http://vn.colortex.cn

[A22] 获取字符串长度
来源：http://ek.asd995.cn

Py:   len(s)
来源：http://pr.521024.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nv.huixinmuqiang.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mi.huixinmuqiang.cn

TS:   s.length
来源：http://pw.521024.cn

Java: s.length()
来源：http://rh.hahajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jq.hahajie.cn

Ruby: s.length
来源：http://de.chemitech.net.cn

C#:   s.Length
来源：http://ui.yuexingan06.cn

[A23] 大小写转换
来源：http://ht.haigaiapp.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fs.gzmigu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ch.bookmarksfly.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bo.wgjwhj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rz.szsharing.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xe.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://os.panjiajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hi.hnjuh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hu.colortex.cn

[A24] 去除首尾空白
来源：http://py.lnxyls.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cm.huixinmuqiang.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wv.lnxyls.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lu.huixiangedu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kd.colortex.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wo.shxzskj.cn

Go:   strings.TrimSpace(s)
来源：http://dy.panjiajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://is.jianghongdianzi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fo.gzmigu.cn

[A25] 字符串比较
来源：http://zd.huanxung.cn

Py:   s1 == s2; s1 != s2
来源：http://zc.hahajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wh.gzmigu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wi.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jp.shxzskj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ok.huixiangedu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://aq.bjjhwx.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mi.haigaiapp.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mu.lnxyls.cn

[A26] 类型转换总览
来源：http://ba.jctech888.com.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hk.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ya.lnxyls.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xw.9csxet.cn

TS:   Number() String() Boolean() x as number
来源：http://cn.nicolike.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ak.yuntaijiaju.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sq.panjiajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://si.haigaiapp.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ut.521024.cn

================================================================================
来源：http://yz.szxytkj.cn

B. 流程控制
来源：http://kf.shxzukj.cn

================================================================================
来源：http://gd.lnxyls.cn

[B01] 条件判断 if / else
来源：http://pa.haigaiapp.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hf.shtwfgs.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uu.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cn.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ht.szsharing.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qx.huixinmuqiang.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rs.jctech888.com.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lo.shxzukj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ry.bjjhwx.cn

[B02] 多分支 else if / elif
来源：http://me.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bm.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tu.shxzukj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jg.shxzskj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ot.bjjhwx.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fr.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mb.chemitech.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dm.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://to.muxihuayi.cn

[B03] switch / match / case
来源：http://tr.huixiangedu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dz.wgjwhj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ko.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kx.newstarts.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ge.9csxet.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dz.jianghongdianzi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nk.muxihuayi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vs.jianghongdianzi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qz.newstarts.cn

[B04] for 计数循环
来源：http://yp.lnxyls.cn

Py:   for i in range(10): print(i)
来源：http://zs.shtwfgs.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tl.panjiajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mw.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ff.jianghongdianzi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pi.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qe.chemitech.net.cn

Ruby: 10.times { |i| puts i }
来源：http://ji.gzmigu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wh.shxzskj.cn

[B05] 遍历数组 / 列表
来源：http://rq.gzmigu.cn

Py:   for item in arr: print(item)
来源：http://lg.bookmarksfly.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://oa.colortex.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zo.hnjuh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qe.wgjwhj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://uj.muxihuayi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ia.newstarts.cn

Ruby: arr.each { |item| puts item }
来源：http://it.newstarts.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sm.colortex.cn

[B06] 遍历字典 / 对象
来源：http://qi.jctech888.com.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sc.newstarts.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wk.shxzskj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xg.hnjuh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jb.bookmarksfly.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://az.newstarts.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ba.bjjhwx.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cc.bookmarksfly.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vq.shtwfgs.cn

[B07] while 循环
来源：http://cs.bookmarksfly.cn

Py:   while i < 10: i += 1
来源：http://fk.szxytkj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ie.colortex.cn

JS:   while (i < 10) { i++; }
来源：http://es.521024.cn

TS:   while (i < 10) { i++; }
来源：http://pq.jianghongdianzi.cn

Java: while (i < 10) { i++; }
来源：http://gg.shxzukj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pr.9csxet.cn

Ruby: while i < 10; i += 1; end
来源：http://rd.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://jb.nszjky.cn

[B08] do-while（至少执行一次）
来源：http://cw.nszjky.cn

Py:   # 无 do-while：用 while True + break
来源：http://ol.lnxyls.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sl.shxzukj.cn

JS:   do { i++; } while (i < 10);
来源：http://ff.newstarts.cn

TS:   do { i++; } while (i < 10);
来源：http://rp.shtwfgs.cn

Java: do { i++; } while (i < 10);
来源：http://ej.jctech888.com.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://kr.shxzskj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ad.panjiajie.cn

C#:   do { i++; } while (i < 10);
来源：http://fo.hahajie.cn

[B09] break 与 continue
来源：http://ag.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nr.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rh.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bi.huixiangedu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rc.szsharing.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tg.jianghongdianzi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cz.nszjky.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tg.hahajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nq.asd995.cn

[B10] 遍历同时拿索引
来源：http://kd.shtwfgs.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jg.nicolike.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://iu.chemitech.net.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ft.gzmigu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mb.shxzskj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yy.nicolike.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ox.bjjhwx.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fc.shtwfgs.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fi.nszjky.cn

[B11] 生成数字序列 / 区间
来源：http://tr.9csxet.cn

Py:   list(range(0, 10, 2))
来源：http://ri.shtwfgs.cn

PHP:  range(0, 10, 2);
来源：http://jo.colortex.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mg.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pe.gzmigu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://na.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xq.shtwfgs.cn

Ruby: (0...10).step(2).to_a
来源：http://ef.huanxung.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gs.panjiajie.cn

[B12] 跳出多层循环
来源：http://fd.lnxyls.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jj.szsharing.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xo.muxihuayi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hd.jianghongdianzi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zy.9csxet.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ma.nicolike.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ll.shxzskj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://la.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bj.bookmarksfly.cn

[B13] 判断是否为数字
来源：http://up.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://eb.newstarts.cn

PHP:  is_numeric($x)
来源：http://tf.newstarts.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cx.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kr.asd995.cn

Java: x instanceof Number
来源：http://hm.asd995.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gn.shtwfgs.cn

Ruby: x.is_a?(Numeric)
来源：http://pz.yuntaijiaju.cn

C#:   x is int or double or decimal
来源：http://ny.lnxyls.cn

[B14] 判断值是否在集合内
来源：http://tw.colortex.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zp.yuntaijiaju.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dt.yuexingan06.cn

JS:   [1, 2, 3].includes(x)
来源：http://xk.panjiajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://fs.jctech888.com.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gy.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wl.bookmarksfly.cn

Ruby: [1, 2, 3].include?(x)
来源：http://aa.yuntaijiaju.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mc.bookmarksfly.cn

[B15] 布尔运算与取反
来源：http://gh.szsharing.cn

Py:   a and b or not c
来源：http://ir.chemitech.net.cn

PHP:  $a && $b || !$c
来源：http://bu.bookmarksfly.cn

JS:   a && b || !c
来源：http://mq.yuexingan06.cn

TS:   a && b || !c
来源：http://gx.bookmarksfly.cn

Java: a && b || !c
来源：http://jh.lnxyls.cn

Go:   a && b || !c
来源：http://og.huixiangedu.cn

Ruby: a && b || !c
来源：http://zi.newstarts.cn

C#:   a && b || !c
来源：http://ot.yuexingan06.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bo.yuexingan06.cn

Py:   if not data: return
来源：http://ma.shtwfgs.cn

PHP:  if (!$data) { return; }
来源：http://nl.wgjwhj.cn

JS:   if (!data) return;
来源：http://ab.jianghongdianzi.cn

TS:   if (!data) return;
来源：http://gx.muxihuayi.cn

Java: if (data == null) return;
来源：http://er.szxytkj.cn

Go:   if data == nil { return }
来源：http://gu.lnxyls.cn

Ruby: return if data.nil?
来源：http://kd.huanxung.cn

C#:   if (data == null) return;
来源：http://sn.muxihuayi.cn

================================================================================
来源：http://ro.bookmarksfly.cn

C. 函数与作用域
来源：http://ms.shxzskj.cn

================================================================================
来源：http://iy.muxihuayi.cn

[C01] 定义函数
来源：http://kl.nszjky.cn

Py:   def add(a, b): return a + b
来源：http://qz.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qw.asd995.cn

JS:   function add(a, b) { return a + b; }
来源：http://bo.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vy.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ma.shxzskj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ra.haigaiapp.cn

Ruby: def add(a, b); a + b; end
来源：http://is.yuexingan06.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yl.haigaiapp.cn

[C02] 默认参数
来源：http://hx.haigaiapp.cn

Py:   def greet(name="World"): return name
来源：http://yq.hnjuh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ay.yuexingan06.cn

JS:   function greet(name = "World") { return name; }
来源：http://kr.shxzukj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yk.szxytkj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://du.bookmarksfly.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fy.shxzskj.cn

Ruby: def greet(name = "World") = name
来源：http://xt.yuexingan06.cn

C#:   string Greet(string name = "World") => name;
来源：http://ne.hahajie.cn

[C03] 可变参数
来源：http://ui.yuexingan06.cn

Py:   def total(*args): return sum(args)
来源：http://cv.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://un.hahajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qa.hnjuh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rl.jctech888.com.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nc.yuntaijiaju.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ph.haigaiapp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://id.gzmigu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ny.hnjuh.cn

[C04] 命名参数 / 关键字参数
来源：http://nf.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nu.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ot.9csxet.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tf.lnxyls.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vf.panjiajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://bm.gzmigu.cn

Go:   // 无：用配置结构体参数
来源：http://jp.asd995.cn

Ruby: f(a: 1, b: 2)
来源：http://ub.wgjwhj.cn

C#:   f(a: 1, b: 2)
来源：http://cu.hahajie.cn

[C05] 返回多个值
来源：http://li.nicolike.cn

Py:   return a, b
来源：http://ko.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://ki.huanxung.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sq.panjiajie.cn

TS:   return { a, b };
来源：http://ja.hnjuh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ms.asd995.cn

Go:   return a, b
来源：http://ed.colortex.cn

Ruby: return a, b
来源：http://wl.chemitech.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://jj.bjjhwx.cn

[C06] 匿名函数 / lambda
来源：http://yc.jctech888.com.cn

Py:   square = lambda x: x * x
来源：http://au.nszjky.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ei.nicolike.cn

JS:   const square = x => x * x;
来源：http://jf.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://cv.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://np.muxihuayi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://by.lnxyls.cn

Ruby: square = ->(x) { x * x }
来源：http://rc.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://au.gzmigu.cn

[C07] 把函数作为参数传入
来源：http://sw.asd995.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ub.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ns.shxzskj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vh.9csxet.cn

TS:   arr.map(String)
来源：http://fd.nicolike.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nz.hahajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ow.jianghongdianzi.cn

Ruby: arr.map(&:upcase)
来源：http://wt.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://nh.shtwfgs.cn

[C08] 闭包
来源：http://os.chemitech.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nx.newstarts.cn


<!-- 参考信息 -->