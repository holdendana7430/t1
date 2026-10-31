代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://ni.yuntaijiaju.cn

Py:   ord("A"); chr(65)
来源：http://sa.asd995.cn

PHP:  ord("A"); chr(65)
来源：http://dp.panjiajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sv.huixiangedu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vg.nicolike.cn

Java: (int) 'A'; (char) 65
来源：http://cz.jianghongdianzi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ke.9csxet.cn

Ruby: "A".ord; 65.chr
来源：http://xn.szxytkj.cn

C#:   (int)'A'; (char)65
来源：http://px.lnxyls.cn

[A19] 交换两个变量
来源：http://yx.hahajie.cn

Py:   a, b = b, a
来源：http://oq.hahajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://or.huanxung.cn

JS:   [a, b] = [b, a];
来源：http://bl.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://bn.panjiajie.cn

Java: int t = a; a = b; b = t;
来源：http://rk.panjiajie.cn

Go:   a, b = b, a
来源：http://rj.muxihuayi.cn

Ruby: a, b = b, a
来源：http://pj.gzmigu.cn

C#:   (a, b) = (b, a);
来源：http://kl.lnxyls.cn

[A20] 读取标准输入
来源：http://kt.shxzukj.cn

Py:   name = input("请输入：")
来源：http://zb.521024.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://eu.shxzukj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ja.huanxung.cn

TS:   // Node.js：readline 模块
来源：http://fp.bookmarksfly.cn

Java: new Scanner(System.in).nextLine()
来源：http://jt.yuntaijiaju.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ho.newstarts.cn

Ruby: gets.chomp
来源：http://nb.newstarts.cn

C#:   Console.ReadLine();
来源：http://hb.muxihuayi.cn

[A21] 保留指定小数位输出
来源：http://lw.chemitech.net.cn

Py:   f"{3.14159:.2f}"
来源：http://me.panjiajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://on.bookmarksfly.cn

JS:   (3.14159).toFixed(2)
来源：http://ra.shxzskj.cn

TS:   (3.14159).toFixed(2)
来源：http://bc.wgjwhj.cn

Java: String.format("%.2f", 3.14159)
来源：http://bi.muxihuayi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://go.hnjuh.cn

Ruby: format("%.2f", 3.14159)
来源：http://dt.9csxet.cn

C#:   3.14159.ToString("F2")
来源：http://di.asd995.cn

[A22] 获取字符串长度
来源：http://wn.bookmarksfly.cn

Py:   len(s)
来源：http://bo.hahajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ze.szxytkj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://al.newstarts.cn

TS:   s.length
来源：http://vs.9csxet.cn

Java: s.length()
来源：http://je.haigaiapp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://oi.shxzukj.cn

Ruby: s.length
来源：http://ub.nszjky.cn

C#:   s.Length
来源：http://ve.chemitech.net.cn

[A23] 大小写转换
来源：http://tz.521024.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://io.jctech888.com.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ko.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ta.szxytkj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://td.shtwfgs.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wd.bjjhwx.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hc.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://je.newstarts.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://aj.huixiangedu.cn

[A24] 去除首尾空白
来源：http://av.jctech888.com.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zx.lnxyls.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nn.chemitech.net.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ja.szsharing.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://az.nicolike.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://uh.gzmigu.cn

Go:   strings.TrimSpace(s)
来源：http://xn.9csxet.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kl.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rh.shxzukj.cn

[A25] 字符串比较
来源：http://av.jianghongdianzi.cn

Py:   s1 == s2; s1 != s2
来源：http://ct.bjjhwx.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ke.muxihuayi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qs.9csxet.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hn.huanxung.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://js.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ow.521024.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ys.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fz.lnxyls.cn

[A26] 类型转换总览
来源：http://zh.nszjky.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yg.bjjhwx.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cv.haigaiapp.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bz.szxytkj.cn

TS:   Number() String() Boolean() x as number
来源：http://io.shxzskj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qv.szxytkj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fy.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rs.shxzukj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ei.nicolike.cn

================================================================================
来源：http://cx.shxzskj.cn

B. 流程控制
来源：http://jp.lnxyls.cn

================================================================================
来源：http://kb.bjjhwx.cn

[B01] 条件判断 if / else
来源：http://ht.bookmarksfly.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://tt.shtwfgs.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bw.yuntaijiaju.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://na.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://el.yuntaijiaju.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dh.huixiangedu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pc.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rc.bjjhwx.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tk.shtwfgs.cn

[B02] 多分支 else if / elif
来源：http://fe.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qg.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sk.panjiajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ml.muxihuayi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rd.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tx.colortex.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uv.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rp.szsharing.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dq.szsharing.cn

[B03] switch / match / case
来源：http://oq.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bl.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bi.shtwfgs.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://db.szxytkj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jt.muxihuayi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rk.nszjky.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://it.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bs.jianghongdianzi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sa.panjiajie.cn

[B04] for 计数循环
来源：http://if.yuntaijiaju.cn

Py:   for i in range(10): print(i)
来源：http://rb.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://il.jianghongdianzi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hl.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bn.shxzskj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dw.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vy.yuexingan06.cn

Ruby: 10.times { |i| puts i }
来源：http://nq.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mg.shxzskj.cn

[B05] 遍历数组 / 列表
来源：http://rz.szxytkj.cn

Py:   for item in arr: print(item)
来源：http://nv.huixinmuqiang.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ed.bookmarksfly.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jg.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bx.szxytkj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bl.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qa.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://yq.asd995.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pw.shxzukj.cn

[B06] 遍历字典 / 对象
来源：http://ys.nszjky.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gl.shtwfgs.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fx.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dy.nszjky.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://el.nszjky.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vx.yuntaijiaju.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zq.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vb.lnxyls.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yi.shtwfgs.cn

[B07] while 循环
来源：http://ad.9csxet.cn

Py:   while i < 10: i += 1
来源：http://oy.huanxung.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vn.huanxung.cn

JS:   while (i < 10) { i++; }
来源：http://ly.chemitech.net.cn

TS:   while (i < 10) { i++; }
来源：http://zn.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://wj.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://it.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://pm.9csxet.cn

C#:   while (i < 10) { i++; }
来源：http://mw.asd995.cn

[B08] do-while（至少执行一次）
来源：http://ke.muxihuayi.cn

Py:   # 无 do-while：用 while True + break
来源：http://ty.bjjhwx.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hr.szsharing.cn

JS:   do { i++; } while (i < 10);
来源：http://ct.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://or.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://ds.shxzskj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yq.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pn.haigaiapp.cn

C#:   do { i++; } while (i < 10);
来源：http://pd.shxzukj.cn

[B09] break 与 continue
来源：http://uq.newstarts.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pe.asd995.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kk.gzmigu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gl.hnjuh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qd.yuexingan06.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nm.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gf.lnxyls.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ti.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uw.huixiangedu.cn

[B10] 遍历同时拿索引
来源：http://yd.huixiangedu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dj.asd995.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yb.lnxyls.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vq.lnxyls.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zc.asd995.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hs.huixiangedu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cy.9csxet.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nj.haigaiapp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cv.nicolike.cn

[B11] 生成数字序列 / 区间
来源：http://un.jianghongdianzi.cn

Py:   list(range(0, 10, 2))
来源：http://nx.huanxung.cn

PHP:  range(0, 10, 2);
来源：http://od.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zb.colortex.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eu.bookmarksfly.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sj.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://md.nicolike.cn

Ruby: (0...10).step(2).to_a
来源：http://is.jctech888.com.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ic.jianghongdianzi.cn

[B12] 跳出多层循环
来源：http://zc.wgjwhj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xk.nicolike.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qk.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://iq.wgjwhj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rj.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cl.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cr.bookmarksfly.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://he.haigaiapp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tn.panjiajie.cn

[B13] 判断是否为数字
来源：http://nu.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://eq.gzmigu.cn

PHP:  is_numeric($x)
来源：http://su.521024.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ep.huixiangedu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qc.bjjhwx.cn

Java: x instanceof Number
来源：http://vg.newstarts.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dy.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://ro.shxzukj.cn

C#:   x is int or double or decimal
来源：http://gu.szsharing.cn

[B14] 判断值是否在集合内
来源：http://lq.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pm.shtwfgs.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ka.hnjuh.cn

JS:   [1, 2, 3].includes(x)
来源：http://ew.9csxet.cn

TS:   [1, 2, 3].includes(x)
来源：http://la.haigaiapp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gg.shtwfgs.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xj.wgjwhj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://oh.asd995.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gr.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://kn.521024.cn

Py:   a and b or not c
来源：http://mr.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://dn.gzmigu.cn

JS:   a && b || !c
来源：http://pl.nicolike.cn

TS:   a && b || !c
来源：http://aw.huanxung.cn

Java: a && b || !c
来源：http://wo.haigaiapp.cn

Go:   a && b || !c
来源：http://ue.szxytkj.cn

Ruby: a && b || !c
来源：http://tc.panjiajie.cn

C#:   a && b || !c
来源：http://yg.shxzskj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vh.newstarts.cn

Py:   if not data: return
来源：http://ve.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://ak.jianghongdianzi.cn

JS:   if (!data) return;
来源：http://ve.wgjwhj.cn

TS:   if (!data) return;
来源：http://mp.gzmigu.cn

Java: if (data == null) return;
来源：http://en.hnjuh.cn

Go:   if data == nil { return }
来源：http://ik.nicolike.cn

Ruby: return if data.nil?
来源：http://bf.nicolike.cn

C#:   if (data == null) return;
来源：http://za.yuexingan06.cn

================================================================================
来源：http://jy.shxzukj.cn

C. 函数与作用域
来源：http://yi.hahajie.cn

================================================================================
来源：http://mq.shxzskj.cn

[C01] 定义函数
来源：http://ac.nszjky.cn

Py:   def add(a, b): return a + b
来源：http://ic.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dk.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://zf.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://az.shxzukj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lv.gzmigu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jp.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://am.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nx.shxzskj.cn

[C02] 默认参数
来源：http://nb.bookmarksfly.cn

Py:   def greet(name="World"): return name
来源：http://qb.jctech888.com.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cq.bjjhwx.cn

JS:   function greet(name = "World") { return name; }
来源：http://mv.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ob.jctech888.com.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vi.shxzskj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pw.shxzukj.cn

Ruby: def greet(name = "World") = name
来源：http://uf.panjiajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://mm.shxzskj.cn

[C03] 可变参数
来源：http://hs.shtwfgs.cn

Py:   def total(*args): return sum(args)
来源：http://oc.hnjuh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vt.huixinmuqiang.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kb.9csxet.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jw.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sa.shxzukj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://su.shxzukj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kl.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yt.haigaiapp.cn

[C04] 命名参数 / 关键字参数
来源：http://og.nicolike.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cz.hnjuh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ms.jianghongdianzi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bi.asd995.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kz.hnjuh.cn

Java: // 无：用 Builder 模式或 record
来源：http://jd.chemitech.net.cn

Go:   // 无：用配置结构体参数
来源：http://wj.shtwfgs.cn

Ruby: f(a: 1, b: 2)
来源：http://do.huixinmuqiang.cn

C#:   f(a: 1, b: 2)
来源：http://sf.chemitech.net.cn

[C05] 返回多个值
来源：http://mi.shtwfgs.cn

Py:   return a, b
来源：http://hw.521024.cn

PHP:  return [$a, $b];
来源：http://pe.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ft.szxytkj.cn

TS:   return { a, b };
来源：http://nn.9csxet.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tn.bookmarksfly.cn

Go:   return a, b
来源：http://bb.shxzukj.cn

Ruby: return a, b
来源：http://qk.newstarts.cn

C#:   return (a, b);              // ValueTuple
来源：http://dv.chemitech.net.cn

[C06] 匿名函数 / lambda
来源：http://nm.shtwfgs.cn

Py:   square = lambda x: x * x
来源：http://sm.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wd.yuexingan06.cn

JS:   const square = x => x * x;
来源：http://lt.lnxyls.cn

TS:   const square = (x: number): number => x * x;
来源：http://ka.shxzskj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://br.hnjuh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dc.shxzukj.cn

Ruby: square = ->(x) { x * x }
来源：http://ts.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wq.muxihuayi.cn

[C07] 把函数作为参数传入
来源：http://ef.521024.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qg.asd995.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xt.lnxyls.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nw.lnxyls.cn

TS:   arr.map(String)
来源：http://co.jctech888.com.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wv.nicolike.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rn.colortex.cn

Ruby: arr.map(&:upcase)
来源：http://zl.jianghongdianzi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qp.hnjuh.cn

[C08] 闭包
来源：http://vf.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gu.huanxung.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tt.huanxung.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hr.hnjuh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hq.jianghongdianzi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rw.bjjhwx.cn


<!-- 参考信息 -->