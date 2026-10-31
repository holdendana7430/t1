代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://tg.haigaiapp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hw.hnjuh.cn

TS:   // Node.js：readline 模块
来源：http://mt.huanxung.cn

Java: new Scanner(System.in).nextLine()
来源：http://kv.lnxyls.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ex.shxzukj.cn

Ruby: gets.chomp
来源：http://tw.huixiangedu.cn

C#:   Console.ReadLine();
来源：http://ta.9csxet.cn

[A21] 保留指定小数位输出
来源：http://aa.newstarts.cn

Py:   f"{3.14159:.2f}"
来源：http://yu.9csxet.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bo.nicolike.cn

JS:   (3.14159).toFixed(2)
来源：http://cy.jianghongdianzi.cn

TS:   (3.14159).toFixed(2)
来源：http://wh.hahajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://fx.jianghongdianzi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://oq.shxzukj.cn

Ruby: format("%.2f", 3.14159)
来源：http://cz.yuexingan06.cn

C#:   3.14159.ToString("F2")
来源：http://bm.asd995.cn

[A22] 获取字符串长度
来源：http://ct.hahajie.cn

Py:   len(s)
来源：http://vw.gzmigu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ty.yuntaijiaju.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://md.hnjuh.cn

TS:   s.length
来源：http://zo.asd995.cn

Java: s.length()
来源：http://yi.muxihuayi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wf.lnxyls.cn

Ruby: s.length
来源：http://zq.yuexingan06.cn

C#:   s.Length
来源：http://qy.shxzskj.cn

[A23] 大小写转换
来源：http://ab.gzmigu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gl.chemitech.net.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ul.chemitech.net.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://je.szsharing.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rx.gzmigu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ov.szxytkj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://te.chemitech.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kp.asd995.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ib.colortex.cn

[A24] 去除首尾空白
来源：http://zt.gzmigu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ve.muxihuayi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pr.chemitech.net.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cc.colortex.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://in.newstarts.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vj.shxzukj.cn

Go:   strings.TrimSpace(s)
来源：http://rj.huixiangedu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ba.nszjky.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://im.521024.cn

[A25] 字符串比较
来源：http://ry.asd995.cn

Py:   s1 == s2; s1 != s2
来源：http://qq.nicolike.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zl.huixiangedu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zy.huanxung.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rh.newstarts.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nh.asd995.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jt.shxzukj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mz.colortex.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vv.muxihuayi.cn

[A26] 类型转换总览
来源：http://qb.shxzskj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yo.newstarts.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mf.shtwfgs.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://js.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://el.huixiangedu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lo.shxzukj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nr.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vt.nszjky.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zz.muxihuayi.cn

================================================================================
来源：http://pn.nicolike.cn

B. 流程控制
来源：http://ty.szsharing.cn

================================================================================
来源：http://cf.shxzskj.cn

[B01] 条件判断 if / else
来源：http://ex.asd995.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lb.gzmigu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xw.haigaiapp.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mw.nicolike.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uj.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xn.huanxung.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bc.gzmigu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mq.muxihuayi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gd.chemitech.net.cn

[B02] 多分支 else if / elif
来源：http://jy.huixinmuqiang.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jd.szsharing.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ho.521024.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uv.hahajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vq.huanxung.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mk.asd995.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uf.colortex.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xv.asd995.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ka.9csxet.cn

[B03] switch / match / case
来源：http://qc.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rv.shxzukj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ip.muxihuayi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yy.muxihuayi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zv.huixiangedu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://iw.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fa.szxytkj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lf.shtwfgs.cn

[B04] for 计数循环
来源：http://tz.huixiangedu.cn

Py:   for i in range(10): print(i)
来源：http://hz.asd995.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ez.shxzukj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ax.huixinmuqiang.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gy.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gi.szxytkj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zd.lnxyls.cn

Ruby: 10.times { |i| puts i }
来源：http://zh.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dg.colortex.cn

[B05] 遍历数组 / 列表
来源：http://uj.9csxet.cn

Py:   for item in arr: print(item)
来源：http://ba.szsharing.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jp.jianghongdianzi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hn.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://je.lnxyls.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yl.muxihuayi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ws.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://wk.newstarts.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dh.huanxung.cn

[B06] 遍历字典 / 对象
来源：http://bb.asd995.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kd.szsharing.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ob.szxytkj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fg.hahajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iy.colortex.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://df.lnxyls.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xp.jctech888.com.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://py.shtwfgs.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zf.9csxet.cn

[B07] while 循环
来源：http://gu.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://se.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tz.jianghongdianzi.cn

JS:   while (i < 10) { i++; }
来源：http://wr.nszjky.cn

TS:   while (i < 10) { i++; }
来源：http://xi.huixiangedu.cn

Java: while (i < 10) { i++; }
来源：http://vb.newstarts.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nv.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://cy.nszjky.cn

C#:   while (i < 10) { i++; }
来源：http://qq.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://fg.chemitech.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://yh.shtwfgs.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://se.huixiangedu.cn

JS:   do { i++; } while (i < 10);
来源：http://kn.shtwfgs.cn

TS:   do { i++; } while (i < 10);
来源：http://cj.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://ae.9csxet.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ry.521024.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ys.521024.cn

C#:   do { i++; } while (i < 10);
来源：http://kt.huixinmuqiang.cn

[B09] break 与 continue
来源：http://xv.szsharing.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kl.jianghongdianzi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bw.hnjuh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vo.jianghongdianzi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ne.bookmarksfly.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wa.hahajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bj.szsharing.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bl.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ai.chemitech.net.cn

[B10] 遍历同时拿索引
来源：http://fx.haigaiapp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cr.asd995.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://md.lnxyls.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zd.521024.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ik.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uh.wgjwhj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bi.bjjhwx.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cr.lnxyls.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ki.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://yp.asd995.cn

Py:   list(range(0, 10, 2))
来源：http://am.szsharing.cn

PHP:  range(0, 10, 2);
来源：http://ce.gzmigu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ol.9csxet.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xf.panjiajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fi.jianghongdianzi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jb.chemitech.net.cn

Ruby: (0...10).step(2).to_a
来源：http://vi.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://us.yuntaijiaju.cn

[B12] 跳出多层循环
来源：http://bh.nicolike.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hl.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://du.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ld.gzmigu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mm.shtwfgs.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jp.chemitech.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jl.colortex.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vg.gzmigu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xt.colortex.cn

[B13] 判断是否为数字
来源：http://zg.szsharing.cn

Py:   isinstance(x, (int, float))
来源：http://eu.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://bj.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mj.panjiajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dm.nicolike.cn

Java: x instanceof Number
来源：http://at.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rw.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://lh.lnxyls.cn

C#:   x is int or double or decimal
来源：http://zf.shtwfgs.cn

[B14] 判断值是否在集合内
来源：http://mk.newstarts.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://du.asd995.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cz.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://nz.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://mn.shxzskj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ix.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uo.9csxet.cn

Ruby: [1, 2, 3].include?(x)
来源：http://et.nicolike.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oa.szsharing.cn

[B15] 布尔运算与取反
来源：http://zv.asd995.cn

Py:   a and b or not c
来源：http://pl.nicolike.cn

PHP:  $a && $b || !$c
来源：http://th.521024.cn

JS:   a && b || !c
来源：http://xi.szsharing.cn

TS:   a && b || !c
来源：http://vf.yuntaijiaju.cn

Java: a && b || !c
来源：http://te.yuexingan06.cn

Go:   a && b || !c
来源：http://ev.shtwfgs.cn

Ruby: a && b || !c
来源：http://nf.shxzukj.cn

C#:   a && b || !c
来源：http://zu.panjiajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ci.bjjhwx.cn

Py:   if not data: return
来源：http://il.muxihuayi.cn

PHP:  if (!$data) { return; }
来源：http://dh.huanxung.cn

JS:   if (!data) return;
来源：http://sv.colortex.cn

TS:   if (!data) return;
来源：http://sh.shxzskj.cn

Java: if (data == null) return;
来源：http://vs.szsharing.cn

Go:   if data == nil { return }
来源：http://ge.nszjky.cn

Ruby: return if data.nil?
来源：http://mn.huixiangedu.cn

C#:   if (data == null) return;
来源：http://ki.jctech888.com.cn

================================================================================
来源：http://lv.newstarts.cn

C. 函数与作用域
来源：http://as.lnxyls.cn

================================================================================
来源：http://jg.jianghongdianzi.cn

[C01] 定义函数
来源：http://wv.wgjwhj.cn

Py:   def add(a, b): return a + b
来源：http://tn.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fs.nicolike.cn

JS:   function add(a, b) { return a + b; }
来源：http://ik.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fr.bookmarksfly.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pt.chemitech.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ep.hahajie.cn

Ruby: def add(a, b); a + b; end
来源：http://qp.newstarts.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nu.jctech888.com.cn

[C02] 默认参数
来源：http://in.yuexingan06.cn

Py:   def greet(name="World"): return name
来源：http://so.jctech888.com.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lv.huanxung.cn

JS:   function greet(name = "World") { return name; }
来源：http://vf.newstarts.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ek.asd995.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ya.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rl.hahajie.cn

Ruby: def greet(name = "World") = name
来源：http://ak.jianghongdianzi.cn

C#:   string Greet(string name = "World") => name;
来源：http://wy.lnxyls.cn

[C03] 可变参数
来源：http://ik.bookmarksfly.cn

Py:   def total(*args): return sum(args)
来源：http://nz.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ml.nszjky.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://oh.asd995.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cg.jctech888.com.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hh.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ra.haigaiapp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://uc.panjiajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wt.lnxyls.cn

[C04] 命名参数 / 关键字参数
来源：http://cu.szxytkj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bs.bookmarksfly.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://td.nicolike.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lh.gzmigu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dj.nicolike.cn

Java: // 无：用 Builder 模式或 record
来源：http://fc.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://ql.wgjwhj.cn

Ruby: f(a: 1, b: 2)
来源：http://pp.shxzukj.cn

C#:   f(a: 1, b: 2)
来源：http://th.jianghongdianzi.cn

[C05] 返回多个值
来源：http://bk.asd995.cn

Py:   return a, b
来源：http://wj.shxzskj.cn

PHP:  return [$a, $b];
来源：http://oq.jctech888.com.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bn.shxzukj.cn

TS:   return { a, b };
来源：http://fn.jianghongdianzi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dg.jianghongdianzi.cn

Go:   return a, b
来源：http://av.gzmigu.cn

Ruby: return a, b
来源：http://uq.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://nb.huixinmuqiang.cn

[C06] 匿名函数 / lambda
来源：http://fv.nszjky.cn

Py:   square = lambda x: x * x
来源：http://gg.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://iw.hahajie.cn

JS:   const square = x => x * x;
来源：http://bq.shxzukj.cn

TS:   const square = (x: number): number => x * x;
来源：http://su.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xt.bookmarksfly.cn

Go:   sq := func(x int) int { return x * x }
来源：http://oj.muxihuayi.cn

Ruby: square = ->(x) { x * x }
来源：http://fh.hnjuh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qk.gzmigu.cn

[C07] 把函数作为参数传入
来源：http://fz.yuntaijiaju.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zd.hahajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qv.wgjwhj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vm.hnjuh.cn

TS:   arr.map(String)
来源：http://gk.huixiangedu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jw.shxzukj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ae.panjiajie.cn

Ruby: arr.map(&:upcase)
来源：http://sn.9csxet.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rz.haigaiapp.cn

[C08] 闭包
来源：http://mz.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ed.huixinmuqiang.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jn.panjiajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xl.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tp.huanxung.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ud.chemitech.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://re.521024.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yk.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://df.huanxung.cn

[C09] 递归
来源：http://nq.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ot.shxzskj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kr.asd995.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qs.huixinmuqiang.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oq.yuntaijiaju.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gw.hnjuh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eq.asd995.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ct.colortex.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nk.521024.cn

[C10] 变量作用域
来源：http://ch.chemitech.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vh.nicolike.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://he.colortex.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ht.muxihuayi.cn

TS:   同 JS
来源：http://wt.muxihuayi.cn

Java: 方法内为块级作用域
来源：http://xx.shxzskj.cn

Go:   花括号块级作用域
来源：http://dg.nszjky.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ix.chemitech.net.cn


<!-- 参考信息 -->