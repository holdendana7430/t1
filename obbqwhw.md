代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://mf.szxytkj.cn

Py:   ord("A"); chr(65)
来源：http://bb.bookmarksfly.cn

PHP:  ord("A"); chr(65)
来源：http://qq.panjiajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gy.lnxyls.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mw.huixinmuqiang.cn

Java: (int) 'A'; (char) 65
来源：http://ye.yuexingan06.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zx.nicolike.cn

Ruby: "A".ord; 65.chr
来源：http://rd.haigaiapp.cn

C#:   (int)'A'; (char)65
来源：http://ib.szxytkj.cn

[A19] 交换两个变量
来源：http://nc.huixinmuqiang.cn

Py:   a, b = b, a
来源：http://of.gzmigu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://gr.hnjuh.cn

JS:   [a, b] = [b, a];
来源：http://ez.jctech888.com.cn

TS:   [a, b] = [b, a];
来源：http://pp.haigaiapp.cn

Java: int t = a; a = b; b = t;
来源：http://ex.shxzskj.cn

Go:   a, b = b, a
来源：http://su.hahajie.cn

Ruby: a, b = b, a
来源：http://nt.shtwfgs.cn

C#:   (a, b) = (b, a);
来源：http://wv.chemitech.net.cn

[A20] 读取标准输入
来源：http://vn.yuexingan06.cn

Py:   name = input("请输入：")
来源：http://bi.nicolike.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://kr.hahajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zj.huanxung.cn

TS:   // Node.js：readline 模块
来源：http://vd.wgjwhj.cn

Java: new Scanner(System.in).nextLine()
来源：http://ed.nszjky.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ag.chemitech.net.cn

Ruby: gets.chomp
来源：http://vs.colortex.cn

C#:   Console.ReadLine();
来源：http://pj.shxzskj.cn

[A21] 保留指定小数位输出
来源：http://gr.shxzskj.cn

Py:   f"{3.14159:.2f}"
来源：http://fs.huanxung.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rn.panjiajie.cn

JS:   (3.14159).toFixed(2)
来源：http://jk.panjiajie.cn

TS:   (3.14159).toFixed(2)
来源：http://wm.asd995.cn

Java: String.format("%.2f", 3.14159)
来源：http://so.lnxyls.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mk.colortex.cn

Ruby: format("%.2f", 3.14159)
来源：http://dh.hnjuh.cn

C#:   3.14159.ToString("F2")
来源：http://iy.yuntaijiaju.cn

[A22] 获取字符串长度
来源：http://jn.nszjky.cn

Py:   len(s)
来源：http://xo.bjjhwx.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tm.521024.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bp.9csxet.cn

TS:   s.length
来源：http://yx.lnxyls.cn

Java: s.length()
来源：http://yd.hahajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dm.hnjuh.cn

Ruby: s.length
来源：http://bt.nszjky.cn

C#:   s.Length
来源：http://jy.gzmigu.cn

[A23] 大小写转换
来源：http://tm.521024.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ki.haigaiapp.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cy.szxytkj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qq.szsharing.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bk.521024.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fu.wgjwhj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kj.gzmigu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ik.muxihuayi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ju.wgjwhj.cn

[A24] 去除首尾空白
来源：http://ev.jianghongdianzi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ey.szxytkj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gb.bjjhwx.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eb.yuexingan06.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ba.521024.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gn.yuexingan06.cn

Go:   strings.TrimSpace(s)
来源：http://re.haigaiapp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kd.gzmigu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fv.asd995.cn

[A25] 字符串比较
来源：http://yb.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://yk.szxytkj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zt.yuexingan06.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pb.jctech888.com.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cz.gzmigu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hf.huixiangedu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ke.muxihuayi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://kg.asd995.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ty.bjjhwx.cn

[A26] 类型转换总览
来源：http://eq.nszjky.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fd.huixiangedu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ws.chemitech.net.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://le.hnjuh.cn

TS:   Number() String() Boolean() x as number
来源：http://xz.bjjhwx.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kc.wgjwhj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pe.jianghongdianzi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://gs.huixinmuqiang.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://su.huixinmuqiang.cn

================================================================================
来源：http://xi.jianghongdianzi.cn

B. 流程控制
来源：http://kr.nszjky.cn

================================================================================
来源：http://mt.jianghongdianzi.cn

[B01] 条件判断 if / else
来源：http://nj.hahajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bs.shtwfgs.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mu.asd995.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://js.nicolike.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fl.panjiajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gj.szsharing.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bk.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ci.gzmigu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cf.nicolike.cn

[B02] 多分支 else if / elif
来源：http://pd.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ko.lnxyls.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://iq.jctech888.com.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tk.nszjky.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jg.yuexingan06.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zf.muxihuayi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jr.muxihuayi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rb.shxzskj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pw.shtwfgs.cn

[B03] switch / match / case
来源：http://mo.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jv.muxihuayi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fk.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dz.panjiajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kh.nicolike.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uj.colortex.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bb.yuexingan06.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lc.bjjhwx.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mi.jctech888.com.cn

[B04] for 计数循环
来源：http://lv.bookmarksfly.cn

Py:   for i in range(10): print(i)
来源：http://ce.huixiangedu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nb.shxzskj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vl.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ay.chemitech.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zg.hnjuh.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pq.hnjuh.cn

Ruby: 10.times { |i| puts i }
来源：http://tk.shtwfgs.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gf.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://yg.bjjhwx.cn

Py:   for item in arr: print(item)
来源：http://pz.jianghongdianzi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wv.shtwfgs.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://iz.wgjwhj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ov.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ti.huixinmuqiang.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vw.asd995.cn

Ruby: arr.each { |item| puts item }
来源：http://ss.szxytkj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gs.huanxung.cn

[B06] 遍历字典 / 对象
来源：http://mi.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cn.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lb.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://po.shtwfgs.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uu.huanxung.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://li.jctech888.com.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lg.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://js.newstarts.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://be.muxihuayi.cn

[B07] while 循环
来源：http://je.hahajie.cn

Py:   while i < 10: i += 1
来源：http://af.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mx.asd995.cn

JS:   while (i < 10) { i++; }
来源：http://dc.shtwfgs.cn

TS:   while (i < 10) { i++; }
来源：http://xc.szxytkj.cn

Java: while (i < 10) { i++; }
来源：http://kp.yuntaijiaju.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ot.hnjuh.cn

Ruby: while i < 10; i += 1; end
来源：http://jd.haigaiapp.cn

C#:   while (i < 10) { i++; }
来源：http://xf.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://bq.yuexingan06.cn

Py:   # 无 do-while：用 while True + break
来源：http://xq.gzmigu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://me.colortex.cn

JS:   do { i++; } while (i < 10);
来源：http://os.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://po.521024.cn

Java: do { i++; } while (i < 10);
来源：http://yd.newstarts.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pp.shtwfgs.cn

Ruby: begin; i += 1; end while i < 10
来源：http://oa.newstarts.cn

C#:   do { i++; } while (i < 10);
来源：http://ar.jctech888.com.cn

[B09] break 与 continue
来源：http://lf.hnjuh.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ux.huixinmuqiang.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jo.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ud.521024.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jb.huanxung.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uj.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wm.szsharing.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yc.gzmigu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wa.colortex.cn

[B10] 遍历同时拿索引
来源：http://oj.nszjky.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ts.nicolike.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gx.nszjky.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ex.yuexingan06.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wo.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fm.nszjky.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://af.jctech888.com.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cr.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bg.nszjky.cn

[B11] 生成数字序列 / 区间
来源：http://ip.gzmigu.cn

Py:   list(range(0, 10, 2))
来源：http://la.asd995.cn

PHP:  range(0, 10, 2);
来源：http://rc.lnxyls.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pr.colortex.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ij.jianghongdianzi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pb.shxzskj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jf.521024.cn

Ruby: (0...10).step(2).to_a
来源：http://xe.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ym.yuntaijiaju.cn

[B12] 跳出多层循环
来源：http://at.521024.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gx.chemitech.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mt.muxihuayi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uq.bookmarksfly.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lp.colortex.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gz.huixinmuqiang.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://js.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rl.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nk.szsharing.cn

[B13] 判断是否为数字
来源：http://dv.hnjuh.cn

Py:   isinstance(x, (int, float))
来源：http://cm.szsharing.cn

PHP:  is_numeric($x)
来源：http://yq.asd995.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ou.jctech888.com.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hk.szsharing.cn

Java: x instanceof Number
来源：http://te.panjiajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ew.bjjhwx.cn

Ruby: x.is_a?(Numeric)
来源：http://ok.wgjwhj.cn

C#:   x is int or double or decimal
来源：http://na.jianghongdianzi.cn

[B14] 判断值是否在集合内
来源：http://du.huixinmuqiang.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kd.gzmigu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pj.nszjky.cn

JS:   [1, 2, 3].includes(x)
来源：http://lm.lnxyls.cn

TS:   [1, 2, 3].includes(x)
来源：http://kz.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://eg.huanxung.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ze.wgjwhj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jp.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qo.huixinmuqiang.cn

[B15] 布尔运算与取反
来源：http://tq.colortex.cn

Py:   a and b or not c
来源：http://yk.hahajie.cn

PHP:  $a && $b || !$c
来源：http://eb.9csxet.cn

JS:   a && b || !c
来源：http://sz.haigaiapp.cn

TS:   a && b || !c
来源：http://vh.bjjhwx.cn

Java: a && b || !c
来源：http://xw.huixinmuqiang.cn

Go:   a && b || !c
来源：http://rt.haigaiapp.cn

Ruby: a && b || !c
来源：http://zj.chemitech.net.cn

C#:   a && b || !c
来源：http://pw.nicolike.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zs.hahajie.cn

Py:   if not data: return
来源：http://pl.yuexingan06.cn

PHP:  if (!$data) { return; }
来源：http://ur.hahajie.cn

JS:   if (!data) return;
来源：http://ix.haigaiapp.cn

TS:   if (!data) return;
来源：http://ow.9csxet.cn

Java: if (data == null) return;
来源：http://ki.szsharing.cn

Go:   if data == nil { return }
来源：http://ym.bookmarksfly.cn

Ruby: return if data.nil?
来源：http://eb.asd995.cn

C#:   if (data == null) return;
来源：http://ku.muxihuayi.cn

================================================================================
来源：http://ye.jianghongdianzi.cn

C. 函数与作用域
来源：http://zo.huixiangedu.cn

================================================================================
来源：http://sw.jianghongdianzi.cn

[C01] 定义函数
来源：http://wq.gzmigu.cn

Py:   def add(a, b): return a + b
来源：http://zo.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tj.asd995.cn

JS:   function add(a, b) { return a + b; }
来源：http://ks.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bg.szxytkj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pc.szsharing.cn

Go:   func add(a, b int) int { return a + b }
来源：http://go.nszjky.cn

Ruby: def add(a, b); a + b; end
来源：http://kx.9csxet.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ay.shtwfgs.cn

[C02] 默认参数
来源：http://rl.gzmigu.cn

Py:   def greet(name="World"): return name
来源：http://vw.hahajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://na.bookmarksfly.cn

JS:   function greet(name = "World") { return name; }
来源：http://vk.hahajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mm.wgjwhj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xf.asd995.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rn.huanxung.cn

Ruby: def greet(name = "World") = name
来源：http://vn.wgjwhj.cn

C#:   string Greet(string name = "World") => name;
来源：http://ti.nszjky.cn

[C03] 可变参数
来源：http://ty.shtwfgs.cn

Py:   def total(*args): return sum(args)
来源：http://em.bookmarksfly.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ts.bjjhwx.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jp.hahajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://at.shxzukj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ln.muxihuayi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://id.gzmigu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xs.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://en.huixinmuqiang.cn

[C04] 命名参数 / 关键字参数
来源：http://sz.yuexingan06.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tz.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sh.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ca.huanxung.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ab.shxzukj.cn

Java: // 无：用 Builder 模式或 record
来源：http://ns.wgjwhj.cn

Go:   // 无：用配置结构体参数
来源：http://wo.chemitech.net.cn

Ruby: f(a: 1, b: 2)
来源：http://ua.newstarts.cn

C#:   f(a: 1, b: 2)
来源：http://lb.shxzukj.cn

[C05] 返回多个值
来源：http://vp.huanxung.cn

Py:   return a, b
来源：http://ib.muxihuayi.cn

PHP:  return [$a, $b];
来源：http://sj.hahajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cb.nszjky.cn

TS:   return { a, b };
来源：http://xw.huanxung.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dd.muxihuayi.cn

Go:   return a, b
来源：http://zv.yuexingan06.cn

Ruby: return a, b
来源：http://ma.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://td.newstarts.cn

[C06] 匿名函数 / lambda
来源：http://nb.wgjwhj.cn

Py:   square = lambda x: x * x
来源：http://im.huanxung.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bt.shxzskj.cn

JS:   const square = x => x * x;
来源：http://bg.haigaiapp.cn

TS:   const square = (x: number): number => x * x;
来源：http://ot.huixiangedu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uj.lnxyls.cn

Go:   sq := func(x int) int { return x * x }
来源：http://am.huanxung.cn

Ruby: square = ->(x) { x * x }
来源：http://ws.chemitech.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zv.newstarts.cn

[C07] 把函数作为参数传入
来源：http://ru.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wk.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qo.huixiangedu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jn.huixiangedu.cn

TS:   arr.map(String)
来源：http://gp.haigaiapp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tg.521024.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fc.newstarts.cn

Ruby: arr.map(&:upcase)
来源：http://tb.wgjwhj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ny.bookmarksfly.cn

[C08] 闭包
来源：http://ar.hnjuh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bx.521024.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xp.yuntaijiaju.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ol.shxzukj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oy.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yw.shxzukj.cn


<!-- 参考信息 -->