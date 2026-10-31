代发 wailian999

Ruby: a, b = b, a
来源：http://eh.muxihuayi.cn

C#:   (a, b) = (b, a);
来源：http://mg.yuexingan06.cn

[A20] 读取标准输入
来源：http://tf.szsharing.cn

Py:   name = input("请输入：")
来源：http://mx.wgjwhj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://vm.chemitech.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hi.newstarts.cn

TS:   // Node.js：readline 模块
来源：http://eq.huanxung.cn

Java: new Scanner(System.in).nextLine()
来源：http://vo.wgjwhj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qs.wgjwhj.cn

Ruby: gets.chomp
来源：http://xe.nszjky.cn

C#:   Console.ReadLine();
来源：http://dj.hahajie.cn

[A21] 保留指定小数位输出
来源：http://tq.haigaiapp.cn

Py:   f"{3.14159:.2f}"
来源：http://zi.shxzskj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hh.wgjwhj.cn

JS:   (3.14159).toFixed(2)
来源：http://rx.jianghongdianzi.cn

TS:   (3.14159).toFixed(2)
来源：http://cb.jianghongdianzi.cn

Java: String.format("%.2f", 3.14159)
来源：http://do.9csxet.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wp.muxihuayi.cn

Ruby: format("%.2f", 3.14159)
来源：http://ic.521024.cn

C#:   3.14159.ToString("F2")
来源：http://zi.szxytkj.cn

[A22] 获取字符串长度
来源：http://zf.huanxung.cn

Py:   len(s)
来源：http://yh.colortex.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tw.hnjuh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://of.bookmarksfly.cn

TS:   s.length
来源：http://hn.shxzskj.cn

Java: s.length()
来源：http://ac.wgjwhj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qx.lnxyls.cn

Ruby: s.length
来源：http://te.shtwfgs.cn

C#:   s.Length
来源：http://il.shxzskj.cn

[A23] 大小写转换
来源：http://qd.szxytkj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rm.nszjky.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://db.gzmigu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jh.jianghongdianzi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xa.hahajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bx.panjiajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kk.lnxyls.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vo.szsharing.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ef.shxzukj.cn

[A24] 去除首尾空白
来源：http://pu.huixiangedu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zp.haigaiapp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mz.9csxet.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uy.newstarts.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ub.nszjky.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://es.szxytkj.cn

Go:   strings.TrimSpace(s)
来源：http://xv.colortex.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zm.shxzukj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://se.jctech888.com.cn

[A25] 字符串比较
来源：http://fe.colortex.cn

Py:   s1 == s2; s1 != s2
来源：http://hd.yuntaijiaju.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://oh.szxytkj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tf.chemitech.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wl.szsharing.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jb.huixinmuqiang.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ry.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ns.nszjky.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zq.shxzukj.cn

[A26] 类型转换总览
来源：http://ug.muxihuayi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://na.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bd.nszjky.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://et.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://jc.hahajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pi.panjiajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yi.nszjky.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ul.shtwfgs.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yy.shxzukj.cn

================================================================================
来源：http://qe.shxzskj.cn

B. 流程控制
来源：http://oo.jianghongdianzi.cn

================================================================================
来源：http://xl.huixiangedu.cn

[B01] 条件判断 if / else
来源：http://jj.9csxet.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zd.jctech888.com.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qb.shtwfgs.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kk.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://og.huixiangedu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://do.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kg.huixinmuqiang.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hf.yuexingan06.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fq.lnxyls.cn

[B02] 多分支 else if / elif
来源：http://hu.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vs.szsharing.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ub.hahajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://br.hahajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jq.jianghongdianzi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ej.chemitech.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yh.huanxung.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pi.nicolike.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pc.colortex.cn

[B03] switch / match / case
来源：http://qw.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ta.huixiangedu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://st.jctech888.com.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dh.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lr.haigaiapp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ft.hahajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ib.huixinmuqiang.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bf.haigaiapp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wr.chemitech.net.cn

[B04] for 计数循环
来源：http://sb.colortex.cn

Py:   for i in range(10): print(i)
来源：http://sm.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ek.nicolike.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ib.bjjhwx.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xo.chemitech.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qs.szxytkj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bh.nszjky.cn

Ruby: 10.times { |i| puts i }
来源：http://ye.bjjhwx.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yx.muxihuayi.cn

[B05] 遍历数组 / 列表
来源：http://ad.521024.cn

Py:   for item in arr: print(item)
来源：http://du.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tu.gzmigu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wu.gzmigu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nr.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ar.bjjhwx.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sv.asd995.cn

Ruby: arr.each { |item| puts item }
来源：http://xl.huanxung.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kc.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://vt.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ha.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ak.shxzukj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://th.bjjhwx.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jl.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qi.huixiangedu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pw.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tr.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hv.chemitech.net.cn

[B07] while 循环
来源：http://kr.huixiangedu.cn

Py:   while i < 10: i += 1
来源：http://hg.shxzskj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bm.muxihuayi.cn

JS:   while (i < 10) { i++; }
来源：http://sj.hnjuh.cn

TS:   while (i < 10) { i++; }
来源：http://lk.yuntaijiaju.cn

Java: while (i < 10) { i++; }
来源：http://ja.bjjhwx.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gj.hnjuh.cn

Ruby: while i < 10; i += 1; end
来源：http://vw.yuexingan06.cn

C#:   while (i < 10) { i++; }
来源：http://rk.haigaiapp.cn

[B08] do-while（至少执行一次）
来源：http://wt.huixiangedu.cn

Py:   # 无 do-while：用 while True + break
来源：http://oe.huixinmuqiang.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ie.colortex.cn

JS:   do { i++; } while (i < 10);
来源：http://qa.shtwfgs.cn

TS:   do { i++; } while (i < 10);
来源：http://bh.wgjwhj.cn

Java: do { i++; } while (i < 10);
来源：http://br.newstarts.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ya.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dj.asd995.cn

C#:   do { i++; } while (i < 10);
来源：http://gn.chemitech.net.cn

[B09] break 与 continue
来源：http://na.asd995.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hh.yuexingan06.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xu.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fx.bjjhwx.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bo.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pi.bjjhwx.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jh.colortex.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rg.huixiangedu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://em.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://li.yuexingan06.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://na.szxytkj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zf.jianghongdianzi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pl.wgjwhj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lr.shxzskj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jc.bjjhwx.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gv.newstarts.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zc.huixiangedu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gw.haigaiapp.cn

[B11] 生成数字序列 / 区间
来源：http://wz.gzmigu.cn

Py:   list(range(0, 10, 2))
来源：http://xv.gzmigu.cn

PHP:  range(0, 10, 2);
来源：http://fr.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kp.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wi.521024.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bd.szsharing.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cc.gzmigu.cn

Ruby: (0...10).step(2).to_a
来源：http://gi.szsharing.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kx.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://wg.bjjhwx.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qv.wgjwhj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gj.nicolike.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pf.huanxung.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qe.9csxet.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kz.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jz.wgjwhj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hh.huixinmuqiang.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sc.jctech888.com.cn

[B13] 判断是否为数字
来源：http://ql.shxzukj.cn

Py:   isinstance(x, (int, float))
来源：http://au.bookmarksfly.cn

PHP:  is_numeric($x)
来源：http://xo.jianghongdianzi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ob.huanxung.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bi.newstarts.cn

Java: x instanceof Number
来源：http://mw.huanxung.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uw.colortex.cn

Ruby: x.is_a?(Numeric)
来源：http://lc.nszjky.cn

C#:   x is int or double or decimal
来源：http://wp.nicolike.cn

[B14] 判断值是否在集合内
来源：http://gd.huixiangedu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tl.yuntaijiaju.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jl.shtwfgs.cn

JS:   [1, 2, 3].includes(x)
来源：http://xb.muxihuayi.cn

TS:   [1, 2, 3].includes(x)
来源：http://tp.shxzskj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dv.szxytkj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://je.panjiajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ey.hnjuh.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ve.gzmigu.cn

[B15] 布尔运算与取反
来源：http://ej.gzmigu.cn

Py:   a and b or not c
来源：http://sb.yuntaijiaju.cn

PHP:  $a && $b || !$c
来源：http://xa.asd995.cn

JS:   a && b || !c
来源：http://lq.huanxung.cn

TS:   a && b || !c
来源：http://hx.jianghongdianzi.cn

Java: a && b || !c
来源：http://dy.bjjhwx.cn

Go:   a && b || !c
来源：http://et.shtwfgs.cn

Ruby: a && b || !c
来源：http://hh.521024.cn

C#:   a && b || !c
来源：http://jd.newstarts.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zr.chemitech.net.cn

Py:   if not data: return
来源：http://hy.nicolike.cn

PHP:  if (!$data) { return; }
来源：http://iz.bookmarksfly.cn

JS:   if (!data) return;
来源：http://em.asd995.cn

TS:   if (!data) return;
来源：http://jw.gzmigu.cn

Java: if (data == null) return;
来源：http://yn.shxzskj.cn

Go:   if data == nil { return }
来源：http://yv.huanxung.cn

Ruby: return if data.nil?
来源：http://qf.huanxung.cn

C#:   if (data == null) return;
来源：http://my.hahajie.cn

================================================================================
来源：http://xr.colortex.cn

C. 函数与作用域
来源：http://dg.jianghongdianzi.cn

================================================================================
来源：http://ha.huixiangedu.cn

[C01] 定义函数
来源：http://tu.hahajie.cn

Py:   def add(a, b): return a + b
来源：http://vo.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://db.szxytkj.cn

JS:   function add(a, b) { return a + b; }
来源：http://do.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jj.newstarts.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hr.lnxyls.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kv.jianghongdianzi.cn

Ruby: def add(a, b); a + b; end
来源：http://bn.newstarts.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://di.nicolike.cn

[C02] 默认参数
来源：http://eg.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://gb.shtwfgs.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gi.9csxet.cn

JS:   function greet(name = "World") { return name; }
来源：http://zv.shxzskj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jf.nicolike.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kt.hnjuh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://et.chemitech.net.cn

Ruby: def greet(name = "World") = name
来源：http://nh.bjjhwx.cn

C#:   string Greet(string name = "World") => name;
来源：http://rq.shtwfgs.cn

[C03] 可变参数
来源：http://qr.chemitech.net.cn

Py:   def total(*args): return sum(args)
来源：http://xz.shtwfgs.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kd.szsharing.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://is.nszjky.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ad.lnxyls.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dd.9csxet.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://py.nicolike.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kg.9csxet.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ce.shtwfgs.cn

[C04] 命名参数 / 关键字参数
来源：http://ab.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ks.yuexingan06.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zo.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vc.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://al.szsharing.cn

Java: // 无：用 Builder 模式或 record
来源：http://di.bookmarksfly.cn

Go:   // 无：用配置结构体参数
来源：http://ia.panjiajie.cn

Ruby: f(a: 1, b: 2)
来源：http://fa.szxytkj.cn

C#:   f(a: 1, b: 2)
来源：http://ip.yuntaijiaju.cn

[C05] 返回多个值
来源：http://uj.bjjhwx.cn

Py:   return a, b
来源：http://ej.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://fo.bookmarksfly.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cp.shtwfgs.cn

TS:   return { a, b };
来源：http://go.bookmarksfly.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wj.wgjwhj.cn

Go:   return a, b
来源：http://me.panjiajie.cn

Ruby: return a, b
来源：http://ku.chemitech.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://hh.gzmigu.cn

[C06] 匿名函数 / lambda
来源：http://cb.huixinmuqiang.cn

Py:   square = lambda x: x * x
来源：http://yb.shtwfgs.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wv.shxzukj.cn

JS:   const square = x => x * x;
来源：http://do.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://za.haigaiapp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yr.nicolike.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ne.szsharing.cn

Ruby: square = ->(x) { x * x }
来源：http://ca.521024.cn

C#:   Func<int, int> square = x => x * x;
来源：http://nf.yuexingan06.cn

[C07] 把函数作为参数传入
来源：http://fu.shxzskj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tz.szxytkj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://uv.szxytkj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xm.hnjuh.cn

TS:   arr.map(String)
来源：http://ol.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rc.szxytkj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cx.nicolike.cn

Ruby: arr.map(&:upcase)
来源：http://zs.haigaiapp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://et.huixiangedu.cn

[C08] 闭包
来源：http://ry.bookmarksfly.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vl.asd995.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://he.bjjhwx.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://eq.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vt.newstarts.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qp.chemitech.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://se.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dd.bjjhwx.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oj.yuntaijiaju.cn

[C09] 递归
来源：http://ch.szsharing.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rv.yuexingan06.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sz.asd995.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yn.gzmigu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dp.bookmarksfly.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zy.huanxung.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ti.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nr.huanxung.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ob.jianghongdianzi.cn

[C10] 变量作用域
来源：http://pq.wgjwhj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ih.huixiangedu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fv.huixiangedu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ko.haigaiapp.cn


<!-- 参考信息 -->