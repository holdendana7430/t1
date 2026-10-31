代发 wailian999

JS:   [a, b] = [b, a];
来源：http://xq.szxytkj.cn

TS:   [a, b] = [b, a];
来源：http://uv.szsharing.cn

Java: int t = a; a = b; b = t;
来源：http://zx.haigaiapp.cn

Go:   a, b = b, a
来源：http://ru.shxzskj.cn

Ruby: a, b = b, a
来源：http://dh.wgjwhj.cn

C#:   (a, b) = (b, a);
来源：http://gy.bjjhwx.cn

[A20] 读取标准输入
来源：http://og.wgjwhj.cn

Py:   name = input("请输入：")
来源：http://ss.jctech888.com.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://bl.gzmigu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://uf.szxytkj.cn

TS:   // Node.js：readline 模块
来源：http://nd.huanxung.cn

Java: new Scanner(System.in).nextLine()
来源：http://yq.huanxung.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fx.hahajie.cn

Ruby: gets.chomp
来源：http://mb.shxzukj.cn

C#:   Console.ReadLine();
来源：http://qm.shtwfgs.cn

[A21] 保留指定小数位输出
来源：http://ju.yuntaijiaju.cn

Py:   f"{3.14159:.2f}"
来源：http://cy.huixinmuqiang.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dw.huixinmuqiang.cn

JS:   (3.14159).toFixed(2)
来源：http://zk.haigaiapp.cn

TS:   (3.14159).toFixed(2)
来源：http://oi.bjjhwx.cn

Java: String.format("%.2f", 3.14159)
来源：http://bg.asd995.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rv.newstarts.cn

Ruby: format("%.2f", 3.14159)
来源：http://lg.lnxyls.cn

C#:   3.14159.ToString("F2")
来源：http://qj.shxzukj.cn

[A22] 获取字符串长度
来源：http://jk.wgjwhj.cn

Py:   len(s)
来源：http://vd.yuntaijiaju.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cp.haigaiapp.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://em.521024.cn

TS:   s.length
来源：http://wi.9csxet.cn

Java: s.length()
来源：http://ho.nszjky.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qs.szxytkj.cn

Ruby: s.length
来源：http://vj.nszjky.cn

C#:   s.Length
来源：http://xr.szsharing.cn

[A23] 大小写转换
来源：http://yy.hahajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zv.shtwfgs.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ak.szsharing.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ly.gzmigu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://th.szsharing.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://po.szxytkj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cz.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rf.hahajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fq.lnxyls.cn

[A24] 去除首尾空白
来源：http://bk.hnjuh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vs.jctech888.com.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mr.bjjhwx.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xq.haigaiapp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cp.gzmigu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qu.huanxung.cn

Go:   strings.TrimSpace(s)
来源：http://bk.szsharing.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hh.yuexingan06.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fh.wgjwhj.cn

[A25] 字符串比较
来源：http://ts.chemitech.net.cn

Py:   s1 == s2; s1 != s2
来源：http://kk.bookmarksfly.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kz.bjjhwx.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yi.yuexingan06.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wq.muxihuayi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://eo.hahajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qz.asd995.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qr.yuexingan06.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tt.colortex.cn

[A26] 类型转换总览
来源：http://fz.shxzskj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gi.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ez.jianghongdianzi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kq.chemitech.net.cn

TS:   Number() String() Boolean() x as number
来源：http://wj.wgjwhj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jp.shtwfgs.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xy.jctech888.com.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kj.asd995.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nz.muxihuayi.cn

================================================================================
来源：http://ea.asd995.cn

B. 流程控制
来源：http://vs.newstarts.cn

================================================================================
来源：http://hz.muxihuayi.cn

[B01] 条件判断 if / else
来源：http://zu.colortex.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hq.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vm.panjiajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dl.haigaiapp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lh.newstarts.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ta.gzmigu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zi.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nd.muxihuayi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jd.gzmigu.cn

[B02] 多分支 else if / elif
来源：http://jc.shtwfgs.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qf.huixinmuqiang.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ci.panjiajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ml.szxytkj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xg.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sr.nicolike.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cd.szsharing.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ng.bjjhwx.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lj.shtwfgs.cn

[B03] switch / match / case
来源：http://at.huixiangedu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xl.shxzukj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mk.shxzukj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ge.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ab.9csxet.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mt.lnxyls.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fa.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jp.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vq.huanxung.cn

[B04] for 计数循环
来源：http://vx.muxihuayi.cn

Py:   for i in range(10): print(i)
来源：http://uo.huixiangedu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ke.szsharing.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zx.bjjhwx.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ht.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hp.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ow.shxzskj.cn

Ruby: 10.times { |i| puts i }
来源：http://pi.9csxet.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kn.shxzukj.cn

[B05] 遍历数组 / 列表
来源：http://xu.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://wn.hnjuh.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tp.muxihuayi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://np.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://un.newstarts.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gx.haigaiapp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pk.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://pw.panjiajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wi.hnjuh.cn

[B06] 遍历字典 / 对象
来源：http://og.bjjhwx.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fe.shxzukj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hh.panjiajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cp.521024.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xy.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oj.asd995.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yr.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tx.szsharing.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ee.hahajie.cn

[B07] while 循环
来源：http://sc.huixinmuqiang.cn

Py:   while i < 10: i += 1
来源：http://uz.bookmarksfly.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gs.wgjwhj.cn

JS:   while (i < 10) { i++; }
来源：http://dv.huixiangedu.cn

TS:   while (i < 10) { i++; }
来源：http://dj.9csxet.cn

Java: while (i < 10) { i++; }
来源：http://ev.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://iu.nicolike.cn

Ruby: while i < 10; i += 1; end
来源：http://id.shtwfgs.cn

C#:   while (i < 10) { i++; }
来源：http://iw.jctech888.com.cn

[B08] do-while（至少执行一次）
来源：http://zb.nicolike.cn

Py:   # 无 do-while：用 while True + break
来源：http://vl.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bk.yuexingan06.cn

JS:   do { i++; } while (i < 10);
来源：http://by.szxytkj.cn

TS:   do { i++; } while (i < 10);
来源：http://dc.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://xo.nicolike.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bv.jctech888.com.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rx.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://lw.asd995.cn

[B09] break 与 continue
来源：http://um.szsharing.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zu.hahajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ak.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lx.gzmigu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eh.szxytkj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ny.nicolike.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vo.nszjky.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ia.nicolike.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rj.521024.cn

[B10] 遍历同时拿索引
来源：http://gu.gzmigu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nm.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ag.shxzukj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ci.hahajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yz.521024.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xd.shxzukj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mx.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bl.shtwfgs.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ao.shxzskj.cn

[B11] 生成数字序列 / 区间
来源：http://jg.gzmigu.cn

Py:   list(range(0, 10, 2))
来源：http://ua.wgjwhj.cn

PHP:  range(0, 10, 2);
来源：http://px.nicolike.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tl.yuntaijiaju.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cm.newstarts.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://on.521024.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dh.shtwfgs.cn

Ruby: (0...10).step(2).to_a
来源：http://sy.asd995.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fa.nszjky.cn

[B12] 跳出多层循环
来源：http://dx.521024.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wk.jctech888.com.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dt.nicolike.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cw.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://oe.huanxung.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kq.huixinmuqiang.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fk.shtwfgs.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kz.szxytkj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jx.gzmigu.cn

[B13] 判断是否为数字
来源：http://go.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://hi.muxihuayi.cn

PHP:  is_numeric($x)
来源：http://uk.nicolike.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ls.bjjhwx.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qq.bjjhwx.cn

Java: x instanceof Number
来源：http://cv.yuntaijiaju.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rb.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://gv.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://mx.hahajie.cn

[B14] 判断值是否在集合内
来源：http://vl.wgjwhj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qc.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nq.bjjhwx.cn

JS:   [1, 2, 3].includes(x)
来源：http://ue.shtwfgs.cn

TS:   [1, 2, 3].includes(x)
来源：http://qr.9csxet.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://di.hahajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://om.wgjwhj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://es.szxytkj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gs.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://kg.huixinmuqiang.cn

Py:   a and b or not c
来源：http://vl.gzmigu.cn

PHP:  $a && $b || !$c
来源：http://wd.hnjuh.cn

JS:   a && b || !c
来源：http://uj.shxzskj.cn

TS:   a && b || !c
来源：http://pj.yuntaijiaju.cn

Java: a && b || !c
来源：http://gv.521024.cn

Go:   a && b || !c
来源：http://qc.szsharing.cn

Ruby: a && b || !c
来源：http://qc.szxytkj.cn

C#:   a && b || !c
来源：http://oo.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kp.huanxung.cn

Py:   if not data: return
来源：http://uj.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://xb.muxihuayi.cn

JS:   if (!data) return;
来源：http://xb.yuexingan06.cn

TS:   if (!data) return;
来源：http://ka.jianghongdianzi.cn

Java: if (data == null) return;
来源：http://za.gzmigu.cn

Go:   if data == nil { return }
来源：http://cq.bookmarksfly.cn

Ruby: return if data.nil?
来源：http://hk.9csxet.cn

C#:   if (data == null) return;
来源：http://ul.asd995.cn

================================================================================
来源：http://pz.asd995.cn

C. 函数与作用域
来源：http://km.szsharing.cn

================================================================================
来源：http://zp.yuexingan06.cn

[C01] 定义函数
来源：http://tc.chemitech.net.cn

Py:   def add(a, b): return a + b
来源：http://ts.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gd.bjjhwx.cn

JS:   function add(a, b) { return a + b; }
来源：http://oy.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mt.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vn.szsharing.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ey.yuexingan06.cn

Ruby: def add(a, b); a + b; end
来源：http://zw.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qb.bookmarksfly.cn

[C02] 默认参数
来源：http://ct.chemitech.net.cn

Py:   def greet(name="World"): return name
来源：http://kn.hahajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ue.asd995.cn

JS:   function greet(name = "World") { return name; }
来源：http://yk.colortex.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pl.huixiangedu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cd.nszjky.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qe.huanxung.cn

Ruby: def greet(name = "World") = name
来源：http://es.haigaiapp.cn

C#:   string Greet(string name = "World") => name;
来源：http://du.nicolike.cn

[C03] 可变参数
来源：http://st.shxzukj.cn

Py:   def total(*args): return sum(args)
来源：http://sa.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pw.yuntaijiaju.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://po.hnjuh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vw.wgjwhj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xa.bookmarksfly.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://aq.shxzukj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pq.yuexingan06.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sb.hnjuh.cn

[C04] 命名参数 / 关键字参数
来源：http://kj.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uj.yuexingan06.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kq.shxzskj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zm.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jv.asd995.cn

Java: // 无：用 Builder 模式或 record
来源：http://uf.9csxet.cn

Go:   // 无：用配置结构体参数
来源：http://jj.jctech888.com.cn

Ruby: f(a: 1, b: 2)
来源：http://wz.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://dp.shxzskj.cn

[C05] 返回多个值
来源：http://tl.muxihuayi.cn

Py:   return a, b
来源：http://ft.newstarts.cn

PHP:  return [$a, $b];
来源：http://dj.nicolike.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sg.huanxung.cn

TS:   return { a, b };
来源：http://qu.jctech888.com.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gp.lnxyls.cn

Go:   return a, b
来源：http://wo.shtwfgs.cn

Ruby: return a, b
来源：http://vd.nicolike.cn

C#:   return (a, b);              // ValueTuple
来源：http://bi.bjjhwx.cn

[C06] 匿名函数 / lambda
来源：http://bv.jctech888.com.cn

Py:   square = lambda x: x * x
来源：http://qc.szsharing.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cp.colortex.cn

JS:   const square = x => x * x;
来源：http://vz.9csxet.cn

TS:   const square = (x: number): number => x * x;
来源：http://ob.bjjhwx.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ac.muxihuayi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pa.hnjuh.cn

Ruby: square = ->(x) { x * x }
来源：http://tn.jctech888.com.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pv.shxzskj.cn

[C07] 把函数作为参数传入
来源：http://xn.huixiangedu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jy.huanxung.cn

PHP:  array_map("strtoupper", $arr);
来源：http://te.521024.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ik.jctech888.com.cn

TS:   arr.map(String)
来源：http://ij.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qv.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bf.huanxung.cn

Ruby: arr.map(&:upcase)
来源：http://ub.yuexingan06.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ih.muxihuayi.cn

[C08] 闭包
来源：http://ja.gzmigu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vq.nicolike.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sn.lnxyls.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://eq.haigaiapp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qx.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fi.shxzukj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rw.nszjky.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://om.jianghongdianzi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://py.gzmigu.cn

[C09] 递归
来源：http://kk.nicolike.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vu.nszjky.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dr.huanxung.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bn.521024.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nx.gzmigu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://me.nszjky.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pn.huanxung.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hi.shxzskj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cs.colortex.cn


<!-- 参考信息 -->