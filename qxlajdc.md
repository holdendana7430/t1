代发 wailian999

C#:   (int)'A'; (char)65
来源：http://yt.newstarts.cn

[A19] 交换两个变量
来源：http://iw.szxytkj.cn

Py:   a, b = b, a
来源：http://nn.wgjwhj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fk.huixinmuqiang.cn

JS:   [a, b] = [b, a];
来源：http://ti.nszjky.cn

TS:   [a, b] = [b, a];
来源：http://bl.gzmigu.cn

Java: int t = a; a = b; b = t;
来源：http://qa.chemitech.net.cn

Go:   a, b = b, a
来源：http://bp.shtwfgs.cn

Ruby: a, b = b, a
来源：http://ep.panjiajie.cn

C#:   (a, b) = (b, a);
来源：http://ho.shxzukj.cn

[A20] 读取标准输入
来源：http://os.haigaiapp.cn

Py:   name = input("请输入：")
来源：http://qf.muxihuayi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://yn.szsharing.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ce.haigaiapp.cn

TS:   // Node.js：readline 模块
来源：http://hv.bjjhwx.cn

Java: new Scanner(System.in).nextLine()
来源：http://gs.szsharing.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vy.huixinmuqiang.cn

Ruby: gets.chomp
来源：http://ap.muxihuayi.cn

C#:   Console.ReadLine();
来源：http://ec.asd995.cn

[A21] 保留指定小数位输出
来源：http://dy.nszjky.cn

Py:   f"{3.14159:.2f}"
来源：http://yd.huixinmuqiang.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nw.hahajie.cn

JS:   (3.14159).toFixed(2)
来源：http://tv.yuexingan06.cn

TS:   (3.14159).toFixed(2)
来源：http://cm.shxzskj.cn

Java: String.format("%.2f", 3.14159)
来源：http://gv.9csxet.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mq.gzmigu.cn

Ruby: format("%.2f", 3.14159)
来源：http://ul.bjjhwx.cn

C#:   3.14159.ToString("F2")
来源：http://vs.chemitech.net.cn

[A22] 获取字符串长度
来源：http://oc.newstarts.cn

Py:   len(s)
来源：http://wf.hnjuh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vf.chemitech.net.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fy.colortex.cn

TS:   s.length
来源：http://kw.colortex.cn

Java: s.length()
来源：http://pk.huixiangedu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lg.hahajie.cn

Ruby: s.length
来源：http://mh.asd995.cn

C#:   s.Length
来源：http://lg.nicolike.cn

[A23] 大小写转换
来源：http://mx.wgjwhj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wz.haigaiapp.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://if.shtwfgs.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zd.gzmigu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rq.panjiajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dj.wgjwhj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nc.muxihuayi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qy.shxzskj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zu.szxytkj.cn

[A24] 去除首尾空白
来源：http://pz.hnjuh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jx.shtwfgs.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kf.huixiangedu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fv.shxzukj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ej.asd995.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pn.newstarts.cn

Go:   strings.TrimSpace(s)
来源：http://eb.yuexingan06.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bu.521024.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xj.szxytkj.cn

[A25] 字符串比较
来源：http://qa.shxzukj.cn

Py:   s1 == s2; s1 != s2
来源：http://ka.yuntaijiaju.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ca.jianghongdianzi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lw.colortex.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://st.panjiajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ox.asd995.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cc.gzmigu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hr.bjjhwx.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tx.hnjuh.cn

[A26] 类型转换总览
来源：http://cr.colortex.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ms.szsharing.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hv.wgjwhj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ny.colortex.cn

TS:   Number() String() Boolean() x as number
来源：http://gn.huanxung.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zb.hnjuh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://os.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://uw.szsharing.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rs.521024.cn

================================================================================
来源：http://or.jianghongdianzi.cn

B. 流程控制
来源：http://lg.shtwfgs.cn

================================================================================
来源：http://to.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://qa.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pp.nicolike.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qr.shxzskj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qg.huixinmuqiang.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nf.shxzskj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ab.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://te.huixinmuqiang.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mj.shtwfgs.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mz.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://xb.colortex.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gu.hnjuh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qz.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nj.lnxyls.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://da.hahajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mc.colortex.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bu.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wp.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cr.jianghongdianzi.cn

[B03] switch / match / case
来源：http://nb.yuexingan06.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ql.chemitech.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pm.wgjwhj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pa.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wt.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lg.panjiajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fu.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xy.bjjhwx.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ok.nszjky.cn

[B04] for 计数循环
来源：http://zg.nicolike.cn

Py:   for i in range(10): print(i)
来源：http://ii.jctech888.com.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bf.shxzskj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://au.shtwfgs.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xj.521024.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://un.shxzskj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ta.lnxyls.cn

Ruby: 10.times { |i| puts i }
来源：http://qy.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fv.szsharing.cn

[B05] 遍历数组 / 列表
来源：http://ga.jctech888.com.cn

Py:   for item in arr: print(item)
来源：http://xf.huixiangedu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uv.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ax.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ul.szxytkj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wz.szsharing.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gp.haigaiapp.cn

Ruby: arr.each { |item| puts item }
来源：http://xm.bookmarksfly.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fk.haigaiapp.cn

[B06] 遍历字典 / 对象
来源：http://ak.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qm.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jm.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ky.asd995.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://np.9csxet.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fi.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uf.yuntaijiaju.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://es.shxzukj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://iv.chemitech.net.cn

[B07] while 循环
来源：http://kk.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://zn.yuntaijiaju.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lh.chemitech.net.cn

JS:   while (i < 10) { i++; }
来源：http://qd.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://rc.bjjhwx.cn

Java: while (i < 10) { i++; }
来源：http://zv.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yy.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://ti.lnxyls.cn

C#:   while (i < 10) { i++; }
来源：http://nj.huanxung.cn

[B08] do-while（至少执行一次）
来源：http://lh.gzmigu.cn

Py:   # 无 do-while：用 while True + break
来源：http://sp.521024.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mo.yuntaijiaju.cn

JS:   do { i++; } while (i < 10);
来源：http://dr.asd995.cn

TS:   do { i++; } while (i < 10);
来源：http://zb.wgjwhj.cn

Java: do { i++; } while (i < 10);
来源：http://oq.shxzskj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vq.yuntaijiaju.cn

Ruby: begin; i += 1; end while i < 10
来源：http://oa.panjiajie.cn

C#:   do { i++; } while (i < 10);
来源：http://ph.wgjwhj.cn

[B09] break 与 continue
来源：http://xl.bjjhwx.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cr.9csxet.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wn.szxytkj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kd.haigaiapp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://so.yuntaijiaju.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zc.nicolike.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mg.wgjwhj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ln.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wn.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://kr.szsharing.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qo.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vo.bjjhwx.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nf.haigaiapp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ic.bookmarksfly.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lu.gzmigu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fu.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rb.newstarts.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dk.521024.cn

[B11] 生成数字序列 / 区间
来源：http://bc.panjiajie.cn

Py:   list(range(0, 10, 2))
来源：http://iq.asd995.cn

PHP:  range(0, 10, 2);
来源：http://lf.yuexingan06.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qa.wgjwhj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://da.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gg.huixiangedu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dt.nicolike.cn

Ruby: (0...10).step(2).to_a
来源：http://ye.haigaiapp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zq.szxytkj.cn

[B12] 跳出多层循环
来源：http://rz.muxihuayi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tv.gzmigu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xj.muxihuayi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://aq.bookmarksfly.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://oh.shxzukj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gc.bjjhwx.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zc.shxzukj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ng.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tf.shxzskj.cn

[B13] 判断是否为数字
来源：http://ki.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://je.521024.cn

PHP:  is_numeric($x)
来源：http://lq.9csxet.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vt.asd995.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uc.yuntaijiaju.cn

Java: x instanceof Number
来源：http://ej.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rn.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://aq.nszjky.cn

C#:   x is int or double or decimal
来源：http://pf.wgjwhj.cn

[B14] 判断值是否在集合内
来源：http://ri.szsharing.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vg.9csxet.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rd.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://yi.gzmigu.cn

TS:   [1, 2, 3].includes(x)
来源：http://gf.muxihuayi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ag.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://la.haigaiapp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ra.shxzskj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ri.shxzskj.cn

[B15] 布尔运算与取反
来源：http://ky.chemitech.net.cn

Py:   a and b or not c
来源：http://eq.gzmigu.cn

PHP:  $a && $b || !$c
来源：http://nq.521024.cn

JS:   a && b || !c
来源：http://ac.nszjky.cn

TS:   a && b || !c
来源：http://rf.bookmarksfly.cn

Java: a && b || !c
来源：http://sn.shxzskj.cn

Go:   a && b || !c
来源：http://kx.yuntaijiaju.cn

Ruby: a && b || !c
来源：http://jp.bookmarksfly.cn

C#:   a && b || !c
来源：http://sp.wgjwhj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fl.shtwfgs.cn

Py:   if not data: return
来源：http://cj.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://nv.wgjwhj.cn

JS:   if (!data) return;
来源：http://do.jianghongdianzi.cn

TS:   if (!data) return;
来源：http://ul.colortex.cn

Java: if (data == null) return;
来源：http://jm.bookmarksfly.cn

Go:   if data == nil { return }
来源：http://gp.shxzukj.cn

Ruby: return if data.nil?
来源：http://iv.colortex.cn

C#:   if (data == null) return;
来源：http://wk.huanxung.cn

================================================================================
来源：http://rb.yuntaijiaju.cn

C. 函数与作用域
来源：http://gv.9csxet.cn

================================================================================
来源：http://mr.panjiajie.cn

[C01] 定义函数
来源：http://iu.haigaiapp.cn

Py:   def add(a, b): return a + b
来源：http://oe.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xh.bookmarksfly.cn

JS:   function add(a, b) { return a + b; }
来源：http://dc.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kt.colortex.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mu.panjiajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xc.jianghongdianzi.cn

Ruby: def add(a, b); a + b; end
来源：http://hk.jianghongdianzi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ab.hnjuh.cn

[C02] 默认参数
来源：http://hm.huixinmuqiang.cn

Py:   def greet(name="World"): return name
来源：http://xx.huanxung.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ni.gzmigu.cn

JS:   function greet(name = "World") { return name; }
来源：http://kp.gzmigu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xx.hnjuh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nf.chemitech.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zc.nszjky.cn

Ruby: def greet(name = "World") = name
来源：http://er.shxzukj.cn

C#:   string Greet(string name = "World") => name;
来源：http://bk.szxytkj.cn

[C03] 可变参数
来源：http://he.shtwfgs.cn

Py:   def total(*args): return sum(args)
来源：http://mw.newstarts.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rf.nicolike.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://or.muxihuayi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kx.nszjky.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vs.haigaiapp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zn.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ip.9csxet.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tf.panjiajie.cn

[C04] 命名参数 / 关键字参数
来源：http://wm.gzmigu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eb.shtwfgs.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ss.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yb.521024.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jv.lnxyls.cn

Java: // 无：用 Builder 模式或 record
来源：http://ke.nicolike.cn

Go:   // 无：用配置结构体参数
来源：http://ss.9csxet.cn

Ruby: f(a: 1, b: 2)
来源：http://or.szxytkj.cn

C#:   f(a: 1, b: 2)
来源：http://ll.yuexingan06.cn

[C05] 返回多个值
来源：http://rk.jianghongdianzi.cn

Py:   return a, b
来源：http://ve.gzmigu.cn

PHP:  return [$a, $b];
来源：http://eb.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://am.yuntaijiaju.cn

TS:   return { a, b };
来源：http://xa.jianghongdianzi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zw.9csxet.cn

Go:   return a, b
来源：http://qy.nszjky.cn

Ruby: return a, b
来源：http://ur.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://id.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://lf.szxytkj.cn

Py:   square = lambda x: x * x
来源：http://hj.haigaiapp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bc.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://qx.hahajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://kr.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://es.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xv.hnjuh.cn

Ruby: square = ->(x) { x * x }
来源：http://pt.9csxet.cn

C#:   Func<int, int> square = x => x * x;
来源：http://kf.newstarts.cn

[C07] 把函数作为参数传入
来源：http://eu.bjjhwx.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dc.jctech888.com.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ug.jctech888.com.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ms.asd995.cn

TS:   arr.map(String)
来源：http://xp.muxihuayi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ft.huixiangedu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jn.huixinmuqiang.cn

Ruby: arr.map(&:upcase)
来源：http://mb.haigaiapp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ch.521024.cn

[C08] 闭包
来源：http://xl.jianghongdianzi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cj.9csxet.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xx.wgjwhj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://id.521024.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bu.bookmarksfly.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jg.521024.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qu.jianghongdianzi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ki.huixiangedu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ey.lnxyls.cn

[C09] 递归
来源：http://gk.shtwfgs.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qh.huixinmuqiang.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ed.bjjhwx.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ke.yuntaijiaju.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ew.szxytkj.cn


<!-- 参考信息 -->