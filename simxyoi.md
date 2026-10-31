代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://eg.chemitech.net.cn

TS:   const value = data ?? "默认值";
来源：http://ux.newstarts.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://sw.lnxyls.cn

Go:   if data == "" { data = "默认值" }
来源：http://pz.huanxung.cn

Ruby: value = data || "默认值"
来源：http://ex.huixinmuqiang.cn

C#:   var value = data ?? "默认值";
来源：http://zk.yuexingan06.cn

[A16] 真假值判断规则
来源：http://my.szxytkj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vy.jctech888.com.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lj.shtwfgs.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ig.asd995.cn

TS:   if (!x) {}
来源：http://he.shtwfgs.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ms.hahajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hn.panjiajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hd.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ui.nicolike.cn

[A17] 位运算
来源：http://na.shxzskj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xs.szsharing.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dl.nszjky.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ac.huanxung.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://do.huanxung.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ad.nszjky.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ib.szsharing.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kn.chemitech.net.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nh.nszjky.cn

[A18] 字符与 ASCII 码互转
来源：http://hu.szsharing.cn

Py:   ord("A"); chr(65)
来源：http://eq.chemitech.net.cn

PHP:  ord("A"); chr(65)
来源：http://el.521024.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qj.wgjwhj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ts.wgjwhj.cn

Java: (int) 'A'; (char) 65
来源：http://wr.newstarts.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hq.huanxung.cn

Ruby: "A".ord; 65.chr
来源：http://mu.panjiajie.cn

C#:   (int)'A'; (char)65
来源：http://dp.muxihuayi.cn

[A19] 交换两个变量
来源：http://ny.wgjwhj.cn

Py:   a, b = b, a
来源：http://qc.shtwfgs.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yh.muxihuayi.cn

JS:   [a, b] = [b, a];
来源：http://pp.yuexingan06.cn

TS:   [a, b] = [b, a];
来源：http://ln.szxytkj.cn

Java: int t = a; a = b; b = t;
来源：http://ue.jctech888.com.cn

Go:   a, b = b, a
来源：http://ak.colortex.cn

Ruby: a, b = b, a
来源：http://tz.shtwfgs.cn

C#:   (a, b) = (b, a);
来源：http://ze.yuntaijiaju.cn

[A20] 读取标准输入
来源：http://vu.huanxung.cn

Py:   name = input("请输入：")
来源：http://jb.shtwfgs.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ag.chemitech.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qe.shxzukj.cn

TS:   // Node.js：readline 模块
来源：http://xs.521024.cn

Java: new Scanner(System.in).nextLine()
来源：http://wv.huixinmuqiang.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ev.asd995.cn

Ruby: gets.chomp
来源：http://dg.colortex.cn

C#:   Console.ReadLine();
来源：http://as.hahajie.cn

[A21] 保留指定小数位输出
来源：http://bn.shxzukj.cn

Py:   f"{3.14159:.2f}"
来源：http://hz.szsharing.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ml.bjjhwx.cn

JS:   (3.14159).toFixed(2)
来源：http://yn.newstarts.cn

TS:   (3.14159).toFixed(2)
来源：http://ty.9csxet.cn

Java: String.format("%.2f", 3.14159)
来源：http://al.521024.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ge.colortex.cn

Ruby: format("%.2f", 3.14159)
来源：http://re.lnxyls.cn

C#:   3.14159.ToString("F2")
来源：http://em.jctech888.com.cn

[A22] 获取字符串长度
来源：http://km.shtwfgs.cn

Py:   len(s)
来源：http://qq.nicolike.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xv.9csxet.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wj.asd995.cn

TS:   s.length
来源：http://ly.panjiajie.cn

Java: s.length()
来源：http://xv.asd995.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nl.shxzskj.cn

Ruby: s.length
来源：http://gn.bookmarksfly.cn

C#:   s.Length
来源：http://je.hahajie.cn

[A23] 大小写转换
来源：http://fu.521024.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://yk.hnjuh.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xy.9csxet.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hc.jctech888.com.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ze.jctech888.com.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://iw.wgjwhj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pd.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gf.hahajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://eu.asd995.cn

[A24] 去除首尾空白
来源：http://ts.521024.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xj.huixinmuqiang.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://go.jianghongdianzi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vb.gzmigu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yk.muxihuayi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kw.muxihuayi.cn

Go:   strings.TrimSpace(s)
来源：http://og.szxytkj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rd.huixinmuqiang.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vt.huanxung.cn

[A25] 字符串比较
来源：http://ql.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://jw.bookmarksfly.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qp.szxytkj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gn.haigaiapp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fw.shtwfgs.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ft.nicolike.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fy.shxzskj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rv.szxytkj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lj.jianghongdianzi.cn

[A26] 类型转换总览
来源：http://dm.haigaiapp.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fe.panjiajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ae.9csxet.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://co.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://am.bookmarksfly.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mw.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nq.panjiajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ff.9csxet.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tg.huixiangedu.cn

================================================================================
来源：http://di.panjiajie.cn

B. 流程控制
来源：http://re.huixinmuqiang.cn

================================================================================
来源：http://xk.shxzukj.cn

[B01] 条件判断 if / else
来源：http://xe.jianghongdianzi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://kz.haigaiapp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rb.nicolike.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://as.lnxyls.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://et.huanxung.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sd.colortex.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jg.nicolike.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://iq.shxzukj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gl.yuntaijiaju.cn

[B02] 多分支 else if / elif
来源：http://vb.hnjuh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hj.521024.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lf.asd995.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nx.nicolike.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xq.asd995.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bv.nszjky.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cz.shxzskj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cu.bookmarksfly.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ga.haigaiapp.cn

[B03] switch / match / case
来源：http://ul.9csxet.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nw.shtwfgs.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cu.shtwfgs.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lt.shxzukj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mx.lnxyls.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cp.jctech888.com.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cm.szxytkj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pe.shtwfgs.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tx.shxzukj.cn

[B04] for 计数循环
来源：http://ky.hahajie.cn

Py:   for i in range(10): print(i)
来源：http://rr.wgjwhj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fq.colortex.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://su.lnxyls.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xc.shxzskj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ky.521024.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zp.huixinmuqiang.cn

Ruby: 10.times { |i| puts i }
来源：http://mi.bjjhwx.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ey.lnxyls.cn

[B05] 遍历数组 / 列表
来源：http://tm.hahajie.cn

Py:   for item in arr: print(item)
来源：http://ux.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xu.hahajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://us.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kj.huixiangedu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ik.nszjky.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hp.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://ry.hahajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rp.huixinmuqiang.cn

[B06] 遍历字典 / 对象
来源：http://ur.asd995.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ci.shxzskj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lc.huixiangedu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ey.hnjuh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ls.hahajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://je.nszjky.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jg.bjjhwx.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vi.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jd.newstarts.cn

[B07] while 循环
来源：http://re.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://wc.shtwfgs.cn

PHP:  while ($i < 10) { $i++; }
来源：http://as.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://lc.hnjuh.cn

TS:   while (i < 10) { i++; }
来源：http://fr.gzmigu.cn

Java: while (i < 10) { i++; }
来源：http://pf.wgjwhj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ma.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://tx.chemitech.net.cn

C#:   while (i < 10) { i++; }
来源：http://iq.colortex.cn

[B08] do-while（至少执行一次）
来源：http://ey.panjiajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://us.asd995.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nx.szsharing.cn

JS:   do { i++; } while (i < 10);
来源：http://lf.yuntaijiaju.cn

TS:   do { i++; } while (i < 10);
来源：http://iu.nicolike.cn

Java: do { i++; } while (i < 10);
来源：http://ht.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jp.newstarts.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kn.huanxung.cn

C#:   do { i++; } while (i < 10);
来源：http://pu.lnxyls.cn

[B09] break 与 continue
来源：http://ul.haigaiapp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ee.nicolike.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eu.haigaiapp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qi.shxzskj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uz.9csxet.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nd.bookmarksfly.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oz.jctech888.com.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ub.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eu.nszjky.cn

[B10] 遍历同时拿索引
来源：http://jv.huixiangedu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ns.shxzukj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ys.bjjhwx.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ek.huanxung.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ui.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zx.chemitech.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xn.nicolike.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ne.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ip.bjjhwx.cn

[B11] 生成数字序列 / 区间
来源：http://ea.huixiangedu.cn

Py:   list(range(0, 10, 2))
来源：http://go.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://xl.gzmigu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hr.huixinmuqiang.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.panjiajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://al.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mx.chemitech.net.cn

Ruby: (0...10).step(2).to_a
来源：http://xk.nszjky.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zx.521024.cn

[B12] 跳出多层循环
来源：http://pt.shxzskj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vt.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kg.huixiangedu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ol.wgjwhj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uv.jctech888.com.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sa.huixiangedu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://eu.asd995.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oq.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mr.hnjuh.cn

[B13] 判断是否为数字
来源：http://ps.newstarts.cn

Py:   isinstance(x, (int, float))
来源：http://vz.wgjwhj.cn

PHP:  is_numeric($x)
来源：http://yp.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://em.nszjky.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cx.szxytkj.cn

Java: x instanceof Number
来源：http://ye.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lf.hnjuh.cn

Ruby: x.is_a?(Numeric)
来源：http://tj.szxytkj.cn

C#:   x is int or double or decimal
来源：http://tx.muxihuayi.cn

[B14] 判断值是否在集合内
来源：http://zn.huanxung.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lw.shtwfgs.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zj.jianghongdianzi.cn

JS:   [1, 2, 3].includes(x)
来源：http://tu.nszjky.cn

TS:   [1, 2, 3].includes(x)
来源：http://gt.panjiajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hi.shxzukj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cv.muxihuayi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dv.yuexingan06.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zy.szsharing.cn

[B15] 布尔运算与取反
来源：http://th.newstarts.cn

Py:   a and b or not c
来源：http://fa.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://pn.szxytkj.cn

JS:   a && b || !c
来源：http://cx.panjiajie.cn

TS:   a && b || !c
来源：http://ei.szxytkj.cn

Java: a && b || !c
来源：http://jf.szsharing.cn

Go:   a && b || !c
来源：http://eo.colortex.cn

Ruby: a && b || !c
来源：http://cb.bjjhwx.cn

C#:   a && b || !c
来源：http://uc.szsharing.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ed.colortex.cn

Py:   if not data: return
来源：http://ey.chemitech.net.cn

PHP:  if (!$data) { return; }
来源：http://di.yuntaijiaju.cn

JS:   if (!data) return;
来源：http://zg.chemitech.net.cn

TS:   if (!data) return;
来源：http://zd.shxzukj.cn

Java: if (data == null) return;
来源：http://zg.bjjhwx.cn

Go:   if data == nil { return }
来源：http://uc.szsharing.cn

Ruby: return if data.nil?
来源：http://px.shxzskj.cn

C#:   if (data == null) return;
来源：http://qx.haigaiapp.cn

================================================================================
来源：http://hq.shxzukj.cn

C. 函数与作用域
来源：http://zj.bookmarksfly.cn

================================================================================
来源：http://dq.newstarts.cn

[C01] 定义函数
来源：http://qb.9csxet.cn

Py:   def add(a, b): return a + b
来源：http://ee.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ye.bjjhwx.cn

JS:   function add(a, b) { return a + b; }
来源：http://sg.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lp.hnjuh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://uj.muxihuayi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ro.haigaiapp.cn

Ruby: def add(a, b); a + b; end
来源：http://ih.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ql.wgjwhj.cn

[C02] 默认参数
来源：http://ea.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://xc.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nl.gzmigu.cn

JS:   function greet(name = "World") { return name; }
来源：http://xn.haigaiapp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xc.panjiajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qi.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rc.bookmarksfly.cn

Ruby: def greet(name = "World") = name
来源：http://ux.jianghongdianzi.cn

C#:   string Greet(string name = "World") => name;
来源：http://ip.chemitech.net.cn

[C03] 可变参数
来源：http://ov.yuntaijiaju.cn

Py:   def total(*args): return sum(args)
来源：http://bw.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sb.shtwfgs.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://am.bookmarksfly.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fm.huixinmuqiang.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ck.chemitech.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ko.szsharing.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pe.hnjuh.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fv.haigaiapp.cn

[C04] 命名参数 / 关键字参数
来源：http://is.panjiajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hu.nszjky.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jc.szsharing.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ud.521024.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ny.shtwfgs.cn

Java: // 无：用 Builder 模式或 record
来源：http://hb.gzmigu.cn

Go:   // 无：用配置结构体参数
来源：http://wx.chemitech.net.cn

Ruby: f(a: 1, b: 2)
来源：http://yv.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://lf.huixiangedu.cn

[C05] 返回多个值
来源：http://hz.shtwfgs.cn

Py:   return a, b
来源：http://fz.shxzskj.cn

PHP:  return [$a, $b];
来源：http://xv.bookmarksfly.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rv.nszjky.cn

TS:   return { a, b };
来源：http://xf.newstarts.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://es.nszjky.cn

Go:   return a, b
来源：http://sw.yuntaijiaju.cn

Ruby: return a, b
来源：http://ab.colortex.cn

C#:   return (a, b);              // ValueTuple
来源：http://xr.shxzskj.cn


<!-- 参考信息 -->