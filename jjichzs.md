代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://ar.haigaiapp.cn

Py:   ord("A"); chr(65)
来源：http://un.panjiajie.cn

PHP:  ord("A"); chr(65)
来源：http://kl.lnxyls.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yh.gzmigu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xn.9csxet.cn

Java: (int) 'A'; (char) 65
来源：http://lm.haigaiapp.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://np.lnxyls.cn

Ruby: "A".ord; 65.chr
来源：http://kn.szsharing.cn

C#:   (int)'A'; (char)65
来源：http://pp.jianghongdianzi.cn

[A19] 交换两个变量
来源：http://wf.szxytkj.cn

Py:   a, b = b, a
来源：http://jk.muxihuayi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tt.panjiajie.cn

JS:   [a, b] = [b, a];
来源：http://zv.hnjuh.cn

TS:   [a, b] = [b, a];
来源：http://xl.haigaiapp.cn

Java: int t = a; a = b; b = t;
来源：http://gz.huanxung.cn

Go:   a, b = b, a
来源：http://ob.9csxet.cn

Ruby: a, b = b, a
来源：http://yg.shtwfgs.cn

C#:   (a, b) = (b, a);
来源：http://ig.yuexingan06.cn

[A20] 读取标准输入
来源：http://dj.bjjhwx.cn

Py:   name = input("请输入：")
来源：http://un.hahajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://oi.jctech888.com.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ms.jianghongdianzi.cn

TS:   // Node.js：readline 模块
来源：http://pk.huanxung.cn

Java: new Scanner(System.in).nextLine()
来源：http://sf.panjiajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ud.hnjuh.cn

Ruby: gets.chomp
来源：http://dy.bookmarksfly.cn

C#:   Console.ReadLine();
来源：http://ij.panjiajie.cn

[A21] 保留指定小数位输出
来源：http://ye.yuexingan06.cn

Py:   f"{3.14159:.2f}"
来源：http://qz.521024.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pa.nicolike.cn

JS:   (3.14159).toFixed(2)
来源：http://du.huixinmuqiang.cn

TS:   (3.14159).toFixed(2)
来源：http://uh.lnxyls.cn

Java: String.format("%.2f", 3.14159)
来源：http://zn.bjjhwx.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wc.szsharing.cn

Ruby: format("%.2f", 3.14159)
来源：http://cl.bookmarksfly.cn

C#:   3.14159.ToString("F2")
来源：http://vn.shxzukj.cn

[A22] 获取字符串长度
来源：http://fi.huanxung.cn

Py:   len(s)
来源：http://yk.gzmigu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jy.huixinmuqiang.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sv.szsharing.cn

TS:   s.length
来源：http://jp.hahajie.cn

Java: s.length()
来源：http://uc.lnxyls.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nz.huixinmuqiang.cn

Ruby: s.length
来源：http://re.chemitech.net.cn

C#:   s.Length
来源：http://zb.hnjuh.cn

[A23] 大小写转换
来源：http://uh.gzmigu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://jf.huixiangedu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vb.yuntaijiaju.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pc.huanxung.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qu.lnxyls.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nz.shxzukj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://se.haigaiapp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kp.bjjhwx.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dl.colortex.cn

[A24] 去除首尾空白
来源：http://ch.huanxung.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ju.shtwfgs.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fl.newstarts.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ze.haigaiapp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bc.colortex.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dh.521024.cn

Go:   strings.TrimSpace(s)
来源：http://dq.huixinmuqiang.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mi.bookmarksfly.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kd.newstarts.cn

[A25] 字符串比较
来源：http://do.shxzukj.cn

Py:   s1 == s2; s1 != s2
来源：http://yn.shtwfgs.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ju.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ng.521024.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xh.shxzskj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://li.hnjuh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tj.bookmarksfly.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yu.shtwfgs.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kr.shtwfgs.cn

[A26] 类型转换总览
来源：http://fk.521024.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jh.521024.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pc.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vd.huanxung.cn

TS:   Number() String() Boolean() x as number
来源：http://lt.shtwfgs.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xm.huanxung.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ov.colortex.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://un.shxzukj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sg.huixinmuqiang.cn

================================================================================
来源：http://ks.haigaiapp.cn

B. 流程控制
来源：http://vr.shxzskj.cn

================================================================================
来源：http://an.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://us.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bf.shxzskj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://oe.shxzukj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qn.yuntaijiaju.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gr.wgjwhj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://aq.nicolike.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://di.jctech888.com.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ba.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rw.bookmarksfly.cn

[B02] 多分支 else if / elif
来源：http://la.bookmarksfly.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ob.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qc.nszjky.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gm.521024.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://er.jianghongdianzi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uo.muxihuayi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yg.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wb.jianghongdianzi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mw.chemitech.net.cn

[B03] switch / match / case
来源：http://or.nszjky.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tz.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uc.chemitech.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nf.chemitech.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dn.lnxyls.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vc.shtwfgs.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ko.chemitech.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://eh.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rq.szsharing.cn

[B04] for 计数循环
来源：http://rs.gzmigu.cn

Py:   for i in range(10): print(i)
来源：http://lb.521024.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xu.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yd.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yg.asd995.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ij.panjiajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qk.521024.cn

Ruby: 10.times { |i| puts i }
来源：http://je.bjjhwx.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lw.shxzukj.cn

[B05] 遍历数组 / 列表
来源：http://ra.shtwfgs.cn

Py:   for item in arr: print(item)
来源：http://yb.shtwfgs.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uk.shxzskj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lr.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tm.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yi.jianghongdianzi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://km.newstarts.cn

Ruby: arr.each { |item| puts item }
来源：http://bi.gzmigu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://re.hahajie.cn

[B06] 遍历字典 / 对象
来源：http://pk.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pa.nicolike.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://oy.huanxung.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nu.jianghongdianzi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://js.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nr.muxihuayi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wn.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qk.wgjwhj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rm.chemitech.net.cn

[B07] while 循环
来源：http://lt.haigaiapp.cn

Py:   while i < 10: i += 1
来源：http://cj.hahajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jh.9csxet.cn

JS:   while (i < 10) { i++; }
来源：http://tf.huanxung.cn

TS:   while (i < 10) { i++; }
来源：http://ul.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://xc.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mw.nszjky.cn

Ruby: while i < 10; i += 1; end
来源：http://pk.shtwfgs.cn

C#:   while (i < 10) { i++; }
来源：http://rr.szxytkj.cn

[B08] do-while（至少执行一次）
来源：http://kw.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://oa.nszjky.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://co.newstarts.cn

JS:   do { i++; } while (i < 10);
来源：http://wu.nicolike.cn

TS:   do { i++; } while (i < 10);
来源：http://pb.521024.cn

Java: do { i++; } while (i < 10);
来源：http://ol.muxihuayi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mz.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pv.szsharing.cn

C#:   do { i++; } while (i < 10);
来源：http://ju.yuexingan06.cn

[B09] break 与 continue
来源：http://hg.muxihuayi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zp.bjjhwx.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kg.jctech888.com.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kw.colortex.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sg.asd995.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sf.asd995.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tq.jianghongdianzi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ai.muxihuayi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uu.panjiajie.cn

[B10] 遍历同时拿索引
来源：http://kz.lnxyls.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://oi.yuexingan06.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wr.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kl.yuexingan06.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lq.szsharing.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cv.asd995.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oy.panjiajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lr.bjjhwx.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hq.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://tc.hnjuh.cn

Py:   list(range(0, 10, 2))
来源：http://kg.szsharing.cn

PHP:  range(0, 10, 2);
来源：http://uy.muxihuayi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mw.haigaiapp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ms.hnjuh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qd.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wb.hahajie.cn

Ruby: (0...10).step(2).to_a
来源：http://ml.colortex.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dq.szsharing.cn

[B12] 跳出多层循环
来源：http://zd.szsharing.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qn.shxzskj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rq.bjjhwx.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gv.nicolike.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dx.huanxung.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://aq.huanxung.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ha.jctech888.com.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yg.chemitech.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nb.shtwfgs.cn

[B13] 判断是否为数字
来源：http://fm.asd995.cn

Py:   isinstance(x, (int, float))
来源：http://qn.wgjwhj.cn

PHP:  is_numeric($x)
来源：http://nq.muxihuayi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cq.szsharing.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://to.521024.cn

Java: x instanceof Number
来源：http://ew.chemitech.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://es.newstarts.cn

Ruby: x.is_a?(Numeric)
来源：http://xn.hahajie.cn

C#:   x is int or double or decimal
来源：http://oz.nicolike.cn

[B14] 判断值是否在集合内
来源：http://gp.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jy.panjiajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tj.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://ih.huixinmuqiang.cn

TS:   [1, 2, 3].includes(x)
来源：http://os.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lp.shxzukj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dh.szsharing.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vo.gzmigu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dc.yuexingan06.cn

[B15] 布尔运算与取反
来源：http://qg.muxihuayi.cn

Py:   a and b or not c
来源：http://im.hahajie.cn

PHP:  $a && $b || !$c
来源：http://gi.bjjhwx.cn

JS:   a && b || !c
来源：http://pz.shxzukj.cn

TS:   a && b || !c
来源：http://vr.9csxet.cn

Java: a && b || !c
来源：http://ta.521024.cn

Go:   a && b || !c
来源：http://so.szsharing.cn

Ruby: a && b || !c
来源：http://mo.shtwfgs.cn

C#:   a && b || !c
来源：http://ta.shxzskj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kf.huixiangedu.cn

Py:   if not data: return
来源：http://fn.bookmarksfly.cn

PHP:  if (!$data) { return; }
来源：http://on.nicolike.cn

JS:   if (!data) return;
来源：http://ab.yuexingan06.cn

TS:   if (!data) return;
来源：http://sj.wgjwhj.cn

Java: if (data == null) return;
来源：http://uk.szsharing.cn

Go:   if data == nil { return }
来源：http://ga.jctech888.com.cn

Ruby: return if data.nil?
来源：http://vz.huixinmuqiang.cn

C#:   if (data == null) return;
来源：http://he.jctech888.com.cn

================================================================================
来源：http://aw.wgjwhj.cn

C. 函数与作用域
来源：http://gk.yuexingan06.cn

================================================================================
来源：http://gx.shxzukj.cn

[C01] 定义函数
来源：http://ur.shxzukj.cn

Py:   def add(a, b): return a + b
来源：http://yd.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tk.newstarts.cn

JS:   function add(a, b) { return a + b; }
来源：http://na.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jf.szxytkj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://td.asd995.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vk.hahajie.cn

Ruby: def add(a, b); a + b; end
来源：http://rm.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://va.jctech888.com.cn

[C02] 默认参数
来源：http://lu.jctech888.com.cn

Py:   def greet(name="World"): return name
来源：http://rj.jctech888.com.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zs.shxzskj.cn

JS:   function greet(name = "World") { return name; }
来源：http://pw.muxihuayi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lu.jctech888.com.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fz.521024.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://iq.colortex.cn

Ruby: def greet(name = "World") = name
来源：http://qi.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://ht.lnxyls.cn

[C03] 可变参数
来源：http://cz.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://qk.521024.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sg.jianghongdianzi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dw.nicolike.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xx.jianghongdianzi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vl.jctech888.com.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fa.haigaiapp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ow.yuntaijiaju.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ua.asd995.cn

[C04] 命名参数 / 关键字参数
来源：http://cq.huixiangedu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nx.521024.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kz.chemitech.net.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://se.9csxet.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rq.lnxyls.cn

Java: // 无：用 Builder 模式或 record
来源：http://no.panjiajie.cn

Go:   // 无：用配置结构体参数
来源：http://ha.colortex.cn

Ruby: f(a: 1, b: 2)
来源：http://ks.asd995.cn

C#:   f(a: 1, b: 2)
来源：http://zm.panjiajie.cn

[C05] 返回多个值
来源：http://xl.yuexingan06.cn

Py:   return a, b
来源：http://kg.yuntaijiaju.cn

PHP:  return [$a, $b];
来源：http://io.hahajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yl.wgjwhj.cn

TS:   return { a, b };
来源：http://mg.szsharing.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xb.bookmarksfly.cn

Go:   return a, b
来源：http://wk.muxihuayi.cn

Ruby: return a, b
来源：http://ns.yuntaijiaju.cn

C#:   return (a, b);              // ValueTuple
来源：http://vk.shtwfgs.cn

[C06] 匿名函数 / lambda
来源：http://hb.shxzskj.cn

Py:   square = lambda x: x * x
来源：http://mt.szxytkj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zm.huixinmuqiang.cn

JS:   const square = x => x * x;
来源：http://za.panjiajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://yx.shtwfgs.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qn.szxytkj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xy.lnxyls.cn

Ruby: square = ->(x) { x * x }
来源：http://mq.jianghongdianzi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hv.hnjuh.cn

[C07] 把函数作为参数传入
来源：http://wy.huixinmuqiang.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mc.colortex.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pw.9csxet.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zd.shxzukj.cn

TS:   arr.map(String)
来源：http://tx.hnjuh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rm.hahajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nm.muxihuayi.cn

Ruby: arr.map(&:upcase)
来源：http://af.haigaiapp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vy.lnxyls.cn

[C08] 闭包
来源：http://qq.wgjwhj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cc.shxzskj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kx.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bw.huixiangedu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jk.shxzukj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lc.muxihuayi.cn


<!-- 参考信息 -->