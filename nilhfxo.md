代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://db.bookmarksfly.cn

Ruby: unless x            # nil 与 false 为假
来源：http://cr.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bi.bjjhwx.cn

[A17] 位运算
来源：http://vr.colortex.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lv.shxzskj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mf.chemitech.net.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://go.bjjhwx.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ey.muxihuayi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qv.wgjwhj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wr.muxihuayi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vh.bjjhwx.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ja.9csxet.cn

[A18] 字符与 ASCII 码互转
来源：http://gh.yuexingan06.cn

Py:   ord("A"); chr(65)
来源：http://xg.bookmarksfly.cn

PHP:  ord("A"); chr(65)
来源：http://lw.lnxyls.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gz.asd995.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pl.bjjhwx.cn

Java: (int) 'A'; (char) 65
来源：http://xh.haigaiapp.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://by.nszjky.cn

Ruby: "A".ord; 65.chr
来源：http://wn.asd995.cn

C#:   (int)'A'; (char)65
来源：http://ms.szsharing.cn

[A19] 交换两个变量
来源：http://ej.9csxet.cn

Py:   a, b = b, a
来源：http://cx.bookmarksfly.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qk.hnjuh.cn

JS:   [a, b] = [b, a];
来源：http://ci.shxzukj.cn

TS:   [a, b] = [b, a];
来源：http://uz.haigaiapp.cn

Java: int t = a; a = b; b = t;
来源：http://cn.hnjuh.cn

Go:   a, b = b, a
来源：http://ev.panjiajie.cn

Ruby: a, b = b, a
来源：http://hs.lnxyls.cn

C#:   (a, b) = (b, a);
来源：http://xl.521024.cn

[A20] 读取标准输入
来源：http://rs.newstarts.cn

Py:   name = input("请输入：")
来源：http://mq.wgjwhj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://hj.bjjhwx.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://to.jctech888.com.cn

TS:   // Node.js：readline 模块
来源：http://xv.szsharing.cn

Java: new Scanner(System.in).nextLine()
来源：http://vh.shtwfgs.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zz.huixinmuqiang.cn

Ruby: gets.chomp
来源：http://xr.huanxung.cn

C#:   Console.ReadLine();
来源：http://am.szsharing.cn

[A21] 保留指定小数位输出
来源：http://zq.9csxet.cn

Py:   f"{3.14159:.2f}"
来源：http://pe.yuexingan06.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pw.asd995.cn

JS:   (3.14159).toFixed(2)
来源：http://yv.huixiangedu.cn

TS:   (3.14159).toFixed(2)
来源：http://jq.chemitech.net.cn

Java: String.format("%.2f", 3.14159)
来源：http://jq.9csxet.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vb.bookmarksfly.cn

Ruby: format("%.2f", 3.14159)
来源：http://nv.lnxyls.cn

C#:   3.14159.ToString("F2")
来源：http://si.jianghongdianzi.cn

[A22] 获取字符串长度
来源：http://oo.szsharing.cn

Py:   len(s)
来源：http://iq.9csxet.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ss.lnxyls.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zs.lnxyls.cn

TS:   s.length
来源：http://tz.lnxyls.cn

Java: s.length()
来源：http://xy.521024.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ds.haigaiapp.cn

Ruby: s.length
来源：http://yz.huixinmuqiang.cn

C#:   s.Length
来源：http://ug.hnjuh.cn

[A23] 大小写转换
来源：http://ar.jianghongdianzi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nj.521024.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ul.wgjwhj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ig.chemitech.net.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lc.jianghongdianzi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ro.nszjky.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ka.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bf.lnxyls.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ow.wgjwhj.cn

[A24] 去除首尾空白
来源：http://uz.jianghongdianzi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jc.nicolike.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://iz.yuexingan06.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wg.521024.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oy.asd995.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://db.jctech888.com.cn

Go:   strings.TrimSpace(s)
来源：http://xw.jctech888.com.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nk.haigaiapp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fj.lnxyls.cn

[A25] 字符串比较
来源：http://rx.bjjhwx.cn

Py:   s1 == s2; s1 != s2
来源：http://by.yuexingan06.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ww.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://si.nicolike.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://eg.panjiajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bf.521024.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uu.haigaiapp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://sr.asd995.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://iy.colortex.cn

[A26] 类型转换总览
来源：http://np.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wu.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wf.521024.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sg.yuntaijiaju.cn

TS:   Number() String() Boolean() x as number
来源：http://yi.asd995.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wi.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://od.shxzukj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fx.yuntaijiaju.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fa.lnxyls.cn

================================================================================
来源：http://pn.nicolike.cn

B. 流程控制
来源：http://hd.huixiangedu.cn

================================================================================
来源：http://cp.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://bx.szxytkj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vq.newstarts.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gl.newstarts.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pf.jctech888.com.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xe.huixiangedu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tz.hnjuh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dw.bjjhwx.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mg.jctech888.com.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yo.panjiajie.cn

[B02] 多分支 else if / elif
来源：http://rj.wgjwhj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pi.jctech888.com.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ft.nszjky.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gx.asd995.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hq.jianghongdianzi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ou.9csxet.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kh.muxihuayi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gd.asd995.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ir.9csxet.cn

[B03] switch / match / case
来源：http://er.wgjwhj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mo.nicolike.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fb.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hm.shxzukj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ml.hnjuh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://en.colortex.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ot.asd995.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qx.9csxet.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kp.nicolike.cn

[B04] for 计数循环
来源：http://sl.lnxyls.cn

Py:   for i in range(10): print(i)
来源：http://fi.gzmigu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nz.szxytkj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ef.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ah.panjiajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kn.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ou.nszjky.cn

Ruby: 10.times { |i| puts i }
来源：http://uz.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://op.nszjky.cn

[B05] 遍历数组 / 列表
来源：http://ei.shtwfgs.cn

Py:   for item in arr: print(item)
来源：http://bt.huixiangedu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ao.hnjuh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ua.yuntaijiaju.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ly.chemitech.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bs.hahajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yg.lnxyls.cn

Ruby: arr.each { |item| puts item }
来源：http://sh.gzmigu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mb.yuexingan06.cn

[B06] 遍历字典 / 对象
来源：http://rr.nszjky.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ey.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vo.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yh.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xg.jctech888.com.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sa.wgjwhj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bb.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://eg.hahajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uh.bookmarksfly.cn

[B07] while 循环
来源：http://mo.huanxung.cn

Py:   while i < 10: i += 1
来源：http://hg.szsharing.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ag.panjiajie.cn

JS:   while (i < 10) { i++; }
来源：http://gy.bookmarksfly.cn

TS:   while (i < 10) { i++; }
来源：http://nn.shxzukj.cn

Java: while (i < 10) { i++; }
来源：http://fg.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xn.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://fn.panjiajie.cn

C#:   while (i < 10) { i++; }
来源：http://ni.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://lj.szxytkj.cn

Py:   # 无 do-while：用 while True + break
来源：http://qi.jianghongdianzi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ng.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://be.521024.cn

TS:   do { i++; } while (i < 10);
来源：http://zh.jctech888.com.cn

Java: do { i++; } while (i < 10);
来源：http://ee.muxihuayi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ur.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://su.huixinmuqiang.cn

C#:   do { i++; } while (i < 10);
来源：http://im.huixiangedu.cn

[B09] break 与 continue
来源：http://ej.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ey.wgjwhj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eo.jctech888.com.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ov.huixiangedu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pr.shxzukj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gl.nszjky.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lx.jctech888.com.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qm.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ig.lnxyls.cn

[B10] 遍历同时拿索引
来源：http://vz.hahajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nz.szsharing.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qx.wgjwhj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://id.asd995.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mj.huanxung.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ve.szxytkj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kd.nszjky.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iq.huanxung.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nw.nicolike.cn

[B11] 生成数字序列 / 区间
来源：http://vu.9csxet.cn

Py:   list(range(0, 10, 2))
来源：http://wg.jctech888.com.cn

PHP:  range(0, 10, 2);
来源：http://df.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xj.muxihuayi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hc.wgjwhj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://of.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kx.521024.cn

Ruby: (0...10).step(2).to_a
来源：http://br.panjiajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lh.panjiajie.cn

[B12] 跳出多层循环
来源：http://pk.jianghongdianzi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://an.chemitech.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kv.jctech888.com.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ek.521024.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nm.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kc.newstarts.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mf.newstarts.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kj.gzmigu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hd.chemitech.net.cn

[B13] 判断是否为数字
来源：http://ws.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://pl.hahajie.cn

PHP:  is_numeric($x)
来源：http://mj.nicolike.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ru.nszjky.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qi.9csxet.cn

Java: x instanceof Number
来源：http://br.nicolike.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xh.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://yf.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://mj.shxzskj.cn

[B14] 判断值是否在集合内
来源：http://pf.yuexingan06.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yx.szxytkj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uk.bookmarksfly.cn

JS:   [1, 2, 3].includes(x)
来源：http://ld.lnxyls.cn

TS:   [1, 2, 3].includes(x)
来源：http://us.jctech888.com.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rz.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zk.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://iy.lnxyls.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wg.lnxyls.cn

[B15] 布尔运算与取反
来源：http://vq.colortex.cn

Py:   a and b or not c
来源：http://np.nszjky.cn

PHP:  $a && $b || !$c
来源：http://kb.lnxyls.cn

JS:   a && b || !c
来源：http://yy.hnjuh.cn

TS:   a && b || !c
来源：http://kx.asd995.cn

Java: a && b || !c
来源：http://ka.yuntaijiaju.cn

Go:   a && b || !c
来源：http://ff.shxzskj.cn

Ruby: a && b || !c
来源：http://lq.lnxyls.cn

C#:   a && b || !c
来源：http://oo.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dw.shtwfgs.cn

Py:   if not data: return
来源：http://ai.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://qu.nszjky.cn

JS:   if (!data) return;
来源：http://na.nszjky.cn

TS:   if (!data) return;
来源：http://vw.jctech888.com.cn

Java: if (data == null) return;
来源：http://rf.bookmarksfly.cn

Go:   if data == nil { return }
来源：http://xz.bookmarksfly.cn

Ruby: return if data.nil?
来源：http://ph.hnjuh.cn

C#:   if (data == null) return;
来源：http://cc.bookmarksfly.cn

================================================================================
来源：http://rn.nszjky.cn

C. 函数与作用域
来源：http://jk.521024.cn

================================================================================
来源：http://px.muxihuayi.cn

[C01] 定义函数
来源：http://bx.wgjwhj.cn

Py:   def add(a, b): return a + b
来源：http://vj.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xc.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://ll.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nk.shxzukj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hv.huixinmuqiang.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qp.521024.cn

Ruby: def add(a, b); a + b; end
来源：http://uq.muxihuayi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://az.nszjky.cn

[C02] 默认参数
来源：http://ch.shxzskj.cn

Py:   def greet(name="World"): return name
来源：http://ar.newstarts.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tp.colortex.cn

JS:   function greet(name = "World") { return name; }
来源：http://pe.szxytkj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://oc.9csxet.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tc.muxihuayi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://az.szsharing.cn

Ruby: def greet(name = "World") = name
来源：http://tj.panjiajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://ft.gzmigu.cn

[C03] 可变参数
来源：http://ds.gzmigu.cn

Py:   def total(*args): return sum(args)
来源：http://ki.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://aq.shtwfgs.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sc.lnxyls.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ik.huanxung.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://in.shxzukj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lk.hnjuh.cn

Ruby: def total(*nums); nums.sum; end
来源：http://is.bookmarksfly.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://aq.szxytkj.cn

[C04] 命名参数 / 关键字参数
来源：http://or.yuexingan06.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ky.huixiangedu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yh.bookmarksfly.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pe.yuexingan06.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mp.wgjwhj.cn

Java: // 无：用 Builder 模式或 record
来源：http://ah.shxzukj.cn

Go:   // 无：用配置结构体参数
来源：http://zr.newstarts.cn

Ruby: f(a: 1, b: 2)
来源：http://vc.asd995.cn

C#:   f(a: 1, b: 2)
来源：http://cm.szxytkj.cn

[C05] 返回多个值
来源：http://mf.chemitech.net.cn

Py:   return a, b
来源：http://mw.szsharing.cn

PHP:  return [$a, $b];
来源：http://kh.hahajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qg.hnjuh.cn

TS:   return { a, b };
来源：http://nu.wgjwhj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ux.huixiangedu.cn

Go:   return a, b
来源：http://qv.jctech888.com.cn

Ruby: return a, b
来源：http://iv.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://xx.jctech888.com.cn

[C06] 匿名函数 / lambda
来源：http://vn.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://sh.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xt.hahajie.cn

JS:   const square = x => x * x;
来源：http://dc.szsharing.cn

TS:   const square = (x: number): number => x * x;
来源：http://ak.nszjky.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cd.hahajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bu.nszjky.cn

Ruby: square = ->(x) { x * x }
来源：http://in.hnjuh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://il.9csxet.cn

[C07] 把函数作为参数传入
来源：http://st.huixiangedu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ke.shxzukj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jy.asd995.cn


<!-- 参考信息 -->