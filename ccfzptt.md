代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://sb.huanxung.cn

Py:   ord("A"); chr(65)
来源：http://ek.lnxyls.cn

PHP:  ord("A"); chr(65)
来源：http://zs.gzmigu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vn.yuntaijiaju.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mu.haigaiapp.cn

Java: (int) 'A'; (char) 65
来源：http://sg.nicolike.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://le.bookmarksfly.cn

Ruby: "A".ord; 65.chr
来源：http://ma.yuexingan06.cn

C#:   (int)'A'; (char)65
来源：http://kf.panjiajie.cn

[A19] 交换两个变量
来源：http://tm.huixinmuqiang.cn

Py:   a, b = b, a
来源：http://yz.gzmigu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://lo.bookmarksfly.cn

JS:   [a, b] = [b, a];
来源：http://pq.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://ek.huanxung.cn

Java: int t = a; a = b; b = t;
来源：http://os.nszjky.cn

Go:   a, b = b, a
来源：http://jo.shxzskj.cn

Ruby: a, b = b, a
来源：http://gh.hnjuh.cn

C#:   (a, b) = (b, a);
来源：http://ag.bookmarksfly.cn

[A20] 读取标准输入
来源：http://es.9csxet.cn

Py:   name = input("请输入：")
来源：http://xw.bookmarksfly.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://cr.haigaiapp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tq.yuexingan06.cn

TS:   // Node.js：readline 模块
来源：http://ti.jctech888.com.cn

Java: new Scanner(System.in).nextLine()
来源：http://ke.shtwfgs.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vn.asd995.cn

Ruby: gets.chomp
来源：http://dy.panjiajie.cn

C#:   Console.ReadLine();
来源：http://gj.521024.cn

[A21] 保留指定小数位输出
来源：http://tm.newstarts.cn

Py:   f"{3.14159:.2f}"
来源：http://fr.chemitech.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://co.huanxung.cn

JS:   (3.14159).toFixed(2)
来源：http://el.lnxyls.cn

TS:   (3.14159).toFixed(2)
来源：http://pc.bjjhwx.cn

Java: String.format("%.2f", 3.14159)
来源：http://mx.asd995.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qj.hahajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://qi.huixinmuqiang.cn

C#:   3.14159.ToString("F2")
来源：http://sn.nicolike.cn

[A22] 获取字符串长度
来源：http://ld.gzmigu.cn

Py:   len(s)
来源：http://dq.asd995.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mh.wgjwhj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xs.muxihuayi.cn

TS:   s.length
来源：http://jy.shxzskj.cn

Java: s.length()
来源：http://im.szxytkj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jd.yuexingan06.cn

Ruby: s.length
来源：http://so.9csxet.cn

C#:   s.Length
来源：http://mi.huixiangedu.cn

[A23] 大小写转换
来源：http://un.szsharing.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://cs.huixiangedu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://so.wgjwhj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bj.shxzskj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zq.newstarts.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ii.yuexingan06.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ak.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ld.yuexingan06.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xe.colortex.cn

[A24] 去除首尾空白
来源：http://el.huanxung.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ag.521024.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mz.nicolike.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jt.shxzukj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ay.9csxet.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://oz.asd995.cn

Go:   strings.TrimSpace(s)
来源：http://se.9csxet.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bi.bjjhwx.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vq.nicolike.cn

[A25] 字符串比较
来源：http://ut.huanxung.cn

Py:   s1 == s2; s1 != s2
来源：http://ai.jctech888.com.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wh.lnxyls.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ko.chemitech.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gp.huixiangedu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ap.chemitech.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dn.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pi.bookmarksfly.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ox.huixiangedu.cn

[A26] 类型转换总览
来源：http://yt.yuntaijiaju.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zk.chemitech.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sb.gzmigu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ot.huixiangedu.cn

TS:   Number() String() Boolean() x as number
来源：http://mq.huixinmuqiang.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nx.yuexingan06.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://av.9csxet.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://iy.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dq.nszjky.cn

================================================================================
来源：http://ri.9csxet.cn

B. 流程控制
来源：http://zi.szsharing.cn

================================================================================
来源：http://fp.szsharing.cn

[B01] 条件判断 if / else
来源：http://uf.chemitech.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wx.muxihuayi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hn.szsharing.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bj.colortex.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oy.jianghongdianzi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vf.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xr.lnxyls.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nm.hahajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rw.hahajie.cn

[B02] 多分支 else if / elif
来源：http://lh.yuntaijiaju.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pu.bjjhwx.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://au.muxihuayi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jq.jctech888.com.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ym.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ce.nicolike.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xj.bjjhwx.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://px.521024.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nx.newstarts.cn

[B03] switch / match / case
来源：http://wu.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://en.asd995.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tb.szsharing.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tv.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ts.nicolike.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cb.jctech888.com.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qr.huixinmuqiang.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yu.huanxung.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wd.lnxyls.cn

[B04] for 计数循环
来源：http://wu.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://fu.521024.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sd.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ep.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ev.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vz.nszjky.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lb.wgjwhj.cn

Ruby: 10.times { |i| puts i }
来源：http://xj.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sr.shxzukj.cn

[B05] 遍历数组 / 列表
来源：http://ac.yuexingan06.cn

Py:   for item in arr: print(item)
来源：http://rv.wgjwhj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://os.521024.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://pl.jctech888.com.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pu.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jh.nszjky.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dm.szsharing.cn

Ruby: arr.each { |item| puts item }
来源：http://yt.yuntaijiaju.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rd.chemitech.net.cn

[B06] 遍历字典 / 对象
来源：http://gs.hahajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vn.shxzukj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bb.bookmarksfly.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xt.bjjhwx.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uk.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uw.hnjuh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jo.gzmigu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nb.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://oh.hahajie.cn

[B07] while 循环
来源：http://bn.muxihuayi.cn

Py:   while i < 10: i += 1
来源：http://bi.yuntaijiaju.cn

PHP:  while ($i < 10) { $i++; }
来源：http://aq.wgjwhj.cn

JS:   while (i < 10) { i++; }
来源：http://xv.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://xx.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://kp.jianghongdianzi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rm.szxytkj.cn

Ruby: while i < 10; i += 1; end
来源：http://cy.hnjuh.cn

C#:   while (i < 10) { i++; }
来源：http://jr.hnjuh.cn

[B08] do-while（至少执行一次）
来源：http://bz.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://uz.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vp.nszjky.cn

JS:   do { i++; } while (i < 10);
来源：http://jx.wgjwhj.cn

TS:   do { i++; } while (i < 10);
来源：http://ai.wgjwhj.cn

Java: do { i++; } while (i < 10);
来源：http://oe.szxytkj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zv.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tc.shxzskj.cn

C#:   do { i++; } while (i < 10);
来源：http://ir.521024.cn

[B09] break 与 continue
来源：http://ux.colortex.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jl.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xm.yuntaijiaju.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xz.bjjhwx.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jl.shtwfgs.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jt.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rj.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ly.newstarts.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yi.chemitech.net.cn

[B10] 遍历同时拿索引
来源：http://xv.panjiajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ch.yuexingan06.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://si.lnxyls.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dk.hnjuh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rn.haigaiapp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://by.chemitech.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ma.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jn.wgjwhj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dk.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://bz.shxzukj.cn

Py:   list(range(0, 10, 2))
来源：http://oe.wgjwhj.cn

PHP:  range(0, 10, 2);
来源：http://hp.huixiangedu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iz.yuntaijiaju.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rd.9csxet.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ar.colortex.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dg.newstarts.cn

Ruby: (0...10).step(2).to_a
来源：http://gj.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vq.9csxet.cn

[B12] 跳出多层循环
来源：http://rk.lnxyls.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://al.gzmigu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hd.wgjwhj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dt.muxihuayi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pg.shxzukj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cn.chemitech.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lg.shxzskj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kj.bjjhwx.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dt.jctech888.com.cn

[B13] 判断是否为数字
来源：http://oj.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://ho.muxihuayi.cn

PHP:  is_numeric($x)
来源：http://do.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ab.hnjuh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yw.shtwfgs.cn

Java: x instanceof Number
来源：http://mq.521024.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tv.yuexingan06.cn

Ruby: x.is_a?(Numeric)
来源：http://qf.colortex.cn

C#:   x is int or double or decimal
来源：http://hh.shtwfgs.cn

[B14] 判断值是否在集合内
来源：http://ms.huixiangedu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jk.panjiajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lw.yuntaijiaju.cn

JS:   [1, 2, 3].includes(x)
来源：http://li.newstarts.cn

TS:   [1, 2, 3].includes(x)
来源：http://ra.hnjuh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ib.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bt.shtwfgs.cn

Ruby: [1, 2, 3].include?(x)
来源：http://eg.shxzukj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qu.nicolike.cn

[B15] 布尔运算与取反
来源：http://oq.shxzukj.cn

Py:   a and b or not c
来源：http://ei.gzmigu.cn

PHP:  $a && $b || !$c
来源：http://pl.muxihuayi.cn

JS:   a && b || !c
来源：http://wt.chemitech.net.cn

TS:   a && b || !c
来源：http://ij.newstarts.cn

Java: a && b || !c
来源：http://ur.huixinmuqiang.cn

Go:   a && b || !c
来源：http://sk.nicolike.cn

Ruby: a && b || !c
来源：http://qe.shtwfgs.cn

C#:   a && b || !c
来源：http://sx.shxzskj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vl.521024.cn

Py:   if not data: return
来源：http://es.521024.cn

PHP:  if (!$data) { return; }
来源：http://qc.nszjky.cn

JS:   if (!data) return;
来源：http://iu.nicolike.cn

TS:   if (!data) return;
来源：http://ck.nszjky.cn

Java: if (data == null) return;
来源：http://wc.hahajie.cn

Go:   if data == nil { return }
来源：http://ec.huixinmuqiang.cn

Ruby: return if data.nil?
来源：http://zo.hnjuh.cn

C#:   if (data == null) return;
来源：http://hk.jctech888.com.cn

================================================================================
来源：http://yh.hnjuh.cn

C. 函数与作用域
来源：http://bf.nicolike.cn

================================================================================
来源：http://la.colortex.cn

[C01] 定义函数
来源：http://rl.hahajie.cn

Py:   def add(a, b): return a + b
来源：http://qt.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oy.haigaiapp.cn

JS:   function add(a, b) { return a + b; }
来源：http://ke.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dd.wgjwhj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://li.shxzskj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://st.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://rv.szsharing.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ey.haigaiapp.cn

[C02] 默认参数
来源：http://ct.chemitech.net.cn

Py:   def greet(name="World"): return name
来源：http://zh.shtwfgs.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rv.9csxet.cn

JS:   function greet(name = "World") { return name; }
来源：http://ty.gzmigu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ve.newstarts.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ti.521024.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bk.jctech888.com.cn

Ruby: def greet(name = "World") = name
来源：http://rd.newstarts.cn

C#:   string Greet(string name = "World") => name;
来源：http://ly.yuexingan06.cn

[C03] 可变参数
来源：http://oz.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://kj.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gc.gzmigu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mt.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qn.nicolike.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ht.bookmarksfly.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gp.haigaiapp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://us.huixiangedu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qm.wgjwhj.cn

[C04] 命名参数 / 关键字参数
来源：http://bo.nicolike.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ks.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bk.huixinmuqiang.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yh.nszjky.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vg.hahajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://er.haigaiapp.cn

Go:   // 无：用配置结构体参数
来源：http://rn.huanxung.cn

Ruby: f(a: 1, b: 2)
来源：http://rn.haigaiapp.cn

C#:   f(a: 1, b: 2)
来源：http://wk.bjjhwx.cn

[C05] 返回多个值
来源：http://wz.jianghongdianzi.cn

Py:   return a, b
来源：http://br.szxytkj.cn

PHP:  return [$a, $b];
来源：http://wn.huixinmuqiang.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dl.jctech888.com.cn

TS:   return { a, b };
来源：http://si.hahajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bq.newstarts.cn

Go:   return a, b
来源：http://di.colortex.cn

Ruby: return a, b
来源：http://nx.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://ud.huanxung.cn

[C06] 匿名函数 / lambda
来源：http://wl.bookmarksfly.cn

Py:   square = lambda x: x * x
来源：http://sl.jctech888.com.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vm.521024.cn

JS:   const square = x => x * x;
来源：http://he.panjiajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://yd.gzmigu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vs.wgjwhj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ec.huanxung.cn

Ruby: square = ->(x) { x * x }
来源：http://hd.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bk.bookmarksfly.cn

[C07] 把函数作为参数传入
来源：http://ca.lnxyls.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yq.yuexingan06.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tj.shxzskj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mw.hahajie.cn

TS:   arr.map(String)
来源：http://cj.nicolike.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bm.hnjuh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dm.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://fu.huixinmuqiang.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jj.huixiangedu.cn

[C08] 闭包
来源：http://rs.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vt.nszjky.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ds.huixiangedu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ru.9csxet.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cy.shxzskj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xa.szsharing.cn


<!-- 参考信息 -->