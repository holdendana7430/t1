代发 wailian999

JS:   [a, b] = [b, a];
来源：http://wa.asd995.cn

TS:   [a, b] = [b, a];
来源：http://nc.haigaiapp.cn

Java: int t = a; a = b; b = t;
来源：http://rv.colortex.cn

Go:   a, b = b, a
来源：http://kb.huixiangedu.cn

Ruby: a, b = b, a
来源：http://gf.gzmigu.cn

C#:   (a, b) = (b, a);
来源：http://hj.9csxet.cn

[A20] 读取标准输入
来源：http://ca.haigaiapp.cn

Py:   name = input("请输入：")
来源：http://yr.colortex.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ms.shtwfgs.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qp.muxihuayi.cn

TS:   // Node.js：readline 模块
来源：http://sn.bjjhwx.cn

Java: new Scanner(System.in).nextLine()
来源：http://zo.huanxung.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xp.gzmigu.cn

Ruby: gets.chomp
来源：http://pl.hahajie.cn

C#:   Console.ReadLine();
来源：http://vv.szxytkj.cn

[A21] 保留指定小数位输出
来源：http://uw.hahajie.cn

Py:   f"{3.14159:.2f}"
来源：http://ch.shxzskj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lb.lnxyls.cn

JS:   (3.14159).toFixed(2)
来源：http://wd.wgjwhj.cn

TS:   (3.14159).toFixed(2)
来源：http://qp.colortex.cn

Java: String.format("%.2f", 3.14159)
来源：http://ff.521024.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wz.haigaiapp.cn

Ruby: format("%.2f", 3.14159)
来源：http://sk.huixinmuqiang.cn

C#:   3.14159.ToString("F2")
来源：http://oc.asd995.cn

[A22] 获取字符串长度
来源：http://gz.yuntaijiaju.cn

Py:   len(s)
来源：http://xe.huixinmuqiang.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ii.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://el.colortex.cn

TS:   s.length
来源：http://yk.szsharing.cn

Java: s.length()
来源：http://zc.hnjuh.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bp.huixiangedu.cn

Ruby: s.length
来源：http://ye.huixinmuqiang.cn

C#:   s.Length
来源：http://ih.yuntaijiaju.cn

[A23] 大小写转换
来源：http://uj.nicolike.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://sj.yuntaijiaju.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pt.nicolike.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vy.szxytkj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hb.nszjky.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gv.bjjhwx.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fe.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://av.bookmarksfly.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://yg.jianghongdianzi.cn

[A24] 去除首尾空白
来源：http://rd.bjjhwx.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hb.yuexingan06.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cc.gzmigu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pi.asd995.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fm.9csxet.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://aq.nszjky.cn

Go:   strings.TrimSpace(s)
来源：http://fm.shtwfgs.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ee.haigaiapp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ni.hnjuh.cn

[A25] 字符串比较
来源：http://ry.newstarts.cn

Py:   s1 == s2; s1 != s2
来源：http://rx.huanxung.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sb.gzmigu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ou.newstarts.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qm.shxzskj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xe.newstarts.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ml.huanxung.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://sd.chemitech.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://aa.yuexingan06.cn

[A26] 类型转换总览
来源：http://ve.gzmigu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://av.huixinmuqiang.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kk.szsharing.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ou.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://do.yuntaijiaju.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jl.nicolike.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hd.hahajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kl.gzmigu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mh.shtwfgs.cn

================================================================================
来源：http://fb.colortex.cn

B. 流程控制
来源：http://qp.shxzskj.cn

================================================================================
来源：http://if.shtwfgs.cn

[B01] 条件判断 if / else
来源：http://tr.wgjwhj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mq.huixiangedu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sx.shxzskj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yf.haigaiapp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kl.jctech888.com.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hv.wgjwhj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ye.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mf.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://od.haigaiapp.cn

[B02] 多分支 else if / elif
来源：http://pr.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ul.shtwfgs.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dp.huixinmuqiang.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hy.newstarts.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xa.huanxung.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pb.newstarts.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kd.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ex.nszjky.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fs.hnjuh.cn

[B03] switch / match / case
来源：http://jy.huanxung.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ld.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://td.panjiajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iw.jianghongdianzi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oq.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hx.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pk.huixiangedu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qw.shxzskj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gv.yuexingan06.cn

[B04] for 计数循环
来源：http://xa.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://bf.gzmigu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rl.colortex.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yt.nicolike.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://co.yuexingan06.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ne.yuexingan06.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pe.jianghongdianzi.cn

Ruby: 10.times { |i| puts i }
来源：http://fy.9csxet.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://el.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://xs.521024.cn

Py:   for item in arr: print(item)
来源：http://mj.521024.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sz.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qe.colortex.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qk.shtwfgs.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hv.huanxung.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lv.shtwfgs.cn

Ruby: arr.each { |item| puts item }
来源：http://xv.muxihuayi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://aa.9csxet.cn

[B06] 遍历字典 / 对象
来源：http://gf.yuexingan06.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mm.nicolike.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ut.wgjwhj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://el.nszjky.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ja.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://io.yuntaijiaju.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qe.haigaiapp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jm.huixiangedu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cb.huixiangedu.cn

[B07] while 循环
来源：http://lq.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://gn.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ww.chemitech.net.cn

JS:   while (i < 10) { i++; }
来源：http://fn.lnxyls.cn

TS:   while (i < 10) { i++; }
来源：http://nk.haigaiapp.cn

Java: while (i < 10) { i++; }
来源：http://er.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://of.shxzskj.cn

Ruby: while i < 10; i += 1; end
来源：http://mq.asd995.cn

C#:   while (i < 10) { i++; }
来源：http://my.nicolike.cn

[B08] do-while（至少执行一次）
来源：http://uf.huanxung.cn

Py:   # 无 do-while：用 while True + break
来源：http://xx.yuexingan06.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://lf.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://cp.newstarts.cn

TS:   do { i++; } while (i < 10);
来源：http://et.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://it.haigaiapp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://eu.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yr.newstarts.cn

C#:   do { i++; } while (i < 10);
来源：http://on.hahajie.cn

[B09] break 与 continue
来源：http://re.yuntaijiaju.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gp.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://el.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nz.huixiangedu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hq.muxihuayi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ye.nicolike.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vd.521024.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bz.huixinmuqiang.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://af.gzmigu.cn

[B10] 遍历同时拿索引
来源：http://uq.yuntaijiaju.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ax.szxytkj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://im.nszjky.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yx.szsharing.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fi.chemitech.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pe.gzmigu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sb.hahajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ev.lnxyls.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dy.colortex.cn

[B11] 生成数字序列 / 区间
来源：http://up.jctech888.com.cn

Py:   list(range(0, 10, 2))
来源：http://jw.haigaiapp.cn

PHP:  range(0, 10, 2);
来源：http://dv.521024.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fv.newstarts.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nw.colortex.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fe.jianghongdianzi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://os.asd995.cn

Ruby: (0...10).step(2).to_a
来源：http://pg.shxzskj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dk.szxytkj.cn

[B12] 跳出多层循环
来源：http://ol.szsharing.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ji.newstarts.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gv.gzmigu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fo.bjjhwx.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vt.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xl.chemitech.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zc.huixiangedu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://st.jianghongdianzi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ex.bjjhwx.cn

[B13] 判断是否为数字
来源：http://qz.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://vv.521024.cn

PHP:  is_numeric($x)
来源：http://xi.shxzskj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ge.nszjky.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oo.shtwfgs.cn

Java: x instanceof Number
来源：http://yc.szxytkj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kh.newstarts.cn

Ruby: x.is_a?(Numeric)
来源：http://sl.huixinmuqiang.cn

C#:   x is int or double or decimal
来源：http://ew.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://cm.newstarts.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hi.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gv.521024.cn

JS:   [1, 2, 3].includes(x)
来源：http://ze.bjjhwx.cn

TS:   [1, 2, 3].includes(x)
来源：http://gz.muxihuayi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ne.szxytkj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://da.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yc.haigaiapp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://du.wgjwhj.cn

[B15] 布尔运算与取反
来源：http://rk.yuexingan06.cn

Py:   a and b or not c
来源：http://va.colortex.cn

PHP:  $a && $b || !$c
来源：http://oa.newstarts.cn

JS:   a && b || !c
来源：http://gb.yuexingan06.cn

TS:   a && b || !c
来源：http://ud.huixiangedu.cn

Java: a && b || !c
来源：http://kx.hnjuh.cn

Go:   a && b || !c
来源：http://xc.bookmarksfly.cn

Ruby: a && b || !c
来源：http://ic.shxzskj.cn

C#:   a && b || !c
来源：http://ja.hnjuh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lp.jctech888.com.cn

Py:   if not data: return
来源：http://zj.nicolike.cn

PHP:  if (!$data) { return; }
来源：http://jf.jianghongdianzi.cn

JS:   if (!data) return;
来源：http://sx.jctech888.com.cn

TS:   if (!data) return;
来源：http://to.shxzskj.cn

Java: if (data == null) return;
来源：http://mh.bookmarksfly.cn

Go:   if data == nil { return }
来源：http://gh.nszjky.cn

Ruby: return if data.nil?
来源：http://qz.lnxyls.cn

C#:   if (data == null) return;
来源：http://te.9csxet.cn

================================================================================
来源：http://ex.newstarts.cn

C. 函数与作用域
来源：http://lk.szsharing.cn

================================================================================
来源：http://uo.szsharing.cn

[C01] 定义函数
来源：http://vl.shtwfgs.cn

Py:   def add(a, b): return a + b
来源：http://oo.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gj.nicolike.cn

JS:   function add(a, b) { return a + b; }
来源：http://df.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kp.muxihuayi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fv.colortex.cn

Go:   func add(a, b int) int { return a + b }
来源：http://en.szxytkj.cn

Ruby: def add(a, b); a + b; end
来源：http://kc.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ev.nicolike.cn

[C02] 默认参数
来源：http://uk.hahajie.cn

Py:   def greet(name="World"): return name
来源：http://bn.jianghongdianzi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vw.bjjhwx.cn

JS:   function greet(name = "World") { return name; }
来源：http://bu.jctech888.com.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yb.huanxung.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ng.lnxyls.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ew.yuexingan06.cn

Ruby: def greet(name = "World") = name
来源：http://iy.panjiajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://im.huanxung.cn

[C03] 可变参数
来源：http://wn.lnxyls.cn

Py:   def total(*args): return sum(args)
来源：http://nf.hahajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gw.colortex.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nw.yuntaijiaju.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qp.muxihuayi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zf.jctech888.com.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://by.gzmigu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://dn.haigaiapp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ig.bjjhwx.cn

[C04] 命名参数 / 关键字参数
来源：http://ea.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mr.shtwfgs.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kp.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sf.szsharing.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hh.jianghongdianzi.cn

Java: // 无：用 Builder 模式或 record
来源：http://uw.bookmarksfly.cn

Go:   // 无：用配置结构体参数
来源：http://tv.gzmigu.cn

Ruby: f(a: 1, b: 2)
来源：http://tm.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://pc.asd995.cn

[C05] 返回多个值
来源：http://ol.yuexingan06.cn

Py:   return a, b
来源：http://xi.yuexingan06.cn

PHP:  return [$a, $b];
来源：http://fp.asd995.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hn.9csxet.cn

TS:   return { a, b };
来源：http://yt.newstarts.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pp.hahajie.cn

Go:   return a, b
来源：http://lh.asd995.cn

Ruby: return a, b
来源：http://bc.shxzskj.cn

C#:   return (a, b);              // ValueTuple
来源：http://th.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://xr.shxzskj.cn

Py:   square = lambda x: x * x
来源：http://uh.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rl.jctech888.com.cn

JS:   const square = x => x * x;
来源：http://ie.521024.cn

TS:   const square = (x: number): number => x * x;
来源：http://kc.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oc.huixinmuqiang.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ue.lnxyls.cn

Ruby: square = ->(x) { x * x }
来源：http://ay.bookmarksfly.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yy.colortex.cn

[C07] 把函数作为参数传入
来源：http://xf.yuntaijiaju.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ql.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lq.jctech888.com.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ed.gzmigu.cn

TS:   arr.map(String)
来源：http://mr.jianghongdianzi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zw.haigaiapp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://op.yuexingan06.cn

Ruby: arr.map(&:upcase)
来源：http://wz.huixiangedu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xn.nicolike.cn

[C08] 闭包
来源：http://ky.521024.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xn.bjjhwx.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sx.szxytkj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ej.jctech888.com.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://he.wgjwhj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zk.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mw.wgjwhj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fx.yuntaijiaju.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ao.nicolike.cn

[C09] 递归
来源：http://ex.muxihuayi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wx.asd995.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xp.shtwfgs.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sp.huixiangedu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tz.bookmarksfly.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kv.asd995.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ah.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nw.asd995.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uf.huanxung.cn


<!-- 参考信息 -->