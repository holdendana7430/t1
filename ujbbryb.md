代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zf.huixinmuqiang.cn

Java: (int) 'A'; (char) 65
来源：http://ha.521024.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uu.szxytkj.cn

Ruby: "A".ord; 65.chr
来源：http://kd.jianghongdianzi.cn

C#:   (int)'A'; (char)65
来源：http://xx.lnxyls.cn

[A19] 交换两个变量
来源：http://yq.9csxet.cn

Py:   a, b = b, a
来源：http://tq.yuntaijiaju.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://wz.gzmigu.cn

JS:   [a, b] = [b, a];
来源：http://zi.nszjky.cn

TS:   [a, b] = [b, a];
来源：http://xj.huixinmuqiang.cn

Java: int t = a; a = b; b = t;
来源：http://et.szxytkj.cn

Go:   a, b = b, a
来源：http://ed.szsharing.cn

Ruby: a, b = b, a
来源：http://ql.haigaiapp.cn

C#:   (a, b) = (b, a);
来源：http://fr.521024.cn

[A20] 读取标准输入
来源：http://zj.szsharing.cn

Py:   name = input("请输入：")
来源：http://fp.bjjhwx.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://uc.hahajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mm.huixinmuqiang.cn

TS:   // Node.js：readline 模块
来源：http://fe.huanxung.cn

Java: new Scanner(System.in).nextLine()
来源：http://hq.szxytkj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cd.jctech888.com.cn

Ruby: gets.chomp
来源：http://ke.jctech888.com.cn

C#:   Console.ReadLine();
来源：http://ze.9csxet.cn

[A21] 保留指定小数位输出
来源：http://ja.newstarts.cn

Py:   f"{3.14159:.2f}"
来源：http://eu.hnjuh.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bz.panjiajie.cn

JS:   (3.14159).toFixed(2)
来源：http://es.shtwfgs.cn

TS:   (3.14159).toFixed(2)
来源：http://qp.colortex.cn

Java: String.format("%.2f", 3.14159)
来源：http://fy.9csxet.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ft.colortex.cn

Ruby: format("%.2f", 3.14159)
来源：http://yb.shxzskj.cn

C#:   3.14159.ToString("F2")
来源：http://pt.colortex.cn

[A22] 获取字符串长度
来源：http://el.haigaiapp.cn

Py:   len(s)
来源：http://zj.wgjwhj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://if.nicolike.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rn.colortex.cn

TS:   s.length
来源：http://mp.shxzukj.cn

Java: s.length()
来源：http://lg.gzmigu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sy.panjiajie.cn

Ruby: s.length
来源：http://hv.nicolike.cn

C#:   s.Length
来源：http://hq.jctech888.com.cn

[A23] 大小写转换
来源：http://sw.shxzukj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wu.gzmigu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ot.shtwfgs.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nb.newstarts.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lc.gzmigu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rd.szsharing.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jr.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jh.panjiajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ab.szxytkj.cn

[A24] 去除首尾空白
来源：http://aw.haigaiapp.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tn.shxzukj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gj.9csxet.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ws.yuexingan06.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://af.newstarts.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ph.nszjky.cn

Go:   strings.TrimSpace(s)
来源：http://zb.bookmarksfly.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ph.bjjhwx.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tg.colortex.cn

[A25] 字符串比较
来源：http://js.jctech888.com.cn

Py:   s1 == s2; s1 != s2
来源：http://rv.9csxet.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pw.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://my.shtwfgs.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://el.nszjky.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cl.gzmigu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rv.gzmigu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vj.chemitech.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://le.yuntaijiaju.cn

[A26] 类型转换总览
来源：http://yl.yuntaijiaju.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ck.shxzukj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zt.szsharing.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ht.huixinmuqiang.cn

TS:   Number() String() Boolean() x as number
来源：http://fp.shxzukj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cw.nicolike.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://em.nicolike.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qi.shtwfgs.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://af.szsharing.cn

================================================================================
来源：http://lw.asd995.cn

B. 流程控制
来源：http://kv.nicolike.cn

================================================================================
来源：http://gt.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://gk.9csxet.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fy.huixinmuqiang.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bo.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://uz.nicolike.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uc.wgjwhj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://yh.hnjuh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qw.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sc.asd995.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rr.newstarts.cn

[B02] 多分支 else if / elif
来源：http://yk.hahajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cl.lnxyls.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fk.hahajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oc.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://io.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://be.panjiajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://su.bjjhwx.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zg.yuexingan06.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ef.newstarts.cn

[B03] switch / match / case
来源：http://oq.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bp.huixiangedu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cq.bookmarksfly.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bm.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nj.jianghongdianzi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pc.asd995.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cd.colortex.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bo.asd995.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uh.lnxyls.cn

[B04] for 计数循环
来源：http://ab.huixiangedu.cn

Py:   for i in range(10): print(i)
来源：http://hp.jctech888.com.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kt.shxzskj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://la.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ui.huanxung.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://br.hahajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kx.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://xf.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mk.nicolike.cn

[B05] 遍历数组 / 列表
来源：http://sh.9csxet.cn

Py:   for item in arr: print(item)
来源：http://ww.hnjuh.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lg.9csxet.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xp.asd995.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hj.hnjuh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fk.wgjwhj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bv.haigaiapp.cn

Ruby: arr.each { |item| puts item }
来源：http://wg.colortex.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cs.chemitech.net.cn

[B06] 遍历字典 / 对象
来源：http://pq.huanxung.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pd.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zd.bjjhwx.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bs.bjjhwx.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://in.szxytkj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qj.yuexingan06.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rq.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ia.newstarts.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://td.9csxet.cn

[B07] while 循环
来源：http://rd.colortex.cn

Py:   while i < 10: i += 1
来源：http://kn.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://au.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://bf.muxihuayi.cn

TS:   while (i < 10) { i++; }
来源：http://li.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://gx.shxzskj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sv.lnxyls.cn

Ruby: while i < 10; i += 1; end
来源：http://nc.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://yv.shtwfgs.cn

[B08] do-while（至少执行一次）
来源：http://uk.haigaiapp.cn

Py:   # 无 do-while：用 while True + break
来源：http://hb.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kx.huanxung.cn

JS:   do { i++; } while (i < 10);
来源：http://pj.jctech888.com.cn

TS:   do { i++; } while (i < 10);
来源：http://ao.9csxet.cn

Java: do { i++; } while (i < 10);
来源：http://gg.newstarts.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://as.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vp.9csxet.cn

C#:   do { i++; } while (i < 10);
来源：http://gy.shtwfgs.cn

[B09] break 与 continue
来源：http://mx.hnjuh.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gr.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xt.gzmigu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pd.lnxyls.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yp.yuexingan06.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cn.jianghongdianzi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ln.huixiangedu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ff.muxihuayi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rp.muxihuayi.cn

[B10] 遍历同时拿索引
来源：http://ez.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://of.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qf.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dq.bjjhwx.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://as.9csxet.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yv.jianghongdianzi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bu.haigaiapp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nh.newstarts.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://np.hahajie.cn

[B11] 生成数字序列 / 区间
来源：http://rd.huixiangedu.cn

Py:   list(range(0, 10, 2))
来源：http://mu.asd995.cn

PHP:  range(0, 10, 2);
来源：http://gk.newstarts.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pq.jianghongdianzi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tb.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kw.hnjuh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zg.bookmarksfly.cn

Ruby: (0...10).step(2).to_a
来源：http://uc.panjiajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gt.yuntaijiaju.cn

[B12] 跳出多层循环
来源：http://zz.jianghongdianzi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uu.huixinmuqiang.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tn.jctech888.com.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qx.newstarts.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ry.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://go.jianghongdianzi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yc.chemitech.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ih.huanxung.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wq.huixiangedu.cn

[B13] 判断是否为数字
来源：http://xu.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://xe.yuntaijiaju.cn

PHP:  is_numeric($x)
来源：http://vg.jianghongdianzi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zi.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tu.jianghongdianzi.cn

Java: x instanceof Number
来源：http://mz.yuntaijiaju.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ng.bookmarksfly.cn

Ruby: x.is_a?(Numeric)
来源：http://ep.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://bt.lnxyls.cn

[B14] 判断值是否在集合内
来源：http://ws.chemitech.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vy.huixinmuqiang.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://au.jianghongdianzi.cn

JS:   [1, 2, 3].includes(x)
来源：http://ud.jianghongdianzi.cn

TS:   [1, 2, 3].includes(x)
来源：http://yv.lnxyls.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lw.lnxyls.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yb.nicolike.cn

Ruby: [1, 2, 3].include?(x)
来源：http://db.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tq.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://ef.huixiangedu.cn

Py:   a and b or not c
来源：http://ms.muxihuayi.cn

PHP:  $a && $b || !$c
来源：http://mw.yuexingan06.cn

JS:   a && b || !c
来源：http://rc.wgjwhj.cn

TS:   a && b || !c
来源：http://wy.szxytkj.cn

Java: a && b || !c
来源：http://dm.hnjuh.cn

Go:   a && b || !c
来源：http://zw.newstarts.cn

Ruby: a && b || !c
来源：http://wo.hahajie.cn

C#:   a && b || !c
来源：http://ic.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ty.hahajie.cn

Py:   if not data: return
来源：http://uk.bookmarksfly.cn

PHP:  if (!$data) { return; }
来源：http://rn.hnjuh.cn

JS:   if (!data) return;
来源：http://vw.9csxet.cn

TS:   if (!data) return;
来源：http://ci.nszjky.cn

Java: if (data == null) return;
来源：http://il.gzmigu.cn

Go:   if data == nil { return }
来源：http://kk.shxzskj.cn

Ruby: return if data.nil?
来源：http://hx.nszjky.cn

C#:   if (data == null) return;
来源：http://mx.szsharing.cn

================================================================================
来源：http://qh.haigaiapp.cn

C. 函数与作用域
来源：http://qw.huixinmuqiang.cn

================================================================================
来源：http://hb.shxzukj.cn

[C01] 定义函数
来源：http://my.jianghongdianzi.cn

Py:   def add(a, b): return a + b
来源：http://se.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zn.huixinmuqiang.cn

JS:   function add(a, b) { return a + b; }
来源：http://ip.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zy.wgjwhj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sv.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jo.panjiajie.cn

Ruby: def add(a, b); a + b; end
来源：http://hd.jianghongdianzi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kb.jianghongdianzi.cn

[C02] 默认参数
来源：http://bb.szxytkj.cn

Py:   def greet(name="World"): return name
来源：http://bo.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://me.haigaiapp.cn

JS:   function greet(name = "World") { return name; }
来源：http://tg.shxzskj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zm.nszjky.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zb.jctech888.com.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lc.huixinmuqiang.cn

Ruby: def greet(name = "World") = name
来源：http://hr.shtwfgs.cn

C#:   string Greet(string name = "World") => name;
来源：http://wh.wgjwhj.cn

[C03] 可变参数
来源：http://nc.panjiajie.cn

Py:   def total(*args): return sum(args)
来源：http://le.nszjky.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://di.hnjuh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gz.shtwfgs.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zu.bookmarksfly.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xb.nicolike.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vn.huixinmuqiang.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zy.hnjuh.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yi.jianghongdianzi.cn

[C04] 命名参数 / 关键字参数
来源：http://cd.nicolike.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://en.521024.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qn.jianghongdianzi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xi.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fg.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://sc.hahajie.cn

Go:   // 无：用配置结构体参数
来源：http://hc.bookmarksfly.cn

Ruby: f(a: 1, b: 2)
来源：http://vt.yuntaijiaju.cn

C#:   f(a: 1, b: 2)
来源：http://zo.shxzskj.cn

[C05] 返回多个值
来源：http://tq.jctech888.com.cn

Py:   return a, b
来源：http://vv.hahajie.cn

PHP:  return [$a, $b];
来源：http://bc.chemitech.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://je.haigaiapp.cn

TS:   return { a, b };
来源：http://pr.asd995.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yi.huixiangedu.cn

Go:   return a, b
来源：http://wc.colortex.cn

Ruby: return a, b
来源：http://qm.shxzskj.cn

C#:   return (a, b);              // ValueTuple
来源：http://hj.bjjhwx.cn

[C06] 匿名函数 / lambda
来源：http://xn.hahajie.cn

Py:   square = lambda x: x * x
来源：http://wh.bookmarksfly.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qz.huixinmuqiang.cn

JS:   const square = x => x * x;
来源：http://nf.panjiajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://ay.jianghongdianzi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hl.colortex.cn

Go:   sq := func(x int) int { return x * x }
来源：http://of.szsharing.cn

Ruby: square = ->(x) { x * x }
来源：http://hd.nicolike.cn

C#:   Func<int, int> square = x => x * x;
来源：http://sc.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://et.gzmigu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ob.haigaiapp.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cb.nszjky.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tw.shtwfgs.cn

TS:   arr.map(String)
来源：http://xw.hnjuh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qb.muxihuayi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zz.521024.cn

Ruby: arr.map(&:upcase)
来源：http://iv.jianghongdianzi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bz.panjiajie.cn

[C08] 闭包
来源：http://on.asd995.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qt.muxihuayi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ix.bookmarksfly.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kw.gzmigu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qy.bjjhwx.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://iy.jctech888.com.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kt.521024.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hj.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ho.yuexingan06.cn

[C09] 递归
来源：http://xk.jianghongdianzi.cn


<!-- 参考信息 -->