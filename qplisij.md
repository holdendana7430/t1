代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://gs.yuntaijiaju.cn

TS:   const value = data ?? "默认值";
来源：http://ra.hnjuh.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pe.nszjky.cn

Go:   if data == "" { data = "默认值" }
来源：http://pt.hnjuh.cn

Ruby: value = data || "默认值"
来源：http://dj.lnxyls.cn

C#:   var value = data ?? "默认值";
来源：http://wy.huixinmuqiang.cn

[A16] 真假值判断规则
来源：http://bg.asd995.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fx.nszjky.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qd.panjiajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rh.jctech888.com.cn

TS:   if (!x) {}
来源：http://uo.shtwfgs.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vp.szxytkj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ph.panjiajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://kt.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zo.gzmigu.cn

[A17] 位运算
来源：http://tu.haigaiapp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jd.newstarts.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gq.chemitech.net.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ph.muxihuayi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://he.jianghongdianzi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yj.hnjuh.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jl.bookmarksfly.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wn.huanxung.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sq.huanxung.cn

[A18] 字符与 ASCII 码互转
来源：http://hr.muxihuayi.cn

Py:   ord("A"); chr(65)
来源：http://fg.nszjky.cn

PHP:  ord("A"); chr(65)
来源：http://oq.chemitech.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://py.yuexingan06.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pj.newstarts.cn

Java: (int) 'A'; (char) 65
来源：http://dm.szsharing.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bt.bjjhwx.cn

Ruby: "A".ord; 65.chr
来源：http://cv.yuntaijiaju.cn

C#:   (int)'A'; (char)65
来源：http://do.huixiangedu.cn

[A19] 交换两个变量
来源：http://li.huanxung.cn

Py:   a, b = b, a
来源：http://dn.bjjhwx.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://im.521024.cn

JS:   [a, b] = [b, a];
来源：http://pr.szsharing.cn

TS:   [a, b] = [b, a];
来源：http://kv.jctech888.com.cn

Java: int t = a; a = b; b = t;
来源：http://sb.haigaiapp.cn

Go:   a, b = b, a
来源：http://tc.bjjhwx.cn

Ruby: a, b = b, a
来源：http://an.nszjky.cn

C#:   (a, b) = (b, a);
来源：http://oi.jianghongdianzi.cn

[A20] 读取标准输入
来源：http://bl.bjjhwx.cn

Py:   name = input("请输入：")
来源：http://yp.9csxet.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gw.gzmigu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dy.gzmigu.cn

TS:   // Node.js：readline 模块
来源：http://ga.hahajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://ki.bjjhwx.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ey.yuntaijiaju.cn

Ruby: gets.chomp
来源：http://uy.521024.cn

C#:   Console.ReadLine();
来源：http://hf.shxzskj.cn

[A21] 保留指定小数位输出
来源：http://eq.panjiajie.cn

Py:   f"{3.14159:.2f}"
来源：http://jg.huixiangedu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fx.lnxyls.cn

JS:   (3.14159).toFixed(2)
来源：http://xh.wgjwhj.cn

TS:   (3.14159).toFixed(2)
来源：http://wx.jianghongdianzi.cn

Java: String.format("%.2f", 3.14159)
来源：http://pu.hnjuh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://as.jctech888.com.cn

Ruby: format("%.2f", 3.14159)
来源：http://rv.nicolike.cn

C#:   3.14159.ToString("F2")
来源：http://st.hahajie.cn

[A22] 获取字符串长度
来源：http://ku.asd995.cn

Py:   len(s)
来源：http://ru.szsharing.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://an.panjiajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://eq.muxihuayi.cn

TS:   s.length
来源：http://ut.lnxyls.cn

Java: s.length()
来源：http://dg.shxzukj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uu.huixinmuqiang.cn

Ruby: s.length
来源：http://ty.colortex.cn

C#:   s.Length
来源：http://ke.jianghongdianzi.cn

[A23] 大小写转换
来源：http://gj.hahajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://su.nszjky.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ug.jctech888.com.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tl.nszjky.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fx.yuntaijiaju.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zi.9csxet.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yh.chemitech.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kd.muxihuayi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ol.szsharing.cn

[A24] 去除首尾空白
来源：http://wi.lnxyls.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sw.gzmigu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nc.hahajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cp.gzmigu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ms.wgjwhj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://eg.shxzskj.cn

Go:   strings.TrimSpace(s)
来源：http://tj.asd995.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qq.newstarts.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yk.lnxyls.cn

[A25] 字符串比较
来源：http://vy.nicolike.cn

Py:   s1 == s2; s1 != s2
来源：http://it.bookmarksfly.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ho.asd995.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mx.hahajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yg.szxytkj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://un.newstarts.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://si.bookmarksfly.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://as.jianghongdianzi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://km.gzmigu.cn

[A26] 类型转换总览
来源：http://lf.szsharing.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bs.9csxet.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pc.panjiajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zi.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://rt.shxzukj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nj.shxzukj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wg.huixiangedu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lj.chemitech.net.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vz.chemitech.net.cn

================================================================================
来源：http://sw.nszjky.cn

B. 流程控制
来源：http://kf.muxihuayi.cn

================================================================================
来源：http://nr.shxzskj.cn

[B01] 条件判断 if / else
来源：http://ht.nszjky.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mw.szsharing.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yd.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lb.asd995.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bl.shxzskj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gj.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vd.bookmarksfly.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://la.hahajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ol.nicolike.cn

[B02] 多分支 else if / elif
来源：http://qo.yuexingan06.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sf.9csxet.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fu.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sv.jianghongdianzi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bg.jianghongdianzi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vc.shtwfgs.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://co.shtwfgs.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ky.szsharing.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://li.chemitech.net.cn

[B03] switch / match / case
来源：http://ov.bjjhwx.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://br.wgjwhj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oq.yuexingan06.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nl.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kw.nszjky.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kj.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gk.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hm.newstarts.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ip.jctech888.com.cn

[B04] for 计数循环
来源：http://jh.nszjky.cn

Py:   for i in range(10): print(i)
来源：http://uk.szsharing.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://os.szsharing.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ab.huixiangedu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://al.521024.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bv.panjiajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://za.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://cc.shxzskj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sh.huixiangedu.cn

[B05] 遍历数组 / 列表
来源：http://vx.nszjky.cn

Py:   for item in arr: print(item)
来源：http://gm.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mv.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://au.yuntaijiaju.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yt.chemitech.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kw.asd995.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kc.chemitech.net.cn

Ruby: arr.each { |item| puts item }
来源：http://sc.chemitech.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://is.huanxung.cn

[B06] 遍历字典 / 对象
来源：http://ts.lnxyls.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zi.newstarts.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zt.szsharing.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ct.shxzskj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wy.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ja.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ac.yuntaijiaju.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yo.szxytkj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yp.muxihuayi.cn

[B07] while 循环
来源：http://nq.shxzukj.cn

Py:   while i < 10: i += 1
来源：http://sk.nicolike.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ag.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://ed.huanxung.cn

TS:   while (i < 10) { i++; }
来源：http://wj.chemitech.net.cn

Java: while (i < 10) { i++; }
来源：http://xh.9csxet.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vs.chemitech.net.cn

Ruby: while i < 10; i += 1; end
来源：http://uk.muxihuayi.cn

C#:   while (i < 10) { i++; }
来源：http://nt.newstarts.cn

[B08] do-while（至少执行一次）
来源：http://oq.shtwfgs.cn

Py:   # 无 do-while：用 while True + break
来源：http://uz.colortex.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cw.jianghongdianzi.cn

JS:   do { i++; } while (i < 10);
来源：http://rl.jctech888.com.cn

TS:   do { i++; } while (i < 10);
来源：http://ws.colortex.cn

Java: do { i++; } while (i < 10);
来源：http://kp.shtwfgs.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yh.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wa.bjjhwx.cn

C#:   do { i++; } while (i < 10);
来源：http://uq.jctech888.com.cn

[B09] break 与 continue
来源：http://hs.colortex.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qy.nicolike.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pw.szxytkj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ar.9csxet.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aw.panjiajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wk.nicolike.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zp.lnxyls.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wk.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jk.szxytkj.cn

[B10] 遍历同时拿索引
来源：http://jn.yuexingan06.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uz.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bk.nszjky.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jw.wgjwhj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ot.colortex.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dc.shxzskj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yo.jctech888.com.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nx.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://df.newstarts.cn

[B11] 生成数字序列 / 区间
来源：http://wk.gzmigu.cn

Py:   list(range(0, 10, 2))
来源：http://pa.colortex.cn

PHP:  range(0, 10, 2);
来源：http://ea.bookmarksfly.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wk.gzmigu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nq.yuntaijiaju.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yh.shxzskj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qz.521024.cn

Ruby: (0...10).step(2).to_a
来源：http://gq.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ww.hnjuh.cn

[B12] 跳出多层循环
来源：http://xr.lnxyls.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ol.jctech888.com.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wa.newstarts.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hx.wgjwhj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bp.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://io.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pz.szsharing.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vc.huanxung.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wi.jctech888.com.cn

[B13] 判断是否为数字
来源：http://rt.huanxung.cn

Py:   isinstance(x, (int, float))
来源：http://uj.9csxet.cn

PHP:  is_numeric($x)
来源：http://ww.huixinmuqiang.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ya.haigaiapp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zr.shtwfgs.cn

Java: x instanceof Number
来源：http://sg.asd995.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cr.nicolike.cn

Ruby: x.is_a?(Numeric)
来源：http://hl.gzmigu.cn

C#:   x is int or double or decimal
来源：http://ab.yuntaijiaju.cn

[B14] 判断值是否在集合内
来源：http://sc.newstarts.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qd.huixiangedu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ia.haigaiapp.cn

JS:   [1, 2, 3].includes(x)
来源：http://fk.huixiangedu.cn

TS:   [1, 2, 3].includes(x)
来源：http://fq.9csxet.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hb.yuexingan06.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ah.muxihuayi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nn.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://no.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://jm.huixinmuqiang.cn

Py:   a and b or not c
来源：http://in.asd995.cn

PHP:  $a && $b || !$c
来源：http://ww.newstarts.cn

JS:   a && b || !c
来源：http://ca.huixinmuqiang.cn

TS:   a && b || !c
来源：http://gd.gzmigu.cn

Java: a && b || !c
来源：http://xe.muxihuayi.cn

Go:   a && b || !c
来源：http://cg.jctech888.com.cn

Ruby: a && b || !c
来源：http://wp.jctech888.com.cn

C#:   a && b || !c
来源：http://az.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gg.chemitech.net.cn

Py:   if not data: return
来源：http://ix.szxytkj.cn

PHP:  if (!$data) { return; }
来源：http://ia.nicolike.cn

JS:   if (!data) return;
来源：http://oe.panjiajie.cn

TS:   if (!data) return;
来源：http://bc.chemitech.net.cn

Java: if (data == null) return;
来源：http://hb.bjjhwx.cn

Go:   if data == nil { return }
来源：http://sh.jctech888.com.cn

Ruby: return if data.nil?
来源：http://tv.nszjky.cn

C#:   if (data == null) return;
来源：http://ih.shxzskj.cn

================================================================================
来源：http://xz.shxzukj.cn

C. 函数与作用域
来源：http://gs.muxihuayi.cn

================================================================================
来源：http://ks.521024.cn

[C01] 定义函数
来源：http://ro.shtwfgs.cn

Py:   def add(a, b): return a + b
来源：http://nb.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hg.nszjky.cn

JS:   function add(a, b) { return a + b; }
来源：http://pk.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wd.chemitech.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hw.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://uc.jianghongdianzi.cn

Ruby: def add(a, b); a + b; end
来源：http://ec.colortex.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kj.huanxung.cn

[C02] 默认参数
来源：http://rj.huixinmuqiang.cn

Py:   def greet(name="World"): return name
来源：http://bj.huanxung.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ci.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://fk.muxihuayi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://km.wgjwhj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fb.shxzukj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://np.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://hj.haigaiapp.cn

C#:   string Greet(string name = "World") => name;
来源：http://kv.bookmarksfly.cn

[C03] 可变参数
来源：http://qs.panjiajie.cn

Py:   def total(*args): return sum(args)
来源：http://zc.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oy.bjjhwx.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qv.jctech888.com.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qv.wgjwhj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qd.muxihuayi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ay.yuexingan06.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bx.nszjky.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ap.muxihuayi.cn

[C04] 命名参数 / 关键字参数
来源：http://og.huanxung.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tq.gzmigu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qn.lnxyls.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ep.9csxet.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ir.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://xu.9csxet.cn

Go:   // 无：用配置结构体参数
来源：http://ky.shxzukj.cn

Ruby: f(a: 1, b: 2)
来源：http://ra.jianghongdianzi.cn

C#:   f(a: 1, b: 2)
来源：http://kj.nszjky.cn

[C05] 返回多个值
来源：http://vc.shtwfgs.cn

Py:   return a, b
来源：http://hu.panjiajie.cn

PHP:  return [$a, $b];
来源：http://jr.asd995.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mx.newstarts.cn

TS:   return { a, b };
来源：http://zg.jctech888.com.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ei.jianghongdianzi.cn

Go:   return a, b
来源：http://rf.colortex.cn

Ruby: return a, b
来源：http://vk.haigaiapp.cn

C#:   return (a, b);              // ValueTuple
来源：http://vx.muxihuayi.cn


<!-- 参考信息 -->