代发 wailian999

C#:   (int)'A'; (char)65
来源：http://mv.huixiangedu.cn

[A19] 交换两个变量
来源：http://fz.yuexingan06.cn

Py:   a, b = b, a
来源：http://ae.szsharing.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yx.hahajie.cn

JS:   [a, b] = [b, a];
来源：http://sj.yuexingan06.cn

TS:   [a, b] = [b, a];
来源：http://bz.bookmarksfly.cn

Java: int t = a; a = b; b = t;
来源：http://yv.9csxet.cn

Go:   a, b = b, a
来源：http://bv.colortex.cn

Ruby: a, b = b, a
来源：http://ok.colortex.cn

C#:   (a, b) = (b, a);
来源：http://kq.panjiajie.cn

[A20] 读取标准输入
来源：http://cl.jctech888.com.cn

Py:   name = input("请输入：")
来源：http://pq.huanxung.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://kz.szsharing.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rw.colortex.cn

TS:   // Node.js：readline 模块
来源：http://kr.9csxet.cn

Java: new Scanner(System.in).nextLine()
来源：http://nk.shxzskj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qp.nicolike.cn

Ruby: gets.chomp
来源：http://kc.521024.cn

C#:   Console.ReadLine();
来源：http://ur.colortex.cn

[A21] 保留指定小数位输出
来源：http://rb.szxytkj.cn

Py:   f"{3.14159:.2f}"
来源：http://oi.jianghongdianzi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://sp.nicolike.cn

JS:   (3.14159).toFixed(2)
来源：http://jb.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://oc.yuntaijiaju.cn

Java: String.format("%.2f", 3.14159)
来源：http://xk.hahajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rt.jctech888.com.cn

Ruby: format("%.2f", 3.14159)
来源：http://so.newstarts.cn

C#:   3.14159.ToString("F2")
来源：http://xd.shtwfgs.cn

[A22] 获取字符串长度
来源：http://bs.haigaiapp.cn

Py:   len(s)
来源：http://oh.szxytkj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zt.huanxung.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hs.huixinmuqiang.cn

TS:   s.length
来源：http://mr.lnxyls.cn

Java: s.length()
来源：http://tm.hnjuh.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ow.bjjhwx.cn

Ruby: s.length
来源：http://zd.gzmigu.cn

C#:   s.Length
来源：http://zl.9csxet.cn

[A23] 大小写转换
来源：http://ap.bjjhwx.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://le.shxzukj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://av.9csxet.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cy.bjjhwx.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fy.bjjhwx.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gb.huanxung.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qq.nicolike.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ma.haigaiapp.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rd.yuntaijiaju.cn

[A24] 去除首尾空白
来源：http://nm.asd995.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tj.jianghongdianzi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jb.jianghongdianzi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iu.wgjwhj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://en.bjjhwx.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ux.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://cj.asd995.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qw.huixinmuqiang.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bc.9csxet.cn

[A25] 字符串比较
来源：http://pk.shxzukj.cn

Py:   s1 == s2; s1 != s2
来源：http://pe.colortex.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vc.gzmigu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ae.szsharing.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://th.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://eg.panjiajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yz.hnjuh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nd.bookmarksfly.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uz.newstarts.cn

[A26] 类型转换总览
来源：http://zf.huanxung.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gu.colortex.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hc.colortex.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hj.nszjky.cn

TS:   Number() String() Boolean() x as number
来源：http://ry.lnxyls.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nk.huixinmuqiang.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gi.jianghongdianzi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bq.panjiajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uq.colortex.cn

================================================================================
来源：http://fl.nicolike.cn

B. 流程控制
来源：http://xb.lnxyls.cn

================================================================================
来源：http://sj.gzmigu.cn

[B01] 条件判断 if / else
来源：http://bj.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mk.szxytkj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ij.lnxyls.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hk.shtwfgs.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ie.muxihuayi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fx.bjjhwx.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://de.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cm.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bq.asd995.cn

[B02] 多分支 else if / elif
来源：http://yj.nszjky.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yf.colortex.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cc.lnxyls.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gy.haigaiapp.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wi.huixiangedu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qg.9csxet.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ka.chemitech.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fg.asd995.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bd.huixiangedu.cn

[B03] switch / match / case
来源：http://hc.wgjwhj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sn.lnxyls.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nt.newstarts.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ff.lnxyls.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yv.hnjuh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qj.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://at.huanxung.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sq.szsharing.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fd.colortex.cn

[B04] for 计数循环
来源：http://ln.chemitech.net.cn

Py:   for i in range(10): print(i)
来源：http://bf.yuexingan06.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hn.panjiajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ue.huixinmuqiang.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dy.gzmigu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rh.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://my.newstarts.cn

Ruby: 10.times { |i| puts i }
来源：http://rk.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yj.lnxyls.cn

[B05] 遍历数组 / 列表
来源：http://so.jianghongdianzi.cn

Py:   for item in arr: print(item)
来源：http://so.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jf.panjiajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://px.gzmigu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rj.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wc.asd995.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://oa.chemitech.net.cn

Ruby: arr.each { |item| puts item }
来源：http://an.szxytkj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ue.nszjky.cn

[B06] 遍历字典 / 对象
来源：http://ni.lnxyls.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ik.haigaiapp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jw.bookmarksfly.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vy.shxzukj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ul.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xs.nszjky.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hy.haigaiapp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rr.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.jctech888.com.cn

[B07] while 循环
来源：http://dn.huixinmuqiang.cn

Py:   while i < 10: i += 1
来源：http://py.wgjwhj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gd.huanxung.cn

JS:   while (i < 10) { i++; }
来源：http://lt.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://vz.yuexingan06.cn

Java: while (i < 10) { i++; }
来源：http://vb.haigaiapp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nr.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://el.shxzukj.cn

C#:   while (i < 10) { i++; }
来源：http://jd.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://fz.9csxet.cn

Py:   # 无 do-while：用 while True + break
来源：http://oc.asd995.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dl.colortex.cn

JS:   do { i++; } while (i < 10);
来源：http://xk.bookmarksfly.cn

TS:   do { i++; } while (i < 10);
来源：http://ro.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://ab.jctech888.com.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rc.chemitech.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rh.shtwfgs.cn

C#:   do { i++; } while (i < 10);
来源：http://rm.wgjwhj.cn

[B09] break 与 continue
来源：http://uo.jianghongdianzi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xc.hahajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yr.521024.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qu.yuntaijiaju.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ny.hahajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lc.nicolike.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sl.gzmigu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ps.wgjwhj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xo.shtwfgs.cn

[B10] 遍历同时拿索引
来源：http://di.huanxung.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ts.bookmarksfly.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yg.colortex.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ab.yuntaijiaju.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fz.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hx.huixiangedu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ay.wgjwhj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vu.lnxyls.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qf.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://mf.521024.cn

Py:   list(range(0, 10, 2))
来源：http://sz.bjjhwx.cn

PHP:  range(0, 10, 2);
来源：http://qw.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lt.gzmigu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iw.newstarts.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://iw.muxihuayi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ic.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://bo.newstarts.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lt.haigaiapp.cn

[B12] 跳出多层循环
来源：http://lc.wgjwhj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ph.9csxet.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gt.bjjhwx.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wg.panjiajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ya.lnxyls.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ac.asd995.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cg.huanxung.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oj.yuntaijiaju.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cf.colortex.cn

[B13] 判断是否为数字
来源：http://xq.szxytkj.cn

Py:   isinstance(x, (int, float))
来源：http://yo.shtwfgs.cn

PHP:  is_numeric($x)
来源：http://ki.szxytkj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vu.huixinmuqiang.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xb.jianghongdianzi.cn

Java: x instanceof Number
来源：http://ff.muxihuayi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jp.hahajie.cn

Ruby: x.is_a?(Numeric)
来源：http://yw.wgjwhj.cn

C#:   x is int or double or decimal
来源：http://tr.9csxet.cn

[B14] 判断值是否在集合内
来源：http://ru.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pw.asd995.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ob.asd995.cn

JS:   [1, 2, 3].includes(x)
来源：http://pb.shxzukj.cn

TS:   [1, 2, 3].includes(x)
来源：http://le.panjiajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rv.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ti.huixiangedu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ft.haigaiapp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rg.yuexingan06.cn

[B15] 布尔运算与取反
来源：http://jq.asd995.cn

Py:   a and b or not c
来源：http://ja.yuexingan06.cn

PHP:  $a && $b || !$c
来源：http://vj.9csxet.cn

JS:   a && b || !c
来源：http://fu.shxzskj.cn

TS:   a && b || !c
来源：http://so.wgjwhj.cn

Java: a && b || !c
来源：http://vc.nszjky.cn

Go:   a && b || !c
来源：http://lx.asd995.cn

Ruby: a && b || !c
来源：http://mt.shtwfgs.cn

C#:   a && b || !c
来源：http://ci.haigaiapp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jz.szsharing.cn

Py:   if not data: return
来源：http://eu.colortex.cn

PHP:  if (!$data) { return; }
来源：http://fl.shxzukj.cn

JS:   if (!data) return;
来源：http://jh.panjiajie.cn

TS:   if (!data) return;
来源：http://nt.bjjhwx.cn

Java: if (data == null) return;
来源：http://af.bjjhwx.cn

Go:   if data == nil { return }
来源：http://mq.yuexingan06.cn

Ruby: return if data.nil?
来源：http://lr.chemitech.net.cn

C#:   if (data == null) return;
来源：http://fr.colortex.cn

================================================================================
来源：http://hl.newstarts.cn

C. 函数与作用域
来源：http://tn.yuexingan06.cn

================================================================================
来源：http://th.asd995.cn

[C01] 定义函数
来源：http://an.haigaiapp.cn

Py:   def add(a, b): return a + b
来源：http://ib.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pd.hnjuh.cn

JS:   function add(a, b) { return a + b; }
来源：http://lu.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://me.chemitech.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mw.nszjky.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vc.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://iw.9csxet.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fv.newstarts.cn

[C02] 默认参数
来源：http://ae.wgjwhj.cn

Py:   def greet(name="World"): return name
来源：http://jd.wgjwhj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hn.521024.cn

JS:   function greet(name = "World") { return name; }
来源：http://oy.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://he.bookmarksfly.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gm.wgjwhj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xc.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://vo.hahajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://je.asd995.cn

[C03] 可变参数
来源：http://ws.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://gp.gzmigu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ef.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://or.yuexingan06.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yy.shxzukj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ey.bookmarksfly.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qw.bookmarksfly.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hc.yuexingan06.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nb.jctech888.com.cn

[C04] 命名参数 / 关键字参数
来源：http://bg.hnjuh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bp.muxihuayi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gc.huixinmuqiang.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jp.9csxet.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ca.muxihuayi.cn

Java: // 无：用 Builder 模式或 record
来源：http://cd.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://ww.szxytkj.cn

Ruby: f(a: 1, b: 2)
来源：http://zu.panjiajie.cn

C#:   f(a: 1, b: 2)
来源：http://pp.szsharing.cn

[C05] 返回多个值
来源：http://pn.newstarts.cn

Py:   return a, b
来源：http://gc.szxytkj.cn

PHP:  return [$a, $b];
来源：http://fw.bjjhwx.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dp.521024.cn

TS:   return { a, b };
来源：http://to.huixinmuqiang.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://di.yuexingan06.cn

Go:   return a, b
来源：http://ug.9csxet.cn

Ruby: return a, b
来源：http://ly.shtwfgs.cn

C#:   return (a, b);              // ValueTuple
来源：http://rf.hnjuh.cn

[C06] 匿名函数 / lambda
来源：http://oi.huixiangedu.cn

Py:   square = lambda x: x * x
来源：http://kk.wgjwhj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gi.huixinmuqiang.cn

JS:   const square = x => x * x;
来源：http://xq.szsharing.cn

TS:   const square = (x: number): number => x * x;
来源：http://kh.9csxet.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yw.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jn.wgjwhj.cn

Ruby: square = ->(x) { x * x }
来源：http://lr.shxzskj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bo.9csxet.cn

[C07] 把函数作为参数传入
来源：http://wt.wgjwhj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ck.asd995.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xb.nicolike.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rf.lnxyls.cn

TS:   arr.map(String)
来源：http://ib.wgjwhj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://md.huixiangedu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ro.hnjuh.cn

Ruby: arr.map(&:upcase)
来源：http://ad.muxihuayi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ci.szsharing.cn

[C08] 闭包
来源：http://yn.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ip.chemitech.net.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://co.nszjky.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://aq.asd995.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ta.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ku.9csxet.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://at.muxihuayi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fs.yuexingan06.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yu.szxytkj.cn

[C09] 递归
来源：http://nz.asd995.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://er.muxihuayi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ww.jctech888.com.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ed.521024.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://va.shtwfgs.cn


<!-- 参考信息 -->