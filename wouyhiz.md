代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://fy.shxzukj.cn

Py:   ord("A"); chr(65)
来源：http://sq.shxzskj.cn

PHP:  ord("A"); chr(65)
来源：http://ox.wgjwhj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nh.shtwfgs.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uj.gzmigu.cn

Java: (int) 'A'; (char) 65
来源：http://by.haigaiapp.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gd.panjiajie.cn

Ruby: "A".ord; 65.chr
来源：http://ay.jctech888.com.cn

C#:   (int)'A'; (char)65
来源：http://sp.haigaiapp.cn

[A19] 交换两个变量
来源：http://oy.jctech888.com.cn

Py:   a, b = b, a
来源：http://ot.colortex.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://pv.bookmarksfly.cn

JS:   [a, b] = [b, a];
来源：http://yd.hnjuh.cn

TS:   [a, b] = [b, a];
来源：http://ql.nicolike.cn

Java: int t = a; a = b; b = t;
来源：http://ig.lnxyls.cn

Go:   a, b = b, a
来源：http://ie.panjiajie.cn

Ruby: a, b = b, a
来源：http://pu.jctech888.com.cn

C#:   (a, b) = (b, a);
来源：http://gy.huixiangedu.cn

[A20] 读取标准输入
来源：http://my.yuexingan06.cn

Py:   name = input("请输入：")
来源：http://eb.nszjky.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://go.jctech888.com.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jj.jianghongdianzi.cn

TS:   // Node.js：readline 模块
来源：http://nr.wgjwhj.cn

Java: new Scanner(System.in).nextLine()
来源：http://hh.huixiangedu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pq.yuntaijiaju.cn

Ruby: gets.chomp
来源：http://kk.shxzukj.cn

C#:   Console.ReadLine();
来源：http://si.shxzukj.cn

[A21] 保留指定小数位输出
来源：http://ay.newstarts.cn

Py:   f"{3.14159:.2f}"
来源：http://bm.9csxet.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mm.yuexingan06.cn

JS:   (3.14159).toFixed(2)
来源：http://rl.hnjuh.cn

TS:   (3.14159).toFixed(2)
来源：http://mt.haigaiapp.cn

Java: String.format("%.2f", 3.14159)
来源：http://fk.newstarts.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gm.szxytkj.cn

Ruby: format("%.2f", 3.14159)
来源：http://zz.huanxung.cn

C#:   3.14159.ToString("F2")
来源：http://xj.wgjwhj.cn

[A22] 获取字符串长度
来源：http://ya.colortex.cn

Py:   len(s)
来源：http://er.jianghongdianzi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ae.nicolike.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wj.lnxyls.cn

TS:   s.length
来源：http://st.yuexingan06.cn

Java: s.length()
来源：http://nu.jianghongdianzi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dn.jianghongdianzi.cn

Ruby: s.length
来源：http://oj.hnjuh.cn

C#:   s.Length
来源：http://ye.wgjwhj.cn

[A23] 大小写转换
来源：http://uy.521024.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gs.shtwfgs.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rr.szxytkj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://js.chemitech.net.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zn.huixinmuqiang.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tj.hnjuh.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tv.9csxet.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uu.521024.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://oo.9csxet.cn

[A24] 去除首尾空白
来源：http://kj.hnjuh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xc.szsharing.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kj.jctech888.com.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ow.asd995.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xv.bjjhwx.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ha.jctech888.com.cn

Go:   strings.TrimSpace(s)
来源：http://bb.lnxyls.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ks.bookmarksfly.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pr.haigaiapp.cn

[A25] 字符串比较
来源：http://qf.asd995.cn

Py:   s1 == s2; s1 != s2
来源：http://fm.szsharing.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ub.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pj.yuexingan06.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ji.shtwfgs.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ku.newstarts.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cl.muxihuayi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://oz.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ww.huixiangedu.cn

[A26] 类型转换总览
来源：http://wd.chemitech.net.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gw.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ey.bookmarksfly.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://aw.huixiangedu.cn

TS:   Number() String() Boolean() x as number
来源：http://oq.szsharing.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ka.hahajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://re.huixinmuqiang.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ab.bjjhwx.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zx.panjiajie.cn

================================================================================
来源：http://yt.bjjhwx.cn

B. 流程控制
来源：http://te.haigaiapp.cn

================================================================================
来源：http://yl.hnjuh.cn

[B01] 条件判断 if / else
来源：http://eg.shxzukj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://sp.huanxung.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qg.yuntaijiaju.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rg.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qh.lnxyls.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://aa.wgjwhj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pb.colortex.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wq.huanxung.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mn.lnxyls.cn

[B02] 多分支 else if / elif
来源：http://pj.lnxyls.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yt.bookmarksfly.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ke.shxzukj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dn.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jr.hnjuh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ha.lnxyls.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fv.shxzskj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xr.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uo.jctech888.com.cn

[B03] switch / match / case
来源：http://zf.nicolike.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gt.gzmigu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xk.521024.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://od.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://am.yuexingan06.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xv.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vl.huanxung.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kp.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tp.colortex.cn

[B04] for 计数循环
来源：http://xl.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://yl.shxzskj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dx.yuntaijiaju.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ka.huanxung.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mn.shtwfgs.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mx.nszjky.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ev.hahajie.cn

Ruby: 10.times { |i| puts i }
来源：http://iz.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gz.chemitech.net.cn

[B05] 遍历数组 / 列表
来源：http://vl.panjiajie.cn

Py:   for item in arr: print(item)
来源：http://fg.newstarts.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zw.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wn.lnxyls.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://uc.gzmigu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ea.hnjuh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bf.shxzskj.cn

Ruby: arr.each { |item| puts item }
来源：http://cq.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fc.muxihuayi.cn

[B06] 遍历字典 / 对象
来源：http://gh.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ci.nicolike.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nr.shxzukj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oj.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ce.chemitech.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://su.newstarts.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sa.bookmarksfly.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qe.huixinmuqiang.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cz.hahajie.cn

[B07] while 循环
来源：http://fl.asd995.cn

Py:   while i < 10: i += 1
来源：http://ep.bookmarksfly.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lg.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://yn.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://wa.panjiajie.cn

Java: while (i < 10) { i++; }
来源：http://bp.newstarts.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oa.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://ok.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://mj.szxytkj.cn

[B08] do-while（至少执行一次）
来源：http://sy.newstarts.cn

Py:   # 无 do-while：用 while True + break
来源：http://nl.shxzukj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hj.yuntaijiaju.cn

JS:   do { i++; } while (i < 10);
来源：http://lj.szxytkj.cn

TS:   do { i++; } while (i < 10);
来源：http://ry.muxihuayi.cn

Java: do { i++; } while (i < 10);
来源：http://yz.szsharing.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xo.muxihuayi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://as.gzmigu.cn

C#:   do { i++; } while (i < 10);
来源：http://jq.hahajie.cn

[B09] break 与 continue
来源：http://cu.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cr.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mz.chemitech.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://km.nszjky.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nw.wgjwhj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ac.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wu.haigaiapp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ww.haigaiapp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ar.jianghongdianzi.cn

[B10] 遍历同时拿索引
来源：http://fn.nicolike.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://st.hahajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nq.colortex.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nf.hnjuh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bk.bjjhwx.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jc.jctech888.com.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://in.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rs.panjiajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://aa.colortex.cn

[B11] 生成数字序列 / 区间
来源：http://ro.9csxet.cn

Py:   list(range(0, 10, 2))
来源：http://ct.jctech888.com.cn

PHP:  range(0, 10, 2);
来源：http://dl.nicolike.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hy.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hl.bookmarksfly.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fy.wgjwhj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ku.jctech888.com.cn

Ruby: (0...10).step(2).to_a
来源：http://je.nicolike.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ga.hnjuh.cn

[B12] 跳出多层循环
来源：http://qu.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yo.huixiangedu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://si.szsharing.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wz.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tp.jctech888.com.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ni.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uk.colortex.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bd.hnjuh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wp.jctech888.com.cn

[B13] 判断是否为数字
来源：http://kv.nicolike.cn

Py:   isinstance(x, (int, float))
来源：http://rn.asd995.cn

PHP:  is_numeric($x)
来源：http://tr.gzmigu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://le.yuntaijiaju.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://un.huixinmuqiang.cn

Java: x instanceof Number
来源：http://vu.panjiajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jg.hnjuh.cn

Ruby: x.is_a?(Numeric)
来源：http://ab.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://it.colortex.cn

[B14] 判断值是否在集合内
来源：http://sx.panjiajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fx.nicolike.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yb.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://yq.yuntaijiaju.cn

TS:   [1, 2, 3].includes(x)
来源：http://vd.9csxet.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kt.asd995.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tk.yuexingan06.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xn.nicolike.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zd.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://fi.521024.cn

Py:   a and b or not c
来源：http://ek.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://jd.wgjwhj.cn

JS:   a && b || !c
来源：http://zz.shtwfgs.cn

TS:   a && b || !c
来源：http://cr.wgjwhj.cn

Java: a && b || !c
来源：http://ok.newstarts.cn

Go:   a && b || !c
来源：http://if.gzmigu.cn

Ruby: a && b || !c
来源：http://uf.szsharing.cn

C#:   a && b || !c
来源：http://mu.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tw.hnjuh.cn

Py:   if not data: return
来源：http://bh.panjiajie.cn

PHP:  if (!$data) { return; }
来源：http://kj.huanxung.cn

JS:   if (!data) return;
来源：http://df.huanxung.cn

TS:   if (!data) return;
来源：http://zi.hahajie.cn

Java: if (data == null) return;
来源：http://mh.asd995.cn

Go:   if data == nil { return }
来源：http://br.colortex.cn

Ruby: return if data.nil?
来源：http://pz.bjjhwx.cn

C#:   if (data == null) return;
来源：http://eb.bookmarksfly.cn

================================================================================
来源：http://rk.hnjuh.cn

C. 函数与作用域
来源：http://fr.hnjuh.cn

================================================================================
来源：http://hh.szxytkj.cn

[C01] 定义函数
来源：http://io.haigaiapp.cn

Py:   def add(a, b): return a + b
来源：http://mb.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pj.yuntaijiaju.cn

JS:   function add(a, b) { return a + b; }
来源：http://qb.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ik.gzmigu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qs.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cp.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://le.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ex.huanxung.cn

[C02] 默认参数
来源：http://qx.szsharing.cn

Py:   def greet(name="World"): return name
来源：http://am.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bk.bookmarksfly.cn

JS:   function greet(name = "World") { return name; }
来源：http://ox.shxzukj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rv.shxzskj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://uz.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tk.panjiajie.cn

Ruby: def greet(name = "World") = name
来源：http://gs.shtwfgs.cn

C#:   string Greet(string name = "World") => name;
来源：http://qj.muxihuayi.cn

[C03] 可变参数
来源：http://fd.shxzukj.cn

Py:   def total(*args): return sum(args)
来源：http://ti.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qw.wgjwhj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hu.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zx.shxzukj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rg.chemitech.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ms.nszjky.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bj.jianghongdianzi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hw.huixiangedu.cn

[C04] 命名参数 / 关键字参数
来源：http://rd.asd995.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yo.bjjhwx.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tp.9csxet.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ed.jianghongdianzi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gi.colortex.cn

Java: // 无：用 Builder 模式或 record
来源：http://qa.gzmigu.cn

Go:   // 无：用配置结构体参数
来源：http://ah.bookmarksfly.cn

Ruby: f(a: 1, b: 2)
来源：http://vd.shxzskj.cn

C#:   f(a: 1, b: 2)
来源：http://mm.huixinmuqiang.cn

[C05] 返回多个值
来源：http://yf.szxytkj.cn

Py:   return a, b
来源：http://dx.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://dw.jctech888.com.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://gz.szxytkj.cn

TS:   return { a, b };
来源：http://no.szxytkj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ju.szsharing.cn

Go:   return a, b
来源：http://ya.nicolike.cn

Ruby: return a, b
来源：http://zk.szsharing.cn

C#:   return (a, b);              // ValueTuple
来源：http://je.jianghongdianzi.cn

[C06] 匿名函数 / lambda
来源：http://qu.colortex.cn

Py:   square = lambda x: x * x
来源：http://gg.nicolike.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yn.hnjuh.cn

JS:   const square = x => x * x;
来源：http://bm.jctech888.com.cn

TS:   const square = (x: number): number => x * x;
来源：http://kl.huixinmuqiang.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rf.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lr.shxzskj.cn

Ruby: square = ->(x) { x * x }
来源：http://wa.szxytkj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bq.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://oa.shtwfgs.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qt.huixinmuqiang.cn

PHP:  array_map("strtoupper", $arr);
来源：http://sd.lnxyls.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wl.haigaiapp.cn

TS:   arr.map(String)
来源：http://ii.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://iq.gzmigu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zc.wgjwhj.cn

Ruby: arr.map(&:upcase)
来源：http://yk.szsharing.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zr.yuntaijiaju.cn

[C08] 闭包
来源：http://ap.9csxet.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jm.yuexingan06.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yt.huixinmuqiang.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rv.huanxung.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jz.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qc.szsharing.cn


<!-- 参考信息 -->