代发 wailian999

JS:   [a, b] = [b, a];
来源：http://vf.haigaiapp.cn

TS:   [a, b] = [b, a];
来源：http://vj.lnxyls.cn

Java: int t = a; a = b; b = t;
来源：http://jx.huixinmuqiang.cn

Go:   a, b = b, a
来源：http://xy.yuntaijiaju.cn

Ruby: a, b = b, a
来源：http://kq.wgjwhj.cn

C#:   (a, b) = (b, a);
来源：http://tw.newstarts.cn

[A20] 读取标准输入
来源：http://xn.jctech888.com.cn

Py:   name = input("请输入：")
来源：http://ps.szxytkj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rp.hahajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hj.nszjky.cn

TS:   // Node.js：readline 模块
来源：http://qt.shtwfgs.cn

Java: new Scanner(System.in).nextLine()
来源：http://dc.huixinmuqiang.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dm.lnxyls.cn

Ruby: gets.chomp
来源：http://vk.wgjwhj.cn

C#:   Console.ReadLine();
来源：http://pn.wgjwhj.cn

[A21] 保留指定小数位输出
来源：http://fy.chemitech.net.cn

Py:   f"{3.14159:.2f}"
来源：http://fg.bjjhwx.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ci.shtwfgs.cn

JS:   (3.14159).toFixed(2)
来源：http://uy.yuexingan06.cn

TS:   (3.14159).toFixed(2)
来源：http://lb.jctech888.com.cn

Java: String.format("%.2f", 3.14159)
来源：http://qe.nicolike.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://eg.shtwfgs.cn

Ruby: format("%.2f", 3.14159)
来源：http://cm.huixiangedu.cn

C#:   3.14159.ToString("F2")
来源：http://qz.521024.cn

[A22] 获取字符串长度
来源：http://tv.huixiangedu.cn

Py:   len(s)
来源：http://ep.jctech888.com.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cy.yuexingan06.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gl.bjjhwx.cn

TS:   s.length
来源：http://ta.521024.cn

Java: s.length()
来源：http://ho.bjjhwx.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://di.shxzskj.cn

Ruby: s.length
来源：http://hk.huixiangedu.cn

C#:   s.Length
来源：http://fy.jianghongdianzi.cn

[A23] 大小写转换
来源：http://sa.bookmarksfly.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ys.nicolike.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gx.nicolike.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jx.haigaiapp.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ma.jianghongdianzi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dk.jctech888.com.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sb.szsharing.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nm.szxytkj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ky.huanxung.cn

[A24] 去除首尾空白
来源：http://lq.panjiajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rh.wgjwhj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fs.panjiajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ak.shxzukj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hv.521024.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nr.lnxyls.cn

Go:   strings.TrimSpace(s)
来源：http://hc.nszjky.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://my.huanxung.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ul.hnjuh.cn

[A25] 字符串比较
来源：http://ob.hnjuh.cn

Py:   s1 == s2; s1 != s2
来源：http://qs.yuexingan06.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cl.szxytkj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ja.asd995.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fc.szsharing.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yi.huixinmuqiang.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ie.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://iu.yuexingan06.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ie.shxzukj.cn

[A26] 类型转换总览
来源：http://ie.521024.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gr.521024.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zq.bookmarksfly.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://oq.huixiangedu.cn

TS:   Number() String() Boolean() x as number
来源：http://er.shtwfgs.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lx.newstarts.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://it.yuntaijiaju.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ki.newstarts.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nh.chemitech.net.cn

================================================================================
来源：http://on.jianghongdianzi.cn

B. 流程控制
来源：http://es.muxihuayi.cn

================================================================================
来源：http://rt.szxytkj.cn

[B01] 条件判断 if / else
来源：http://on.nszjky.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://td.bookmarksfly.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yz.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://np.shxzukj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kt.lnxyls.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rz.huixinmuqiang.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ou.huanxung.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pl.521024.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uk.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://eh.wgjwhj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jl.gzmigu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://us.jctech888.com.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://is.nszjky.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ep.shxzskj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wa.hnjuh.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ca.gzmigu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://up.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://et.chemitech.net.cn

[B03] switch / match / case
来源：http://hx.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cu.gzmigu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dk.asd995.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cv.lnxyls.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zh.asd995.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cy.bjjhwx.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ph.yuntaijiaju.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ba.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pn.shtwfgs.cn

[B04] for 计数循环
来源：http://tt.gzmigu.cn

Py:   for i in range(10): print(i)
来源：http://kn.hnjuh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hq.hnjuh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tx.bjjhwx.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eg.huixinmuqiang.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ar.haigaiapp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xo.yuexingan06.cn

Ruby: 10.times { |i| puts i }
来源：http://tz.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zh.shxzukj.cn

[B05] 遍历数组 / 列表
来源：http://wd.jianghongdianzi.cn

Py:   for item in arr: print(item)
来源：http://df.wgjwhj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sl.hnjuh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rt.hnjuh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ky.nszjky.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tl.huanxung.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vk.hnjuh.cn

Ruby: arr.each { |item| puts item }
来源：http://rj.wgjwhj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://re.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://ri.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ag.huixiangedu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vb.panjiajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dr.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wk.huanxung.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gl.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gs.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://at.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hu.nszjky.cn

[B07] while 循环
来源：http://zx.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://xy.yuexingan06.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mj.nszjky.cn

JS:   while (i < 10) { i++; }
来源：http://va.9csxet.cn

TS:   while (i < 10) { i++; }
来源：http://wm.shxzskj.cn

Java: while (i < 10) { i++; }
来源：http://vg.huanxung.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mb.yuntaijiaju.cn

Ruby: while i < 10; i += 1; end
来源：http://cd.newstarts.cn

C#:   while (i < 10) { i++; }
来源：http://gj.huanxung.cn

[B08] do-while（至少执行一次）
来源：http://zo.521024.cn

Py:   # 无 do-while：用 while True + break
来源：http://xz.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zc.colortex.cn

JS:   do { i++; } while (i < 10);
来源：http://ov.jianghongdianzi.cn

TS:   do { i++; } while (i < 10);
来源：http://oy.yuntaijiaju.cn

Java: do { i++; } while (i < 10);
来源：http://wt.jianghongdianzi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xa.szxytkj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://io.huixinmuqiang.cn

C#:   do { i++; } while (i < 10);
来源：http://sl.jianghongdianzi.cn

[B09] break 与 continue
来源：http://vt.muxihuayi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sg.colortex.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qu.muxihuayi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ax.shxzskj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cc.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://py.newstarts.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hw.newstarts.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ox.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lq.9csxet.cn

[B10] 遍历同时拿索引
来源：http://po.haigaiapp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cc.gzmigu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dw.nszjky.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tr.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sm.jianghongdianzi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://my.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://po.huixiangedu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ru.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zp.huixiangedu.cn

[B11] 生成数字序列 / 区间
来源：http://tr.bjjhwx.cn

Py:   list(range(0, 10, 2))
来源：http://cn.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://tg.huixiangedu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pl.wgjwhj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rc.shxzukj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ti.yuexingan06.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ga.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://do.newstarts.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fr.huanxung.cn

[B12] 跳出多层循环
来源：http://hy.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fv.yuntaijiaju.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://me.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tt.shtwfgs.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dj.huanxung.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hw.szsharing.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bk.hahajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lm.asd995.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kd.bjjhwx.cn

[B13] 判断是否为数字
来源：http://hj.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://at.colortex.cn

PHP:  is_numeric($x)
来源：http://jw.jctech888.com.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ds.yuntaijiaju.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ur.huixiangedu.cn

Java: x instanceof Number
来源：http://ad.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://un.colortex.cn

Ruby: x.is_a?(Numeric)
来源：http://fv.yuntaijiaju.cn

C#:   x is int or double or decimal
来源：http://ne.chemitech.net.cn

[B14] 判断值是否在集合内
来源：http://um.nicolike.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://et.yuexingan06.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ym.hnjuh.cn

JS:   [1, 2, 3].includes(x)
来源：http://hq.jianghongdianzi.cn

TS:   [1, 2, 3].includes(x)
来源：http://lg.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ur.lnxyls.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wo.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qm.huixinmuqiang.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uj.huanxung.cn

[B15] 布尔运算与取反
来源：http://pe.yuntaijiaju.cn

Py:   a and b or not c
来源：http://uy.bjjhwx.cn

PHP:  $a && $b || !$c
来源：http://tf.huanxung.cn

JS:   a && b || !c
来源：http://ay.yuntaijiaju.cn

TS:   a && b || !c
来源：http://vo.shxzskj.cn

Java: a && b || !c
来源：http://xs.newstarts.cn

Go:   a && b || !c
来源：http://dw.521024.cn

Ruby: a && b || !c
来源：http://wf.wgjwhj.cn

C#:   a && b || !c
来源：http://ck.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ia.chemitech.net.cn

Py:   if not data: return
来源：http://ys.jctech888.com.cn

PHP:  if (!$data) { return; }
来源：http://bh.9csxet.cn

JS:   if (!data) return;
来源：http://gy.szxytkj.cn

TS:   if (!data) return;
来源：http://wq.szxytkj.cn

Java: if (data == null) return;
来源：http://pq.newstarts.cn

Go:   if data == nil { return }
来源：http://sx.chemitech.net.cn

Ruby: return if data.nil?
来源：http://uc.gzmigu.cn

C#:   if (data == null) return;
来源：http://or.shtwfgs.cn

================================================================================
来源：http://hv.hahajie.cn

C. 函数与作用域
来源：http://wa.szsharing.cn

================================================================================
来源：http://ed.hahajie.cn

[C01] 定义函数
来源：http://hq.jianghongdianzi.cn

Py:   def add(a, b): return a + b
来源：http://rj.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rd.jctech888.com.cn

JS:   function add(a, b) { return a + b; }
来源：http://mj.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cc.jctech888.com.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://or.huanxung.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rb.asd995.cn

Ruby: def add(a, b); a + b; end
来源：http://qa.colortex.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cz.huixiangedu.cn

[C02] 默认参数
来源：http://hw.wgjwhj.cn

Py:   def greet(name="World"): return name
来源：http://mk.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://li.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://kh.huanxung.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://kv.huanxung.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://eh.chemitech.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rb.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://ju.jianghongdianzi.cn

C#:   string Greet(string name = "World") => name;
来源：http://az.521024.cn

[C03] 可变参数
来源：http://ux.huanxung.cn

Py:   def total(*args): return sum(args)
来源：http://es.bjjhwx.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sa.szsharing.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sl.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pd.hahajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xp.bjjhwx.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pw.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ti.panjiajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://eu.asd995.cn

[C04] 命名参数 / 关键字参数
来源：http://ux.szxytkj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vp.huanxung.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zd.jianghongdianzi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vb.shxzukj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ii.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://ef.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://fs.521024.cn

Ruby: f(a: 1, b: 2)
来源：http://zj.panjiajie.cn

C#:   f(a: 1, b: 2)
来源：http://sq.yuntaijiaju.cn

[C05] 返回多个值
来源：http://by.shxzukj.cn

Py:   return a, b
来源：http://hw.haigaiapp.cn

PHP:  return [$a, $b];
来源：http://uw.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xr.bjjhwx.cn

TS:   return { a, b };
来源：http://yi.gzmigu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vm.muxihuayi.cn

Go:   return a, b
来源：http://je.shxzukj.cn

Ruby: return a, b
来源：http://pm.shxzskj.cn

C#:   return (a, b);              // ValueTuple
来源：http://ag.muxihuayi.cn

[C06] 匿名函数 / lambda
来源：http://et.nicolike.cn

Py:   square = lambda x: x * x
来源：http://ja.gzmigu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cc.shxzskj.cn

JS:   const square = x => x * x;
来源：http://dd.huixinmuqiang.cn

TS:   const square = (x: number): number => x * x;
来源：http://pi.shtwfgs.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uo.huixiangedu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dk.bookmarksfly.cn

Ruby: square = ->(x) { x * x }
来源：http://jd.lnxyls.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xa.bjjhwx.cn

[C07] 把函数作为参数传入
来源：http://sf.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pk.shxzukj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qq.shtwfgs.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sr.jctech888.com.cn

TS:   arr.map(String)
来源：http://gm.shtwfgs.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yy.newstarts.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hd.szxytkj.cn

Ruby: arr.map(&:upcase)
来源：http://gz.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kx.9csxet.cn

[C08] 闭包
来源：http://ex.wgjwhj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nh.shxzskj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zy.wgjwhj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://es.yuntaijiaju.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ro.yuexingan06.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pu.yuntaijiaju.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://er.asd995.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cc.colortex.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xi.asd995.cn

[C09] 递归
来源：http://dl.521024.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ef.muxihuayi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jr.gzmigu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ty.521024.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fy.huanxung.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ir.muxihuayi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qf.hahajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rw.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ak.hahajie.cn


<!-- 参考信息 -->