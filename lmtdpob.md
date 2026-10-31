代发 wailian999

Ruby: a, b = b, a
来源：http://bi.bjjhwx.cn

C#:   (a, b) = (b, a);
来源：http://dr.nszjky.cn

[A20] 读取标准输入
来源：http://mz.chemitech.net.cn

Py:   name = input("请输入：")
来源：http://sd.haigaiapp.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://oj.haigaiapp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pm.521024.cn

TS:   // Node.js：readline 模块
来源：http://uk.nszjky.cn

Java: new Scanner(System.in).nextLine()
来源：http://sp.hahajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zm.9csxet.cn

Ruby: gets.chomp
来源：http://nj.newstarts.cn

C#:   Console.ReadLine();
来源：http://pm.colortex.cn

[A21] 保留指定小数位输出
来源：http://tk.yuntaijiaju.cn

Py:   f"{3.14159:.2f}"
来源：http://eh.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://az.shtwfgs.cn

JS:   (3.14159).toFixed(2)
来源：http://hg.newstarts.cn

TS:   (3.14159).toFixed(2)
来源：http://km.shtwfgs.cn

Java: String.format("%.2f", 3.14159)
来源：http://re.nicolike.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://in.jctech888.com.cn

Ruby: format("%.2f", 3.14159)
来源：http://by.bjjhwx.cn

C#:   3.14159.ToString("F2")
来源：http://rh.chemitech.net.cn

[A22] 获取字符串长度
来源：http://vv.shtwfgs.cn

Py:   len(s)
来源：http://ng.newstarts.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://te.hnjuh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mu.shxzukj.cn

TS:   s.length
来源：http://dj.szsharing.cn

Java: s.length()
来源：http://bt.chemitech.net.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bu.muxihuayi.cn

Ruby: s.length
来源：http://yr.lnxyls.cn

C#:   s.Length
来源：http://eg.shxzukj.cn

[A23] 大小写转换
来源：http://tq.panjiajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fr.hahajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://sq.colortex.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kk.newstarts.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://iw.muxihuayi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jm.haigaiapp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gq.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://eo.haigaiapp.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xp.chemitech.net.cn

[A24] 去除首尾空白
来源：http://wj.colortex.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vj.nszjky.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://db.gzmigu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ak.yuntaijiaju.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://am.lnxyls.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://og.jianghongdianzi.cn

Go:   strings.TrimSpace(s)
来源：http://ro.shxzukj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hh.huanxung.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://iy.yuntaijiaju.cn

[A25] 字符串比较
来源：http://iq.lnxyls.cn

Py:   s1 == s2; s1 != s2
来源：http://yq.colortex.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jp.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nc.muxihuayi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fm.chemitech.net.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sd.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://iy.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nq.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vw.huanxung.cn

[A26] 类型转换总览
来源：http://sn.bookmarksfly.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qm.nszjky.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dc.wgjwhj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rt.colortex.cn

TS:   Number() String() Boolean() x as number
来源：http://rt.newstarts.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fg.521024.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://om.bjjhwx.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ts.bjjhwx.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hx.huixiangedu.cn

================================================================================
来源：http://tw.haigaiapp.cn

B. 流程控制
来源：http://bk.bookmarksfly.cn

================================================================================
来源：http://sa.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://tk.nszjky.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zc.9csxet.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fn.bookmarksfly.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://do.bjjhwx.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oy.panjiajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://kx.gzmigu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://eg.521024.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://oi.yuexingan06.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gx.9csxet.cn

[B02] 多分支 else if / elif
来源：http://ma.shtwfgs.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gg.9csxet.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tu.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zn.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dz.szsharing.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uh.huixiangedu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kj.bjjhwx.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://oz.wgjwhj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.521024.cn

[B03] switch / match / case
来源：http://ct.huanxung.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ez.panjiajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dj.9csxet.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ks.jctech888.com.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kc.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nl.nszjky.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nl.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qc.asd995.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hj.nicolike.cn

[B04] for 计数循环
来源：http://ag.yuexingan06.cn

Py:   for i in range(10): print(i)
来源：http://zh.newstarts.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://if.szsharing.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ly.hnjuh.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ot.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rb.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fa.nszjky.cn

Ruby: 10.times { |i| puts i }
来源：http://qf.wgjwhj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gf.hnjuh.cn

[B05] 遍历数组 / 列表
来源：http://ef.yuntaijiaju.cn

Py:   for item in arr: print(item)
来源：http://nk.muxihuayi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xi.lnxyls.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rp.asd995.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mh.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zc.yuexingan06.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lr.panjiajie.cn

Ruby: arr.each { |item| puts item }
来源：http://vq.newstarts.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jy.panjiajie.cn

[B06] 遍历字典 / 对象
来源：http://ck.szxytkj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vu.gzmigu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ap.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lc.huixinmuqiang.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://im.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ke.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zx.haigaiapp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sf.panjiajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kk.chemitech.net.cn

[B07] while 循环
来源：http://lm.nszjky.cn

Py:   while i < 10: i += 1
来源：http://pi.9csxet.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qq.muxihuayi.cn

JS:   while (i < 10) { i++; }
来源：http://qb.9csxet.cn

TS:   while (i < 10) { i++; }
来源：http://sp.shxzskj.cn

Java: while (i < 10) { i++; }
来源：http://ae.szxytkj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://am.chemitech.net.cn

Ruby: while i < 10; i += 1; end
来源：http://ew.chemitech.net.cn

C#:   while (i < 10) { i++; }
来源：http://rv.chemitech.net.cn

[B08] do-while（至少执行一次）
来源：http://op.hnjuh.cn

Py:   # 无 do-while：用 while True + break
来源：http://ew.jianghongdianzi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://be.bookmarksfly.cn

JS:   do { i++; } while (i < 10);
来源：http://vs.szxytkj.cn

TS:   do { i++; } while (i < 10);
来源：http://ca.haigaiapp.cn

Java: do { i++; } while (i < 10);
来源：http://dl.szsharing.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vc.shtwfgs.cn

Ruby: begin; i += 1; end while i < 10
来源：http://iy.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://lf.wgjwhj.cn

[B09] break 与 continue
来源：http://bt.wgjwhj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qf.huixinmuqiang.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gb.nicolike.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eg.szsharing.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kr.colortex.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://is.shtwfgs.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ca.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gi.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ig.wgjwhj.cn

[B10] 遍历同时拿索引
来源：http://zq.bookmarksfly.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zq.shxzukj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://er.bjjhwx.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zw.yuexingan06.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hb.colortex.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kp.huixiangedu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yq.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ha.newstarts.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nw.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://lk.521024.cn

Py:   list(range(0, 10, 2))
来源：http://og.colortex.cn

PHP:  range(0, 10, 2);
来源：http://rj.muxihuayi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://md.521024.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rj.muxihuayi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zh.jctech888.com.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wh.hnjuh.cn

Ruby: (0...10).step(2).to_a
来源：http://uk.jctech888.com.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bq.9csxet.cn

[B12] 跳出多层循环
来源：http://xj.521024.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ai.szsharing.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://st.muxihuayi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qk.huanxung.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zl.bjjhwx.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ez.szsharing.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wh.newstarts.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mr.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sb.panjiajie.cn

[B13] 判断是否为数字
来源：http://qp.chemitech.net.cn

Py:   isinstance(x, (int, float))
来源：http://tx.shxzskj.cn

PHP:  is_numeric($x)
来源：http://vp.haigaiapp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iy.jctech888.com.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bk.huixiangedu.cn

Java: x instanceof Number
来源：http://sc.colortex.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xp.jctech888.com.cn

Ruby: x.is_a?(Numeric)
来源：http://wr.hnjuh.cn

C#:   x is int or double or decimal
来源：http://qy.newstarts.cn

[B14] 判断值是否在集合内
来源：http://cn.szsharing.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://au.panjiajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ge.huanxung.cn

JS:   [1, 2, 3].includes(x)
来源：http://qs.bjjhwx.cn

TS:   [1, 2, 3].includes(x)
来源：http://db.panjiajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qk.bjjhwx.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sn.jianghongdianzi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fm.hahajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ta.huixiangedu.cn

[B15] 布尔运算与取反
来源：http://gz.huanxung.cn

Py:   a and b or not c
来源：http://aj.szsharing.cn

PHP:  $a && $b || !$c
来源：http://ns.huixinmuqiang.cn

JS:   a && b || !c
来源：http://bs.wgjwhj.cn

TS:   a && b || !c
来源：http://bw.bjjhwx.cn

Java: a && b || !c
来源：http://vc.huanxung.cn

Go:   a && b || !c
来源：http://rk.gzmigu.cn

Ruby: a && b || !c
来源：http://aj.9csxet.cn

C#:   a && b || !c
来源：http://ls.muxihuayi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ts.szxytkj.cn

Py:   if not data: return
来源：http://as.haigaiapp.cn

PHP:  if (!$data) { return; }
来源：http://uo.bjjhwx.cn

JS:   if (!data) return;
来源：http://jc.bjjhwx.cn

TS:   if (!data) return;
来源：http://vu.9csxet.cn

Java: if (data == null) return;
来源：http://ck.shxzukj.cn

Go:   if data == nil { return }
来源：http://xm.nszjky.cn

Ruby: return if data.nil?
来源：http://gd.shxzskj.cn

C#:   if (data == null) return;
来源：http://qb.shxzukj.cn

================================================================================
来源：http://uj.panjiajie.cn

C. 函数与作用域
来源：http://fz.colortex.cn

================================================================================
来源：http://ob.nicolike.cn

[C01] 定义函数
来源：http://mc.lnxyls.cn

Py:   def add(a, b): return a + b
来源：http://oo.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tx.nicolike.cn

JS:   function add(a, b) { return a + b; }
来源：http://fi.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aw.hnjuh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://si.colortex.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gr.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://fm.huixiangedu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://eh.bookmarksfly.cn

[C02] 默认参数
来源：http://tm.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://vu.haigaiapp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nq.hahajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://ap.asd995.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://og.wgjwhj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://de.szsharing.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sw.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://tp.yuexingan06.cn

C#:   string Greet(string name = "World") => name;
来源：http://ro.hnjuh.cn

[C03] 可变参数
来源：http://cl.huanxung.cn

Py:   def total(*args): return sum(args)
来源：http://yq.huixinmuqiang.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ye.huixinmuqiang.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ip.chemitech.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://oa.muxihuayi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lf.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ej.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ae.yuexingan06.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wc.jianghongdianzi.cn

[C04] 命名参数 / 关键字参数
来源：http://re.szxytkj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sc.jianghongdianzi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qd.shxzukj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xm.colortex.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lw.shtwfgs.cn

Java: // 无：用 Builder 模式或 record
来源：http://or.lnxyls.cn

Go:   // 无：用配置结构体参数
来源：http://zk.521024.cn

Ruby: f(a: 1, b: 2)
来源：http://db.muxihuayi.cn

C#:   f(a: 1, b: 2)
来源：http://uu.lnxyls.cn

[C05] 返回多个值
来源：http://ar.szxytkj.cn

Py:   return a, b
来源：http://yi.colortex.cn

PHP:  return [$a, $b];
来源：http://ob.huixinmuqiang.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xv.bookmarksfly.cn

TS:   return { a, b };
来源：http://el.521024.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ul.shxzskj.cn

Go:   return a, b
来源：http://mo.bookmarksfly.cn

Ruby: return a, b
来源：http://cj.shtwfgs.cn

C#:   return (a, b);              // ValueTuple
来源：http://gw.lnxyls.cn

[C06] 匿名函数 / lambda
来源：http://mx.bjjhwx.cn

Py:   square = lambda x: x * x
来源：http://nc.hnjuh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tp.9csxet.cn

JS:   const square = x => x * x;
来源：http://yi.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://yn.huixinmuqiang.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jl.haigaiapp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://di.huixinmuqiang.cn

Ruby: square = ->(x) { x * x }
来源：http://wt.huixinmuqiang.cn

C#:   Func<int, int> square = x => x * x;
来源：http://no.panjiajie.cn

[C07] 把函数作为参数传入
来源：http://bj.gzmigu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yy.haigaiapp.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ym.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://su.hahajie.cn

TS:   arr.map(String)
来源：http://wo.bjjhwx.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pt.hahajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://su.nszjky.cn

Ruby: arr.map(&:upcase)
来源：http://pj.shxzskj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bm.chemitech.net.cn

[C08] 闭包
来源：http://if.jctech888.com.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kp.shxzskj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pc.shxzskj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ch.lnxyls.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nh.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dk.szsharing.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oj.shxzskj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bg.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qk.bjjhwx.cn

[C09] 递归
来源：http://gd.gzmigu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://be.9csxet.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zb.gzmigu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tr.hnjuh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sa.hahajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xr.lnxyls.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ac.newstarts.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ap.521024.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uy.yuntaijiaju.cn

[C10] 变量作用域
来源：http://ke.muxihuayi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mb.colortex.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vy.521024.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hh.bjjhwx.cn


<!-- 参考信息 -->