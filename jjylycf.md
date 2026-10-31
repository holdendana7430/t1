代发 wailian999

Ruby: a, b = b, a
来源：http://ew.521024.cn

C#:   (a, b) = (b, a);
来源：http://fm.colortex.cn

[A20] 读取标准输入
来源：http://wq.hnjuh.cn

Py:   name = input("请输入：")
来源：http://wz.hahajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://jr.yuntaijiaju.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xo.jctech888.com.cn

TS:   // Node.js：readline 模块
来源：http://vl.szsharing.cn

Java: new Scanner(System.in).nextLine()
来源：http://vk.hnjuh.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vl.panjiajie.cn

Ruby: gets.chomp
来源：http://ro.panjiajie.cn

C#:   Console.ReadLine();
来源：http://xw.yuntaijiaju.cn

[A21] 保留指定小数位输出
来源：http://hd.huixiangedu.cn

Py:   f"{3.14159:.2f}"
来源：http://me.huixiangedu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://eh.yuexingan06.cn

JS:   (3.14159).toFixed(2)
来源：http://jf.yuntaijiaju.cn

TS:   (3.14159).toFixed(2)
来源：http://wo.nicolike.cn

Java: String.format("%.2f", 3.14159)
来源：http://ot.haigaiapp.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dd.nicolike.cn

Ruby: format("%.2f", 3.14159)
来源：http://lc.szxytkj.cn

C#:   3.14159.ToString("F2")
来源：http://iu.jctech888.com.cn

[A22] 获取字符串长度
来源：http://qf.521024.cn

Py:   len(s)
来源：http://cj.shxzukj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mk.hnjuh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ne.shxzskj.cn

TS:   s.length
来源：http://df.newstarts.cn

Java: s.length()
来源：http://ay.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kh.yuntaijiaju.cn

Ruby: s.length
来源：http://cd.asd995.cn

C#:   s.Length
来源：http://yn.newstarts.cn

[A23] 大小写转换
来源：http://ve.huixiangedu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://uu.jianghongdianzi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kx.shtwfgs.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ob.bjjhwx.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://of.huixinmuqiang.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wm.szsharing.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nh.nszjky.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pa.nicolike.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qg.haigaiapp.cn

[A24] 去除首尾空白
来源：http://vz.huixinmuqiang.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wi.nicolike.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mj.shxzskj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://df.chemitech.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uf.shtwfgs.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ho.colortex.cn

Go:   strings.TrimSpace(s)
来源：http://ze.colortex.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dt.wgjwhj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ed.jianghongdianzi.cn

[A25] 字符串比较
来源：http://oc.nszjky.cn

Py:   s1 == s2; s1 != s2
来源：http://la.yuexingan06.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dr.asd995.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hg.haigaiapp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ii.colortex.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tp.muxihuayi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qx.jctech888.com.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xc.yuexingan06.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kt.jianghongdianzi.cn

[A26] 类型转换总览
来源：http://jl.yuntaijiaju.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uu.nicolike.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ei.colortex.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yz.panjiajie.cn

TS:   Number() String() Boolean() x as number
来源：http://sd.9csxet.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sn.lnxyls.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mb.huanxung.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://la.asd995.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ne.newstarts.cn

================================================================================
来源：http://lu.haigaiapp.cn

B. 流程控制
来源：http://be.wgjwhj.cn

================================================================================
来源：http://jp.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://ei.yuntaijiaju.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ed.chemitech.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jx.szsharing.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://po.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dv.asd995.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gd.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qw.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://po.szsharing.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://so.nszjky.cn

[B02] 多分支 else if / elif
来源：http://by.shxzukj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mx.lnxyls.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ym.nszjky.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://va.asd995.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bj.szxytkj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dd.nszjky.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://my.hahajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qb.gzmigu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qa.chemitech.net.cn

[B03] switch / match / case
来源：http://dw.nszjky.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yj.jianghongdianzi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ki.yuexingan06.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ez.colortex.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yo.huixiangedu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zb.colortex.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://db.yuntaijiaju.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xx.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fd.yuexingan06.cn

[B04] for 计数循环
来源：http://uo.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://bw.shtwfgs.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ny.shxzukj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zq.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ph.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nc.wgjwhj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jf.huixiangedu.cn

Ruby: 10.times { |i| puts i }
来源：http://kt.nszjky.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ea.szxytkj.cn

[B05] 遍历数组 / 列表
来源：http://zo.wgjwhj.cn

Py:   for item in arr: print(item)
来源：http://ej.wgjwhj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sc.hnjuh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dd.hahajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wi.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qj.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vb.szsharing.cn

Ruby: arr.each { |item| puts item }
来源：http://vs.huanxung.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://be.bjjhwx.cn

[B06] 遍历字典 / 对象
来源：http://ir.lnxyls.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://uv.huanxung.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ye.huanxung.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xg.521024.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oc.szxytkj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nc.huanxung.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lj.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kq.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cj.9csxet.cn

[B07] while 循环
来源：http://lv.yuntaijiaju.cn

Py:   while i < 10: i += 1
来源：http://kk.gzmigu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kv.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://lm.bookmarksfly.cn

TS:   while (i < 10) { i++; }
来源：http://re.gzmigu.cn

Java: while (i < 10) { i++; }
来源：http://tt.shtwfgs.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gw.haigaiapp.cn

Ruby: while i < 10; i += 1; end
来源：http://ji.jianghongdianzi.cn

C#:   while (i < 10) { i++; }
来源：http://we.colortex.cn

[B08] do-while（至少执行一次）
来源：http://cj.hahajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://yy.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yx.jianghongdianzi.cn

JS:   do { i++; } while (i < 10);
来源：http://tv.nicolike.cn

TS:   do { i++; } while (i < 10);
来源：http://kj.muxihuayi.cn

Java: do { i++; } while (i < 10);
来源：http://xg.521024.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gk.asd995.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pt.shtwfgs.cn

C#:   do { i++; } while (i < 10);
来源：http://ea.shxzukj.cn

[B09] break 与 continue
来源：http://sn.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://og.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zq.yuexingan06.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ei.bjjhwx.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hb.colortex.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kg.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hv.lnxyls.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mh.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://al.shxzukj.cn

[B10] 遍历同时拿索引
来源：http://gl.panjiajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rh.wgjwhj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://aj.yuexingan06.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://aj.lnxyls.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xn.chemitech.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rk.shxzskj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rw.panjiajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lp.9csxet.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://da.jianghongdianzi.cn

[B11] 生成数字序列 / 区间
来源：http://qx.huanxung.cn

Py:   list(range(0, 10, 2))
来源：http://fd.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://je.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jh.chemitech.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://is.szxytkj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dt.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ld.nszjky.cn

Ruby: (0...10).step(2).to_a
来源：http://jn.shxzskj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ha.jctech888.com.cn

[B12] 跳出多层循环
来源：http://nr.hahajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ab.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fj.gzmigu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://be.muxihuayi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tr.hahajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cw.hahajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xm.shxzskj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kp.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://od.lnxyls.cn

[B13] 判断是否为数字
来源：http://hm.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://nc.yuexingan06.cn

PHP:  is_numeric($x)
来源：http://dj.yuntaijiaju.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ow.haigaiapp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fc.gzmigu.cn

Java: x instanceof Number
来源：http://cn.shxzskj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bd.jianghongdianzi.cn

Ruby: x.is_a?(Numeric)
来源：http://un.wgjwhj.cn

C#:   x is int or double or decimal
来源：http://tt.shxzskj.cn

[B14] 判断值是否在集合内
来源：http://my.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qy.hnjuh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ds.panjiajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://av.colortex.cn

TS:   [1, 2, 3].includes(x)
来源：http://fl.wgjwhj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://go.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://io.nicolike.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ob.gzmigu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rd.jianghongdianzi.cn

[B15] 布尔运算与取反
来源：http://is.huixiangedu.cn

Py:   a and b or not c
来源：http://ln.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://ya.colortex.cn

JS:   a && b || !c
来源：http://zc.shtwfgs.cn

TS:   a && b || !c
来源：http://yx.hahajie.cn

Java: a && b || !c
来源：http://xb.huixinmuqiang.cn

Go:   a && b || !c
来源：http://si.jctech888.com.cn

Ruby: a && b || !c
来源：http://vi.yuntaijiaju.cn

C#:   a && b || !c
来源：http://mp.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://er.panjiajie.cn

Py:   if not data: return
来源：http://br.jctech888.com.cn

PHP:  if (!$data) { return; }
来源：http://wa.szsharing.cn

JS:   if (!data) return;
来源：http://gb.colortex.cn

TS:   if (!data) return;
来源：http://da.huixiangedu.cn

Java: if (data == null) return;
来源：http://pe.huixiangedu.cn

Go:   if data == nil { return }
来源：http://rv.chemitech.net.cn

Ruby: return if data.nil?
来源：http://rk.shtwfgs.cn

C#:   if (data == null) return;
来源：http://bz.521024.cn

================================================================================
来源：http://dg.jctech888.com.cn

C. 函数与作用域
来源：http://er.shxzukj.cn

================================================================================
来源：http://ep.szsharing.cn

[C01] 定义函数
来源：http://zp.chemitech.net.cn

Py:   def add(a, b): return a + b
来源：http://ps.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lh.shtwfgs.cn

JS:   function add(a, b) { return a + b; }
来源：http://im.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cn.jianghongdianzi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nt.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rz.shtwfgs.cn

Ruby: def add(a, b); a + b; end
来源：http://mh.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dd.panjiajie.cn

[C02] 默认参数
来源：http://ne.lnxyls.cn

Py:   def greet(name="World"): return name
来源：http://pg.wgjwhj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tm.shtwfgs.cn

JS:   function greet(name = "World") { return name; }
来源：http://ld.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vp.newstarts.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sf.9csxet.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kj.szxytkj.cn

Ruby: def greet(name = "World") = name
来源：http://wm.yuntaijiaju.cn

C#:   string Greet(string name = "World") => name;
来源：http://ac.shxzskj.cn

[C03] 可变参数
来源：http://ly.asd995.cn

Py:   def total(*args): return sum(args)
来源：http://ng.chemitech.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mm.asd995.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fp.huanxung.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mc.colortex.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sn.shxzukj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wn.haigaiapp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ay.jctech888.com.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qb.9csxet.cn

[C04] 命名参数 / 关键字参数
来源：http://hp.wgjwhj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yk.chemitech.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ze.muxihuayi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dh.bookmarksfly.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rb.szxytkj.cn

Java: // 无：用 Builder 模式或 record
来源：http://tx.chemitech.net.cn

Go:   // 无：用配置结构体参数
来源：http://ns.huixiangedu.cn

Ruby: f(a: 1, b: 2)
来源：http://yv.muxihuayi.cn

C#:   f(a: 1, b: 2)
来源：http://ce.panjiajie.cn

[C05] 返回多个值
来源：http://nb.szxytkj.cn

Py:   return a, b
来源：http://cq.muxihuayi.cn

PHP:  return [$a, $b];
来源：http://qn.shxzskj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://at.colortex.cn

TS:   return { a, b };
来源：http://lr.shtwfgs.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kt.bjjhwx.cn

Go:   return a, b
来源：http://xd.asd995.cn

Ruby: return a, b
来源：http://sb.bookmarksfly.cn

C#:   return (a, b);              // ValueTuple
来源：http://po.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://ac.shxzskj.cn

Py:   square = lambda x: x * x
来源：http://ow.hnjuh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://io.gzmigu.cn

JS:   const square = x => x * x;
来源：http://rs.gzmigu.cn

TS:   const square = (x: number): number => x * x;
来源：http://rq.bjjhwx.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qk.gzmigu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lv.huixinmuqiang.cn

Ruby: square = ->(x) { x * x }
来源：http://rr.panjiajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dc.szxytkj.cn

[C07] 把函数作为参数传入
来源：http://pp.lnxyls.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ie.shxzskj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cy.hnjuh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wk.nszjky.cn

TS:   arr.map(String)
来源：http://go.colortex.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zh.jctech888.com.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sy.hahajie.cn

Ruby: arr.map(&:upcase)
来源：http://wc.haigaiapp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qo.shxzskj.cn

[C08] 闭包
来源：http://kv.szxytkj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rd.521024.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jm.jctech888.com.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xr.shxzskj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xu.bookmarksfly.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xz.nicolike.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xx.shtwfgs.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yi.huixiangedu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ti.jianghongdianzi.cn

[C09] 递归
来源：http://pr.colortex.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://eg.chemitech.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://it.jianghongdianzi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pb.muxihuayi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jm.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vi.9csxet.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ll.chemitech.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zd.chemitech.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://te.shxzskj.cn

[C10] 变量作用域
来源：http://jj.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wx.wgjwhj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tj.panjiajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xl.shxzskj.cn


<!-- 参考信息 -->