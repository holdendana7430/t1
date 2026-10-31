代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zp.jctech888.com.cn

Java: (int) 'A'; (char) 65
来源：http://xw.asd995.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vt.lnxyls.cn

Ruby: "A".ord; 65.chr
来源：http://pt.colortex.cn

C#:   (int)'A'; (char)65
来源：http://ps.wgjwhj.cn

[A19] 交换两个变量
来源：http://zq.gzmigu.cn

Py:   a, b = b, a
来源：http://yv.gzmigu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://di.lnxyls.cn

JS:   [a, b] = [b, a];
来源：http://hq.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://kt.9csxet.cn

Java: int t = a; a = b; b = t;
来源：http://ek.hnjuh.cn

Go:   a, b = b, a
来源：http://uy.hnjuh.cn

Ruby: a, b = b, a
来源：http://iq.shtwfgs.cn

C#:   (a, b) = (b, a);
来源：http://dt.muxihuayi.cn

[A20] 读取标准输入
来源：http://ex.szsharing.cn

Py:   name = input("请输入：")
来源：http://au.nszjky.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ni.panjiajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xj.chemitech.net.cn

TS:   // Node.js：readline 模块
来源：http://no.nicolike.cn

Java: new Scanner(System.in).nextLine()
来源：http://wd.huixinmuqiang.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lw.huanxung.cn

Ruby: gets.chomp
来源：http://sx.haigaiapp.cn

C#:   Console.ReadLine();
来源：http://od.huixinmuqiang.cn

[A21] 保留指定小数位输出
来源：http://ta.panjiajie.cn

Py:   f"{3.14159:.2f}"
来源：http://gf.bjjhwx.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wa.bookmarksfly.cn

JS:   (3.14159).toFixed(2)
来源：http://ei.nicolike.cn

TS:   (3.14159).toFixed(2)
来源：http://jt.yuntaijiaju.cn

Java: String.format("%.2f", 3.14159)
来源：http://hn.9csxet.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xt.521024.cn

Ruby: format("%.2f", 3.14159)
来源：http://kp.bjjhwx.cn

C#:   3.14159.ToString("F2")
来源：http://kc.shtwfgs.cn

[A22] 获取字符串长度
来源：http://dj.bookmarksfly.cn

Py:   len(s)
来源：http://zj.asd995.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ni.hnjuh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://eo.huanxung.cn

TS:   s.length
来源：http://rq.huanxung.cn

Java: s.length()
来源：http://zh.bjjhwx.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zy.shtwfgs.cn

Ruby: s.length
来源：http://ns.haigaiapp.cn

C#:   s.Length
来源：http://zn.haigaiapp.cn

[A23] 大小写转换
来源：http://ka.chemitech.net.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://pb.jianghongdianzi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vx.jctech888.com.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yy.huixiangedu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gi.9csxet.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fc.muxihuayi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sa.asd995.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ej.huixinmuqiang.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dz.nszjky.cn

[A24] 去除首尾空白
来源：http://nz.hahajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pr.szsharing.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zi.yuexingan06.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tu.9csxet.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wl.yuntaijiaju.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xg.nicolike.cn

Go:   strings.TrimSpace(s)
来源：http://me.chemitech.net.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nz.huixinmuqiang.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pq.yuexingan06.cn

[A25] 字符串比较
来源：http://ah.bookmarksfly.cn

Py:   s1 == s2; s1 != s2
来源：http://dw.yuntaijiaju.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vb.huixiangedu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zg.hahajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://uo.szxytkj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ev.wgjwhj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pp.nszjky.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ns.9csxet.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nz.nicolike.cn

[A26] 类型转换总览
来源：http://vk.jctech888.com.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ww.wgjwhj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uv.yuntaijiaju.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dj.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://pq.9csxet.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vc.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rn.huixinmuqiang.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zf.asd995.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hn.bookmarksfly.cn

================================================================================
来源：http://dr.asd995.cn

B. 流程控制
来源：http://zn.shtwfgs.cn

================================================================================
来源：http://pr.yuntaijiaju.cn

[B01] 条件判断 if / else
来源：http://sb.shxzskj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lu.gzmigu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sn.521024.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xe.haigaiapp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uo.hahajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://va.hahajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dk.nicolike.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jt.chemitech.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nh.wgjwhj.cn

[B02] 多分支 else if / elif
来源：http://yx.lnxyls.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wr.muxihuayi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ff.nszjky.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lv.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sw.muxihuayi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://go.nicolike.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vf.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vy.jctech888.com.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hh.szxytkj.cn

[B03] switch / match / case
来源：http://yi.chemitech.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wy.newstarts.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nt.nicolike.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mn.panjiajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dv.hnjuh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ym.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rm.shtwfgs.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mo.bjjhwx.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wz.panjiajie.cn

[B04] for 计数循环
来源：http://vz.huanxung.cn

Py:   for i in range(10): print(i)
来源：http://qn.hahajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tb.gzmigu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yj.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ga.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zg.nszjky.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nt.jctech888.com.cn

Ruby: 10.times { |i| puts i }
来源：http://kd.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hb.shxzukj.cn

[B05] 遍历数组 / 列表
来源：http://so.hnjuh.cn

Py:   for item in arr: print(item)
来源：http://mw.gzmigu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sc.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fx.yuexingan06.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xp.shtwfgs.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fc.521024.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xo.huanxung.cn

Ruby: arr.each { |item| puts item }
来源：http://rf.colortex.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ei.haigaiapp.cn

[B06] 遍历字典 / 对象
来源：http://hx.yuexingan06.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jb.colortex.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yl.colortex.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fv.haigaiapp.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://km.colortex.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mb.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ua.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yg.shxzskj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ig.521024.cn

[B07] while 循环
来源：http://lp.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://td.yuexingan06.cn

PHP:  while ($i < 10) { $i++; }
来源：http://me.jctech888.com.cn

JS:   while (i < 10) { i++; }
来源：http://yt.panjiajie.cn

TS:   while (i < 10) { i++; }
来源：http://do.shxzskj.cn

Java: while (i < 10) { i++; }
来源：http://rx.szsharing.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qs.shxzukj.cn

Ruby: while i < 10; i += 1; end
来源：http://gr.szxytkj.cn

C#:   while (i < 10) { i++; }
来源：http://qf.newstarts.cn

[B08] do-while（至少执行一次）
来源：http://de.muxihuayi.cn

Py:   # 无 do-while：用 while True + break
来源：http://pf.bjjhwx.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hc.wgjwhj.cn

JS:   do { i++; } while (i < 10);
来源：http://co.jianghongdianzi.cn

TS:   do { i++; } while (i < 10);
来源：http://ko.shxzskj.cn

Java: do { i++; } while (i < 10);
来源：http://xs.nszjky.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jc.jianghongdianzi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ik.lnxyls.cn

C#:   do { i++; } while (i < 10);
来源：http://rn.521024.cn

[B09] break 与 continue
来源：http://qi.asd995.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://aa.nszjky.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ce.9csxet.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://em.szsharing.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ih.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fx.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://km.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ez.nicolike.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gs.521024.cn

[B10] 遍历同时拿索引
来源：http://xy.szsharing.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://aq.bookmarksfly.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ry.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vu.gzmigu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fz.521024.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kz.shtwfgs.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://go.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mg.chemitech.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://oh.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://re.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://nh.hnjuh.cn

PHP:  range(0, 10, 2);
来源：http://lf.newstarts.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ae.haigaiapp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kg.muxihuayi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zz.jctech888.com.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lh.jctech888.com.cn

Ruby: (0...10).step(2).to_a
来源：http://hu.hahajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://th.jctech888.com.cn

[B12] 跳出多层循环
来源：http://jd.jctech888.com.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cq.panjiajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zr.jctech888.com.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oh.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vv.shxzskj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xp.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ep.huixiangedu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://td.lnxyls.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qw.colortex.cn

[B13] 判断是否为数字
来源：http://kl.muxihuayi.cn

Py:   isinstance(x, (int, float))
来源：http://xa.newstarts.cn

PHP:  is_numeric($x)
来源：http://sc.chemitech.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ed.bookmarksfly.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rw.bookmarksfly.cn

Java: x instanceof Number
来源：http://pj.shxzskj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cs.9csxet.cn

Ruby: x.is_a?(Numeric)
来源：http://yl.chemitech.net.cn

C#:   x is int or double or decimal
来源：http://cu.gzmigu.cn

[B14] 判断值是否在集合内
来源：http://qt.huixinmuqiang.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kp.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vt.asd995.cn

JS:   [1, 2, 3].includes(x)
来源：http://ll.bjjhwx.cn

TS:   [1, 2, 3].includes(x)
来源：http://ig.asd995.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://no.newstarts.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tg.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gk.521024.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ga.huanxung.cn

[B15] 布尔运算与取反
来源：http://tq.jianghongdianzi.cn

Py:   a and b or not c
来源：http://wq.colortex.cn

PHP:  $a && $b || !$c
来源：http://go.newstarts.cn

JS:   a && b || !c
来源：http://gx.chemitech.net.cn

TS:   a && b || !c
来源：http://hl.asd995.cn

Java: a && b || !c
来源：http://vl.wgjwhj.cn

Go:   a && b || !c
来源：http://rn.nicolike.cn

Ruby: a && b || !c
来源：http://bt.hnjuh.cn

C#:   a && b || !c
来源：http://pp.hnjuh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jd.shxzskj.cn

Py:   if not data: return
来源：http://ut.haigaiapp.cn

PHP:  if (!$data) { return; }
来源：http://gu.newstarts.cn

JS:   if (!data) return;
来源：http://pw.9csxet.cn

TS:   if (!data) return;
来源：http://mf.szsharing.cn

Java: if (data == null) return;
来源：http://is.asd995.cn

Go:   if data == nil { return }
来源：http://cq.muxihuayi.cn

Ruby: return if data.nil?
来源：http://xq.521024.cn

C#:   if (data == null) return;
来源：http://cw.bjjhwx.cn

================================================================================
来源：http://lu.9csxet.cn

C. 函数与作用域
来源：http://tr.muxihuayi.cn

================================================================================
来源：http://pv.521024.cn

[C01] 定义函数
来源：http://xp.newstarts.cn

Py:   def add(a, b): return a + b
来源：http://nz.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lh.colortex.cn

JS:   function add(a, b) { return a + b; }
来源：http://ip.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bf.colortex.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bn.huanxung.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mr.nicolike.cn

Ruby: def add(a, b); a + b; end
来源：http://oa.9csxet.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wd.jianghongdianzi.cn

[C02] 默认参数
来源：http://sh.hahajie.cn

Py:   def greet(name="World"): return name
来源：http://yc.gzmigu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hh.shxzukj.cn

JS:   function greet(name = "World") { return name; }
来源：http://zb.haigaiapp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://io.shxzskj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://in.wgjwhj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fz.shtwfgs.cn

Ruby: def greet(name = "World") = name
来源：http://kx.shxzskj.cn

C#:   string Greet(string name = "World") => name;
来源：http://jv.nicolike.cn

[C03] 可变参数
来源：http://jy.shtwfgs.cn

Py:   def total(*args): return sum(args)
来源：http://qm.shxzskj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mx.haigaiapp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vq.bookmarksfly.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ig.haigaiapp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://os.shxzskj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hj.yuntaijiaju.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ir.bjjhwx.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mf.wgjwhj.cn

[C04] 命名参数 / 关键字参数
来源：http://ay.yuexingan06.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ez.yuexingan06.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tf.szxytkj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://md.jianghongdianzi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tr.bookmarksfly.cn

Java: // 无：用 Builder 模式或 record
来源：http://zr.nszjky.cn

Go:   // 无：用配置结构体参数
来源：http://qo.shxzukj.cn

Ruby: f(a: 1, b: 2)
来源：http://js.yuexingan06.cn

C#:   f(a: 1, b: 2)
来源：http://hm.panjiajie.cn

[C05] 返回多个值
来源：http://hz.szxytkj.cn

Py:   return a, b
来源：http://pc.bookmarksfly.cn

PHP:  return [$a, $b];
来源：http://xv.yuntaijiaju.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vr.yuntaijiaju.cn

TS:   return { a, b };
来源：http://hj.huanxung.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zi.nicolike.cn

Go:   return a, b
来源：http://dk.shtwfgs.cn

Ruby: return a, b
来源：http://gc.shxzskj.cn

C#:   return (a, b);              // ValueTuple
来源：http://wo.huixiangedu.cn

[C06] 匿名函数 / lambda
来源：http://fw.shxzukj.cn

Py:   square = lambda x: x * x
来源：http://hz.panjiajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sv.hahajie.cn

JS:   const square = x => x * x;
来源：http://pe.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://ju.lnxyls.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rf.yuexingan06.cn

Go:   sq := func(x int) int { return x * x }
来源：http://an.9csxet.cn

Ruby: square = ->(x) { x * x }
来源：http://ob.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ej.newstarts.cn

[C07] 把函数作为参数传入
来源：http://ze.jianghongdianzi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ld.shxzukj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wx.panjiajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vq.hnjuh.cn

TS:   arr.map(String)
来源：http://wn.bookmarksfly.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jn.jctech888.com.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wo.haigaiapp.cn

Ruby: arr.map(&:upcase)
来源：http://yi.jianghongdianzi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://du.newstarts.cn

[C08] 闭包
来源：http://zs.wgjwhj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gz.nszjky.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ku.9csxet.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ec.chemitech.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jd.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://id.bookmarksfly.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vy.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hd.521024.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fw.gzmigu.cn

[C09] 递归
来源：http://ky.wgjwhj.cn


<!-- 参考信息 -->