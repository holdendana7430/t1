代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xf.hahajie.cn

Java: (int) 'A'; (char) 65
来源：http://tg.huixinmuqiang.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pg.bookmarksfly.cn

Ruby: "A".ord; 65.chr
来源：http://ge.521024.cn

C#:   (int)'A'; (char)65
来源：http://ay.bjjhwx.cn

[A19] 交换两个变量
来源：http://ha.nicolike.cn

Py:   a, b = b, a
来源：http://nn.bookmarksfly.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fz.lnxyls.cn

JS:   [a, b] = [b, a];
来源：http://bf.jianghongdianzi.cn

TS:   [a, b] = [b, a];
来源：http://np.szxytkj.cn

Java: int t = a; a = b; b = t;
来源：http://ir.szxytkj.cn

Go:   a, b = b, a
来源：http://il.yuntaijiaju.cn

Ruby: a, b = b, a
来源：http://ho.chemitech.net.cn

C#:   (a, b) = (b, a);
来源：http://vk.bjjhwx.cn

[A20] 读取标准输入
来源：http://pg.hnjuh.cn

Py:   name = input("请输入：")
来源：http://fk.colortex.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://go.newstarts.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tu.hnjuh.cn

TS:   // Node.js：readline 模块
来源：http://pz.haigaiapp.cn

Java: new Scanner(System.in).nextLine()
来源：http://rb.yuntaijiaju.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qc.yuexingan06.cn

Ruby: gets.chomp
来源：http://lc.nszjky.cn

C#:   Console.ReadLine();
来源：http://my.chemitech.net.cn

[A21] 保留指定小数位输出
来源：http://kf.huixiangedu.cn

Py:   f"{3.14159:.2f}"
来源：http://op.colortex.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ig.huixinmuqiang.cn

JS:   (3.14159).toFixed(2)
来源：http://hc.shtwfgs.cn

TS:   (3.14159).toFixed(2)
来源：http://jc.shtwfgs.cn

Java: String.format("%.2f", 3.14159)
来源：http://yi.shxzukj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zy.colortex.cn

Ruby: format("%.2f", 3.14159)
来源：http://um.9csxet.cn

C#:   3.14159.ToString("F2")
来源：http://bd.shxzskj.cn

[A22] 获取字符串长度
来源：http://ub.gzmigu.cn

Py:   len(s)
来源：http://dv.shxzskj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ob.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ma.yuntaijiaju.cn

TS:   s.length
来源：http://ya.9csxet.cn

Java: s.length()
来源：http://sp.haigaiapp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gm.huanxung.cn

Ruby: s.length
来源：http://ms.shxzskj.cn

C#:   s.Length
来源：http://yx.lnxyls.cn

[A23] 大小写转换
来源：http://wl.hnjuh.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ae.szxytkj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ty.colortex.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jm.gzmigu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://au.bjjhwx.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pk.521024.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pf.521024.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ic.shxzukj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://uz.hnjuh.cn

[A24] 去除首尾空白
来源：http://kj.colortex.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://js.shtwfgs.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zt.gzmigu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mu.521024.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wg.9csxet.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ov.colortex.cn

Go:   strings.TrimSpace(s)
来源：http://xi.muxihuayi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://th.521024.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gf.muxihuayi.cn

[A25] 字符串比较
来源：http://fl.shtwfgs.cn

Py:   s1 == s2; s1 != s2
来源：http://jr.bjjhwx.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xy.yuexingan06.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ys.panjiajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dp.asd995.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ch.colortex.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dh.gzmigu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://be.shxzukj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://al.lnxyls.cn

[A26] 类型转换总览
来源：http://ut.yuexingan06.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ry.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jz.jianghongdianzi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://eo.wgjwhj.cn

TS:   Number() String() Boolean() x as number
来源：http://vn.shtwfgs.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xf.shtwfgs.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mq.shxzukj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nk.bjjhwx.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nj.shxzskj.cn

================================================================================
来源：http://wu.jctech888.com.cn

B. 流程控制
来源：http://lx.hahajie.cn

================================================================================
来源：http://gn.9csxet.cn

[B01] 条件判断 if / else
来源：http://ck.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://az.colortex.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://po.shtwfgs.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ow.newstarts.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uh.nicolike.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wc.huanxung.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hl.shtwfgs.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yy.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ry.szsharing.cn

[B02] 多分支 else if / elif
来源：http://vt.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fq.9csxet.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://af.szxytkj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vu.newstarts.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lt.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lx.hahajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mj.huixinmuqiang.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://id.shtwfgs.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://et.chemitech.net.cn

[B03] switch / match / case
来源：http://ef.colortex.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cg.jianghongdianzi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vq.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lg.nszjky.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hp.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pm.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://os.bjjhwx.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tr.gzmigu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hg.jianghongdianzi.cn

[B04] for 计数循环
来源：http://qj.bookmarksfly.cn

Py:   for i in range(10): print(i)
来源：http://sq.wgjwhj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ib.szxytkj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://td.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nc.huixinmuqiang.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jo.haigaiapp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rk.szxytkj.cn

Ruby: 10.times { |i| puts i }
来源：http://fh.shtwfgs.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://km.shxzskj.cn

[B05] 遍历数组 / 列表
来源：http://hq.yuexingan06.cn

Py:   for item in arr: print(item)
来源：http://hu.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sd.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wi.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dz.szsharing.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dj.shxzukj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vz.shxzskj.cn

Ruby: arr.each { |item| puts item }
来源：http://qs.gzmigu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qp.asd995.cn

[B06] 遍历字典 / 对象
来源：http://ht.jctech888.com.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jg.9csxet.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fy.panjiajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://in.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ll.colortex.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fa.chemitech.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nm.shtwfgs.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://if.wgjwhj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://da.szsharing.cn

[B07] while 循环
来源：http://so.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://ml.jctech888.com.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ly.shtwfgs.cn

JS:   while (i < 10) { i++; }
来源：http://us.shxzukj.cn

TS:   while (i < 10) { i++; }
来源：http://yt.shtwfgs.cn

Java: while (i < 10) { i++; }
来源：http://ar.shxzskj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rg.haigaiapp.cn

Ruby: while i < 10; i += 1; end
来源：http://aa.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://jk.lnxyls.cn

[B08] do-while（至少执行一次）
来源：http://rs.bookmarksfly.cn

Py:   # 无 do-while：用 while True + break
来源：http://iu.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kq.bookmarksfly.cn

JS:   do { i++; } while (i < 10);
来源：http://gp.bjjhwx.cn

TS:   do { i++; } while (i < 10);
来源：http://mg.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://dy.nszjky.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hi.szxytkj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ax.szxytkj.cn

C#:   do { i++; } while (i < 10);
来源：http://fb.hnjuh.cn

[B09] break 与 continue
来源：http://fh.szsharing.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gr.gzmigu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jn.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nm.wgjwhj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pt.huixinmuqiang.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tb.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xh.jctech888.com.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ka.shtwfgs.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ci.shxzukj.cn

[B10] 遍历同时拿索引
来源：http://zx.9csxet.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ob.haigaiapp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ly.bookmarksfly.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hr.shxzskj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ti.szsharing.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nw.jctech888.com.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gv.gzmigu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kk.newstarts.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ps.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://zo.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://ev.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://zy.gzmigu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zx.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xj.huixiangedu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sh.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uv.yuntaijiaju.cn

Ruby: (0...10).step(2).to_a
来源：http://vp.muxihuayi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bb.hahajie.cn

[B12] 跳出多层循环
来源：http://uq.szsharing.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qg.szxytkj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://on.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wb.bjjhwx.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://np.shxzukj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ey.wgjwhj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://de.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://km.szxytkj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hu.yuntaijiaju.cn

[B13] 判断是否为数字
来源：http://fk.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://qs.szxytkj.cn

PHP:  is_numeric($x)
来源：http://hb.shxzskj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ua.shxzukj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sk.shxzskj.cn

Java: x instanceof Number
来源：http://cf.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lc.hahajie.cn

Ruby: x.is_a?(Numeric)
来源：http://lu.huanxung.cn

C#:   x is int or double or decimal
来源：http://bt.szxytkj.cn

[B14] 判断值是否在集合内
来源：http://tt.chemitech.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jz.szxytkj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rp.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://uv.lnxyls.cn

TS:   [1, 2, 3].includes(x)
来源：http://jm.9csxet.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ty.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rq.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jv.521024.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yd.bookmarksfly.cn

[B15] 布尔运算与取反
来源：http://al.huixinmuqiang.cn

Py:   a and b or not c
来源：http://rl.9csxet.cn

PHP:  $a && $b || !$c
来源：http://ks.yuntaijiaju.cn

JS:   a && b || !c
来源：http://cr.shxzukj.cn

TS:   a && b || !c
来源：http://cm.szxytkj.cn

Java: a && b || !c
来源：http://bb.muxihuayi.cn

Go:   a && b || !c
来源：http://bi.jianghongdianzi.cn

Ruby: a && b || !c
来源：http://jn.huixiangedu.cn

C#:   a && b || !c
来源：http://gf.panjiajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bv.muxihuayi.cn

Py:   if not data: return
来源：http://cj.chemitech.net.cn

PHP:  if (!$data) { return; }
来源：http://vg.jctech888.com.cn

JS:   if (!data) return;
来源：http://re.jianghongdianzi.cn

TS:   if (!data) return;
来源：http://sz.wgjwhj.cn

Java: if (data == null) return;
来源：http://hj.chemitech.net.cn

Go:   if data == nil { return }
来源：http://cf.wgjwhj.cn

Ruby: return if data.nil?
来源：http://hz.shxzskj.cn

C#:   if (data == null) return;
来源：http://az.hnjuh.cn

================================================================================
来源：http://te.asd995.cn

C. 函数与作用域
来源：http://qo.lnxyls.cn

================================================================================
来源：http://kd.chemitech.net.cn

[C01] 定义函数
来源：http://bl.nicolike.cn

Py:   def add(a, b): return a + b
来源：http://pq.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ur.bookmarksfly.cn

JS:   function add(a, b) { return a + b; }
来源：http://kn.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ai.yuexingan06.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zt.nicolike.cn

Go:   func add(a, b int) int { return a + b }
来源：http://su.gzmigu.cn

Ruby: def add(a, b); a + b; end
来源：http://de.lnxyls.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vy.nicolike.cn

[C02] 默认参数
来源：http://bs.wgjwhj.cn

Py:   def greet(name="World"): return name
来源：http://as.shxzukj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jg.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://uw.colortex.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jo.muxihuayi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zl.bjjhwx.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rv.shtwfgs.cn

Ruby: def greet(name = "World") = name
来源：http://sg.asd995.cn

C#:   string Greet(string name = "World") => name;
来源：http://xj.muxihuayi.cn

[C03] 可变参数
来源：http://un.hahajie.cn

Py:   def total(*args): return sum(args)
来源：http://fi.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cp.szsharing.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lg.huanxung.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://st.shxzskj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qo.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ve.jctech888.com.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ik.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gl.chemitech.net.cn

[C04] 命名参数 / 关键字参数
来源：http://mu.huanxung.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lr.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zp.huixiangedu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qg.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ks.9csxet.cn

Java: // 无：用 Builder 模式或 record
来源：http://fx.hahajie.cn

Go:   // 无：用配置结构体参数
来源：http://uh.yuexingan06.cn

Ruby: f(a: 1, b: 2)
来源：http://en.colortex.cn

C#:   f(a: 1, b: 2)
来源：http://vb.bjjhwx.cn

[C05] 返回多个值
来源：http://au.521024.cn

Py:   return a, b
来源：http://hx.hnjuh.cn

PHP:  return [$a, $b];
来源：http://gy.bookmarksfly.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qc.521024.cn

TS:   return { a, b };
来源：http://xh.haigaiapp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ui.wgjwhj.cn

Go:   return a, b
来源：http://uf.panjiajie.cn

Ruby: return a, b
来源：http://uw.newstarts.cn

C#:   return (a, b);              // ValueTuple
来源：http://ry.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://tc.szxytkj.cn

Py:   square = lambda x: x * x
来源：http://mg.panjiajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://lp.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://pz.szxytkj.cn

TS:   const square = (x: number): number => x * x;
来源：http://uj.hahajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nc.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jb.nszjky.cn

Ruby: square = ->(x) { x * x }
来源：http://iu.muxihuayi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://if.asd995.cn

[C07] 把函数作为参数传入
来源：http://qo.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sy.9csxet.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fy.lnxyls.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zj.wgjwhj.cn

TS:   arr.map(String)
来源：http://tn.panjiajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ws.wgjwhj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qj.yuntaijiaju.cn

Ruby: arr.map(&:upcase)
来源：http://yz.shxzskj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ik.bookmarksfly.cn

[C08] 闭包
来源：http://xh.yuexingan06.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xa.shtwfgs.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kw.panjiajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lj.hahajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zg.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ll.huanxung.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pp.chemitech.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yh.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wm.szsharing.cn

[C09] 递归
来源：http://mr.asd995.cn


<!-- 参考信息 -->