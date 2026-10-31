代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ds.chemitech.net.cn

Ruby: gets.chomp
来源：http://sa.jianghongdianzi.cn

C#:   Console.ReadLine();
来源：http://zm.nszjky.cn

[A21] 保留指定小数位输出
来源：http://qf.wgjwhj.cn

Py:   f"{3.14159:.2f}"
来源：http://ra.shxzukj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ix.shxzskj.cn

JS:   (3.14159).toFixed(2)
来源：http://hr.shxzskj.cn

TS:   (3.14159).toFixed(2)
来源：http://es.yuexingan06.cn

Java: String.format("%.2f", 3.14159)
来源：http://sd.shxzukj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bb.hahajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://pz.jianghongdianzi.cn

C#:   3.14159.ToString("F2")
来源：http://ia.521024.cn

[A22] 获取字符串长度
来源：http://xy.jianghongdianzi.cn

Py:   len(s)
来源：http://id.chemitech.net.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cr.shxzukj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dz.panjiajie.cn

TS:   s.length
来源：http://hk.huixiangedu.cn

Java: s.length()
来源：http://ai.hahajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ds.bookmarksfly.cn

Ruby: s.length
来源：http://rh.9csxet.cn

C#:   s.Length
来源：http://ge.shtwfgs.cn

[A23] 大小写转换
来源：http://za.szxytkj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vh.yuntaijiaju.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lv.jianghongdianzi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vq.chemitech.net.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xa.yuexingan06.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ad.nicolike.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dx.nszjky.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fq.colortex.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ri.asd995.cn

[A24] 去除首尾空白
来源：http://jk.521024.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vq.asd995.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hg.shtwfgs.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fc.jctech888.com.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rm.haigaiapp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mm.szxytkj.cn

Go:   strings.TrimSpace(s)
来源：http://xx.huanxung.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dy.szxytkj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yw.huixinmuqiang.cn

[A25] 字符串比较
来源：http://gy.huanxung.cn

Py:   s1 == s2; s1 != s2
来源：http://pm.szxytkj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ga.gzmigu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yi.shxzskj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xj.jianghongdianzi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xv.huixiangedu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ye.huanxung.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ds.hahajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ak.9csxet.cn

[A26] 类型转换总览
来源：http://ok.shxzskj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xz.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qo.hnjuh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ik.lnxyls.cn

TS:   Number() String() Boolean() x as number
来源：http://tr.shxzukj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cp.yuntaijiaju.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ft.nszjky.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://oa.gzmigu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jm.szxytkj.cn

================================================================================
来源：http://uz.panjiajie.cn

B. 流程控制
来源：http://wh.newstarts.cn

================================================================================
来源：http://ms.jianghongdianzi.cn

[B01] 条件判断 if / else
来源：http://db.panjiajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ub.yuexingan06.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nq.colortex.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wy.jctech888.com.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bd.jianghongdianzi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cs.newstarts.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://me.huixiangedu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gr.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ny.szsharing.cn

[B02] 多分支 else if / elif
来源：http://fw.colortex.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hd.yuexingan06.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://oi.gzmigu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wo.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fi.hnjuh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jg.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zu.szsharing.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fm.jianghongdianzi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qj.nicolike.cn

[B03] switch / match / case
来源：http://ti.colortex.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ir.nszjky.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://od.newstarts.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xk.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wg.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mn.yuexingan06.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ih.yuntaijiaju.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uu.haigaiapp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://at.huanxung.cn

[B04] for 计数循环
来源：http://sx.nszjky.cn

Py:   for i in range(10): print(i)
来源：http://jh.huanxung.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ad.wgjwhj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qx.asd995.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ht.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ic.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nw.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://qv.newstarts.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yk.bjjhwx.cn

[B05] 遍历数组 / 列表
来源：http://ob.bjjhwx.cn

Py:   for item in arr: print(item)
来源：http://fq.yuntaijiaju.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qz.huixiangedu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lt.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://os.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://aq.yuexingan06.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fl.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://ye.bookmarksfly.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://og.panjiajie.cn

[B06] 遍历字典 / 对象
来源：http://zg.yuntaijiaju.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qk.newstarts.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ah.panjiajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://os.hnjuh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xy.jianghongdianzi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oe.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://et.bookmarksfly.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tf.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xz.huixiangedu.cn

[B07] while 循环
来源：http://jw.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://pw.jctech888.com.cn

PHP:  while ($i < 10) { $i++; }
来源：http://we.huanxung.cn

JS:   while (i < 10) { i++; }
来源：http://te.muxihuayi.cn

TS:   while (i < 10) { i++; }
来源：http://aa.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://xk.bjjhwx.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zs.hahajie.cn

Ruby: while i < 10; i += 1; end
来源：http://os.newstarts.cn

C#:   while (i < 10) { i++; }
来源：http://uf.nicolike.cn

[B08] do-while（至少执行一次）
来源：http://eb.huanxung.cn

Py:   # 无 do-while：用 while True + break
来源：http://kv.9csxet.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://uf.bookmarksfly.cn

JS:   do { i++; } while (i < 10);
来源：http://vx.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://ec.yuntaijiaju.cn

Java: do { i++; } while (i < 10);
来源：http://uy.hahajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://uf.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mm.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://so.huanxung.cn

[B09] break 与 continue
来源：http://zb.panjiajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mn.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zn.yuexingan06.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ew.szxytkj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cl.gzmigu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://co.muxihuayi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ef.jctech888.com.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gj.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cx.asd995.cn

[B10] 遍历同时拿索引
来源：http://zj.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bb.asd995.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jd.gzmigu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hp.huanxung.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ik.huixiangedu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cd.521024.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fz.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dz.jianghongdianzi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rc.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://uj.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://si.szxytkj.cn

PHP:  range(0, 10, 2);
来源：http://de.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ag.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gu.huixinmuqiang.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cp.gzmigu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ug.haigaiapp.cn

Ruby: (0...10).step(2).to_a
来源：http://bp.haigaiapp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pg.nszjky.cn

[B12] 跳出多层循环
来源：http://wm.521024.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bx.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fh.shxzukj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sh.shxzukj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://id.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kh.huixiangedu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nn.yuntaijiaju.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lq.hahajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://of.newstarts.cn

[B13] 判断是否为数字
来源：http://mg.521024.cn

Py:   isinstance(x, (int, float))
来源：http://in.wgjwhj.cn

PHP:  is_numeric($x)
来源：http://hy.521024.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xx.newstarts.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ip.shxzskj.cn

Java: x instanceof Number
来源：http://ky.huanxung.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vn.panjiajie.cn

Ruby: x.is_a?(Numeric)
来源：http://cf.lnxyls.cn

C#:   x is int or double or decimal
来源：http://ji.hahajie.cn

[B14] 判断值是否在集合内
来源：http://jm.huixinmuqiang.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xg.chemitech.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ru.szxytkj.cn

JS:   [1, 2, 3].includes(x)
来源：http://fd.huixiangedu.cn

TS:   [1, 2, 3].includes(x)
来源：http://sz.haigaiapp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ki.szsharing.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sb.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gb.haigaiapp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yh.colortex.cn

[B15] 布尔运算与取反
来源：http://he.nicolike.cn

Py:   a and b or not c
来源：http://wg.521024.cn

PHP:  $a && $b || !$c
来源：http://ze.hnjuh.cn

JS:   a && b || !c
来源：http://ru.chemitech.net.cn

TS:   a && b || !c
来源：http://ly.yuexingan06.cn

Java: a && b || !c
来源：http://gc.szxytkj.cn

Go:   a && b || !c
来源：http://dv.bookmarksfly.cn

Ruby: a && b || !c
来源：http://vi.huixiangedu.cn

C#:   a && b || !c
来源：http://qx.szxytkj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pd.nszjky.cn

Py:   if not data: return
来源：http://ur.521024.cn

PHP:  if (!$data) { return; }
来源：http://bt.9csxet.cn

JS:   if (!data) return;
来源：http://mk.colortex.cn

TS:   if (!data) return;
来源：http://lf.panjiajie.cn

Java: if (data == null) return;
来源：http://ev.shxzskj.cn

Go:   if data == nil { return }
来源：http://xz.9csxet.cn

Ruby: return if data.nil?
来源：http://qv.gzmigu.cn

C#:   if (data == null) return;
来源：http://oy.9csxet.cn

================================================================================
来源：http://uo.panjiajie.cn

C. 函数与作用域
来源：http://qh.nicolike.cn

================================================================================
来源：http://mr.panjiajie.cn

[C01] 定义函数
来源：http://na.muxihuayi.cn

Py:   def add(a, b): return a + b
来源：http://tp.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xc.szsharing.cn

JS:   function add(a, b) { return a + b; }
来源：http://ul.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mq.lnxyls.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://uw.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://do.chemitech.net.cn

Ruby: def add(a, b); a + b; end
来源：http://xm.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zz.9csxet.cn

[C02] 默认参数
来源：http://di.gzmigu.cn

Py:   def greet(name="World"): return name
来源：http://qr.9csxet.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jw.colortex.cn

JS:   function greet(name = "World") { return name; }
来源：http://wa.jianghongdianzi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hp.shtwfgs.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rj.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gw.hahajie.cn

Ruby: def greet(name = "World") = name
来源：http://ae.nszjky.cn

C#:   string Greet(string name = "World") => name;
来源：http://fr.newstarts.cn

[C03] 可变参数
来源：http://gg.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://bs.newstarts.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://og.9csxet.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://un.gzmigu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kp.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wb.gzmigu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vh.lnxyls.cn

Ruby: def total(*nums); nums.sum; end
来源：http://sw.lnxyls.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tx.9csxet.cn

[C04] 命名参数 / 关键字参数
来源：http://dn.nszjky.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://at.jianghongdianzi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mt.nicolike.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qj.panjiajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://or.huixinmuqiang.cn

Java: // 无：用 Builder 模式或 record
来源：http://mj.wgjwhj.cn

Go:   // 无：用配置结构体参数
来源：http://aj.szsharing.cn

Ruby: f(a: 1, b: 2)
来源：http://ze.colortex.cn

C#:   f(a: 1, b: 2)
来源：http://nb.9csxet.cn

[C05] 返回多个值
来源：http://ss.521024.cn

Py:   return a, b
来源：http://vh.panjiajie.cn

PHP:  return [$a, $b];
来源：http://mf.wgjwhj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://oq.gzmigu.cn

TS:   return { a, b };
来源：http://hf.panjiajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://se.gzmigu.cn

Go:   return a, b
来源：http://uc.szxytkj.cn

Ruby: return a, b
来源：http://wf.jctech888.com.cn

C#:   return (a, b);              // ValueTuple
来源：http://oa.bjjhwx.cn

[C06] 匿名函数 / lambda
来源：http://nv.huixiangedu.cn

Py:   square = lambda x: x * x
来源：http://nb.yuexingan06.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wz.nszjky.cn

JS:   const square = x => x * x;
来源：http://bm.bjjhwx.cn

TS:   const square = (x: number): number => x * x;
来源：http://wa.wgjwhj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://km.haigaiapp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://sq.nicolike.cn

Ruby: square = ->(x) { x * x }
来源：http://ro.muxihuayi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jj.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://vt.szxytkj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cw.shtwfgs.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jg.nszjky.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gy.9csxet.cn

TS:   arr.map(String)
来源：http://na.shxzukj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qa.wgjwhj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://io.huixinmuqiang.cn

Ruby: arr.map(&:upcase)
来源：http://vg.yuntaijiaju.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pa.huixinmuqiang.cn

[C08] 闭包
来源：http://gf.jianghongdianzi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ry.jctech888.com.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jf.521024.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xd.asd995.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jt.shxzskj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qe.asd995.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zd.muxihuayi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mm.gzmigu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kr.chemitech.net.cn

[C09] 递归
来源：http://hz.chemitech.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bp.jctech888.com.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xq.szxytkj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kf.huanxung.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rr.chemitech.net.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://du.newstarts.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gx.szsharing.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jv.nicolike.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ae.shxzukj.cn

[C10] 变量作用域
来源：http://si.newstarts.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://au.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://um.521024.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xv.shxzukj.cn

TS:   同 JS
来源：http://yv.nicolike.cn

Java: 方法内为块级作用域
来源：http://sh.shxzukj.cn

Go:   花括号块级作用域
来源：http://jv.nicolike.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ke.nicolike.cn

C#:   块级作用域
来源：http://zp.shxzskj.cn

[C11] 模块导入与导出
来源：http://at.yuntaijiaju.cn

Py:   from module import func
来源：http://vu.szxytkj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ui.muxihuayi.cn


<!-- 参考信息 -->