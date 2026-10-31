代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rs.9csxet.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sy.colortex.cn

TS:   if (!x) {}
来源：http://vo.nicolike.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nz.hahajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ve.huixinmuqiang.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ja.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nx.panjiajie.cn

[A17] 位运算
来源：http://lh.huixinmuqiang.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://in.jctech888.com.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ru.hahajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pm.haigaiapp.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://oh.521024.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ie.yuexingan06.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nq.szxytkj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://so.muxihuayi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pq.hahajie.cn

[A18] 字符与 ASCII 码互转
来源：http://cd.asd995.cn

Py:   ord("A"); chr(65)
来源：http://de.szsharing.cn

PHP:  ord("A"); chr(65)
来源：http://im.huixinmuqiang.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oq.muxihuayi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://if.shxzukj.cn

Java: (int) 'A'; (char) 65
来源：http://mg.asd995.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yg.gzmigu.cn

Ruby: "A".ord; 65.chr
来源：http://fu.chemitech.net.cn

C#:   (int)'A'; (char)65
来源：http://jw.panjiajie.cn

[A19] 交换两个变量
来源：http://ke.shtwfgs.cn

Py:   a, b = b, a
来源：http://ep.colortex.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://gb.jianghongdianzi.cn

JS:   [a, b] = [b, a];
来源：http://vk.huixinmuqiang.cn

TS:   [a, b] = [b, a];
来源：http://py.chemitech.net.cn

Java: int t = a; a = b; b = t;
来源：http://fo.yuntaijiaju.cn

Go:   a, b = b, a
来源：http://no.521024.cn

Ruby: a, b = b, a
来源：http://ig.jianghongdianzi.cn

C#:   (a, b) = (b, a);
来源：http://oe.shxzskj.cn

[A20] 读取标准输入
来源：http://ng.shxzukj.cn

Py:   name = input("请输入：")
来源：http://re.nicolike.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qp.huixiangedu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rx.hnjuh.cn

TS:   // Node.js：readline 模块
来源：http://yy.haigaiapp.cn

Java: new Scanner(System.in).nextLine()
来源：http://ba.szxytkj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pl.yuexingan06.cn

Ruby: gets.chomp
来源：http://xi.521024.cn

C#:   Console.ReadLine();
来源：http://wa.newstarts.cn

[A21] 保留指定小数位输出
来源：http://jc.9csxet.cn

Py:   f"{3.14159:.2f}"
来源：http://ea.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zp.hnjuh.cn

JS:   (3.14159).toFixed(2)
来源：http://fo.haigaiapp.cn

TS:   (3.14159).toFixed(2)
来源：http://sl.haigaiapp.cn

Java: String.format("%.2f", 3.14159)
来源：http://jc.jctech888.com.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ok.jctech888.com.cn

Ruby: format("%.2f", 3.14159)
来源：http://cq.9csxet.cn

C#:   3.14159.ToString("F2")
来源：http://rn.9csxet.cn

[A22] 获取字符串长度
来源：http://gm.hahajie.cn

Py:   len(s)
来源：http://it.newstarts.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yv.newstarts.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kc.newstarts.cn

TS:   s.length
来源：http://dp.huanxung.cn

Java: s.length()
来源：http://qo.hnjuh.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ze.jctech888.com.cn

Ruby: s.length
来源：http://zg.jianghongdianzi.cn

C#:   s.Length
来源：http://pv.huixinmuqiang.cn

[A23] 大小写转换
来源：http://hz.panjiajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hn.nicolike.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://eg.huixinmuqiang.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rl.huixinmuqiang.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wc.haigaiapp.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://be.newstarts.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cf.9csxet.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ej.jianghongdianzi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hh.521024.cn

[A24] 去除首尾空白
来源：http://av.jctech888.com.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wk.jianghongdianzi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qp.9csxet.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lh.gzmigu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qz.nszjky.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nt.jctech888.com.cn

Go:   strings.TrimSpace(s)
来源：http://nq.yuntaijiaju.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://js.newstarts.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://df.jctech888.com.cn

[A25] 字符串比较
来源：http://ez.bookmarksfly.cn

Py:   s1 == s2; s1 != s2
来源：http://kq.jianghongdianzi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wd.jctech888.com.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pd.yuexingan06.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jf.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yc.jianghongdianzi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hn.huanxung.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cl.shtwfgs.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uv.yuexingan06.cn

[A26] 类型转换总览
来源：http://mc.yuntaijiaju.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uc.huanxung.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ou.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://if.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://mn.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gx.wgjwhj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tm.huanxung.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mb.shtwfgs.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sp.bjjhwx.cn

================================================================================
来源：http://bw.yuexingan06.cn

B. 流程控制
来源：http://vm.521024.cn

================================================================================
来源：http://oy.chemitech.net.cn

[B01] 条件判断 if / else
来源：http://lu.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ut.gzmigu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bu.wgjwhj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gu.huixinmuqiang.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kq.huanxung.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://el.bookmarksfly.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zu.jctech888.com.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://so.jctech888.com.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ri.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://oa.colortex.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ms.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hr.hnjuh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sj.nicolike.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xh.521024.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fy.muxihuayi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yf.nszjky.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yy.yuexingan06.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ao.shtwfgs.cn

[B03] switch / match / case
来源：http://ft.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://et.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uw.muxihuayi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lw.colortex.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ql.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://om.lnxyls.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gf.huanxung.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kw.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://al.yuexingan06.cn

[B04] for 计数循环
来源：http://ey.gzmigu.cn

Py:   for i in range(10): print(i)
来源：http://st.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ck.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oc.haigaiapp.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cl.yuexingan06.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bj.huixinmuqiang.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hr.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://nj.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nr.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://go.szxytkj.cn

Py:   for item in arr: print(item)
来源：http://tq.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://op.hahajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ta.wgjwhj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hh.wgjwhj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hg.shxzukj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nh.haigaiapp.cn

Ruby: arr.each { |item| puts item }
来源：http://ln.colortex.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rt.521024.cn

[B06] 遍历字典 / 对象
来源：http://sb.hnjuh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wo.gzmigu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uv.haigaiapp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oa.muxihuayi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qd.yuntaijiaju.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oi.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nf.jctech888.com.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kd.gzmigu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ey.521024.cn

[B07] while 循环
来源：http://ex.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://tk.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pl.szxytkj.cn

JS:   while (i < 10) { i++; }
来源：http://nc.nszjky.cn

TS:   while (i < 10) { i++; }
来源：http://sw.bjjhwx.cn

Java: while (i < 10) { i++; }
来源：http://rv.lnxyls.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://em.lnxyls.cn

Ruby: while i < 10; i += 1; end
来源：http://ze.huixiangedu.cn

C#:   while (i < 10) { i++; }
来源：http://zs.yuexingan06.cn

[B08] do-while（至少执行一次）
来源：http://mz.521024.cn

Py:   # 无 do-while：用 while True + break
来源：http://hn.yuexingan06.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yk.shxzukj.cn

JS:   do { i++; } while (i < 10);
来源：http://nl.521024.cn

TS:   do { i++; } while (i < 10);
来源：http://yj.shxzskj.cn

Java: do { i++; } while (i < 10);
来源：http://qn.jianghongdianzi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wj.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hq.jianghongdianzi.cn

C#:   do { i++; } while (i < 10);
来源：http://cb.szxytkj.cn

[B09] break 与 continue
来源：http://xy.muxihuayi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qe.jctech888.com.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nc.muxihuayi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.chemitech.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://an.shxzukj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yf.chemitech.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://we.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zi.9csxet.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pj.hahajie.cn

[B10] 遍历同时拿索引
来源：http://nr.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kx.bjjhwx.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gd.bjjhwx.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tn.wgjwhj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uc.jianghongdianzi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kp.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vz.panjiajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pl.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zm.haigaiapp.cn

[B11] 生成数字序列 / 区间
来源：http://lf.panjiajie.cn

Py:   list(range(0, 10, 2))
来源：http://im.asd995.cn

PHP:  range(0, 10, 2);
来源：http://fe.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oa.szsharing.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yb.shxzskj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ec.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sx.nszjky.cn

Ruby: (0...10).step(2).to_a
来源：http://nw.yuntaijiaju.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://au.jianghongdianzi.cn

[B12] 跳出多层循环
来源：http://wt.shxzukj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bz.panjiajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jz.nicolike.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bt.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yl.lnxyls.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://td.newstarts.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vg.shxzskj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jb.hnjuh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cp.wgjwhj.cn

[B13] 判断是否为数字
来源：http://th.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://zl.colortex.cn

PHP:  is_numeric($x)
来源：http://ov.chemitech.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lz.wgjwhj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bi.bjjhwx.cn

Java: x instanceof Number
来源：http://np.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://aa.szsharing.cn

Ruby: x.is_a?(Numeric)
来源：http://az.newstarts.cn

C#:   x is int or double or decimal
来源：http://wm.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://eo.nszjky.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://th.hnjuh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dj.huixinmuqiang.cn

JS:   [1, 2, 3].includes(x)
来源：http://go.wgjwhj.cn

TS:   [1, 2, 3].includes(x)
来源：http://hv.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://my.yuexingan06.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ki.yuexingan06.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qe.haigaiapp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nd.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://vt.nicolike.cn

Py:   a and b or not c
来源：http://ws.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://jg.panjiajie.cn

JS:   a && b || !c
来源：http://rn.gzmigu.cn

TS:   a && b || !c
来源：http://zm.jianghongdianzi.cn

Java: a && b || !c
来源：http://ce.gzmigu.cn

Go:   a && b || !c
来源：http://uk.szsharing.cn

Ruby: a && b || !c
来源：http://hd.bookmarksfly.cn

C#:   a && b || !c
来源：http://gw.jctech888.com.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vf.yuexingan06.cn

Py:   if not data: return
来源：http://dp.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://vn.nicolike.cn

JS:   if (!data) return;
来源：http://vs.chemitech.net.cn

TS:   if (!data) return;
来源：http://wp.shtwfgs.cn

Java: if (data == null) return;
来源：http://cb.yuntaijiaju.cn

Go:   if data == nil { return }
来源：http://hx.9csxet.cn

Ruby: return if data.nil?
来源：http://ph.muxihuayi.cn

C#:   if (data == null) return;
来源：http://sn.szsharing.cn

================================================================================
来源：http://yz.colortex.cn

C. 函数与作用域
来源：http://wi.jianghongdianzi.cn

================================================================================
来源：http://tv.bjjhwx.cn

[C01] 定义函数
来源：http://gk.9csxet.cn

Py:   def add(a, b): return a + b
来源：http://sy.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gv.bjjhwx.cn

JS:   function add(a, b) { return a + b; }
来源：http://hu.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fs.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ej.521024.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sw.9csxet.cn

Ruby: def add(a, b); a + b; end
来源：http://pl.9csxet.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gs.chemitech.net.cn

[C02] 默认参数
来源：http://nl.bookmarksfly.cn

Py:   def greet(name="World"): return name
来源：http://is.asd995.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gk.panjiajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://lj.huanxung.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xr.lnxyls.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ix.521024.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kz.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://ek.asd995.cn

C#:   string Greet(string name = "World") => name;
来源：http://hx.jianghongdianzi.cn

[C03] 可变参数
来源：http://yx.hahajie.cn

Py:   def total(*args): return sum(args)
来源：http://oa.9csxet.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bj.hnjuh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ij.nicolike.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://es.newstarts.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pa.panjiajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ce.jctech888.com.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jf.lnxyls.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rx.lnxyls.cn

[C04] 命名参数 / 关键字参数
来源：http://lw.hahajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://oo.haigaiapp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hm.hahajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://he.nszjky.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ur.huixiangedu.cn

Java: // 无：用 Builder 模式或 record
来源：http://pc.nszjky.cn

Go:   // 无：用配置结构体参数
来源：http://kt.haigaiapp.cn

Ruby: f(a: 1, b: 2)
来源：http://sp.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://fm.haigaiapp.cn

[C05] 返回多个值
来源：http://ol.nszjky.cn

Py:   return a, b
来源：http://an.gzmigu.cn

PHP:  return [$a, $b];
来源：http://pr.jianghongdianzi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vr.newstarts.cn

TS:   return { a, b };
来源：http://cm.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ht.jianghongdianzi.cn

Go:   return a, b
来源：http://uo.hnjuh.cn

Ruby: return a, b
来源：http://he.nicolike.cn

C#:   return (a, b);              // ValueTuple
来源：http://df.huixiangedu.cn

[C06] 匿名函数 / lambda
来源：http://dt.huanxung.cn

Py:   square = lambda x: x * x
来源：http://qq.jianghongdianzi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qj.yuntaijiaju.cn

JS:   const square = x => x * x;
来源：http://ms.shtwfgs.cn

TS:   const square = (x: number): number => x * x;
来源：http://hq.muxihuayi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hg.nszjky.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gv.muxihuayi.cn

Ruby: square = ->(x) { x * x }
来源：http://fp.haigaiapp.cn


<!-- 参考信息 -->