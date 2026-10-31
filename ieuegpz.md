代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://pk.lnxyls.cn

[A15] 空值判断与默认值
来源：http://ze.haigaiapp.cn

Py:   value = data or "默认值"
来源：http://xe.muxihuayi.cn

PHP:  $value = $data ?? "默认值";
来源：http://td.shxzukj.cn

JS:   const value = data ?? "默认值";
来源：http://bb.colortex.cn

TS:   const value = data ?? "默认值";
来源：http://nn.lnxyls.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://aw.9csxet.cn

Go:   if data == "" { data = "默认值" }
来源：http://kp.haigaiapp.cn

Ruby: value = data || "默认值"
来源：http://tr.asd995.cn

C#:   var value = data ?? "默认值";
来源：http://yi.jianghongdianzi.cn

[A16] 真假值判断规则
来源：http://us.wgjwhj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ns.521024.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gj.chemitech.net.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://df.nszjky.cn

TS:   if (!x) {}
来源：http://wv.panjiajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://db.newstarts.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pk.9csxet.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ua.huanxung.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fx.szsharing.cn

[A17] 位运算
来源：http://rn.szsharing.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ub.bjjhwx.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tk.huixiangedu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jm.gzmigu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hr.szxytkj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://go.colortex.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qk.jctech888.com.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ec.szxytkj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ci.gzmigu.cn

[A18] 字符与 ASCII 码互转
来源：http://ls.shtwfgs.cn

Py:   ord("A"); chr(65)
来源：http://uk.yuexingan06.cn

PHP:  ord("A"); chr(65)
来源：http://ff.newstarts.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gl.nszjky.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jz.wgjwhj.cn

Java: (int) 'A'; (char) 65
来源：http://in.szsharing.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vd.jianghongdianzi.cn

Ruby: "A".ord; 65.chr
来源：http://lv.jianghongdianzi.cn

C#:   (int)'A'; (char)65
来源：http://yf.jianghongdianzi.cn

[A19] 交换两个变量
来源：http://sr.jctech888.com.cn

Py:   a, b = b, a
来源：http://su.jctech888.com.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ya.wgjwhj.cn

JS:   [a, b] = [b, a];
来源：http://bp.bjjhwx.cn

TS:   [a, b] = [b, a];
来源：http://gf.szxytkj.cn

Java: int t = a; a = b; b = t;
来源：http://rl.szsharing.cn

Go:   a, b = b, a
来源：http://fc.newstarts.cn

Ruby: a, b = b, a
来源：http://tr.jianghongdianzi.cn

C#:   (a, b) = (b, a);
来源：http://vl.jctech888.com.cn

[A20] 读取标准输入
来源：http://zb.szxytkj.cn

Py:   name = input("请输入：")
来源：http://zv.521024.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ei.yuexingan06.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tl.panjiajie.cn

TS:   // Node.js：readline 模块
来源：http://fa.huanxung.cn

Java: new Scanner(System.in).nextLine()
来源：http://ez.szsharing.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yb.bookmarksfly.cn

Ruby: gets.chomp
来源：http://zt.panjiajie.cn

C#:   Console.ReadLine();
来源：http://pf.yuexingan06.cn

[A21] 保留指定小数位输出
来源：http://om.yuexingan06.cn

Py:   f"{3.14159:.2f}"
来源：http://gh.yuexingan06.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kz.nicolike.cn

JS:   (3.14159).toFixed(2)
来源：http://dg.newstarts.cn

TS:   (3.14159).toFixed(2)
来源：http://lk.jianghongdianzi.cn

Java: String.format("%.2f", 3.14159)
来源：http://dr.huanxung.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gk.szxytkj.cn

Ruby: format("%.2f", 3.14159)
来源：http://ac.jctech888.com.cn

C#:   3.14159.ToString("F2")
来源：http://xq.colortex.cn

[A22] 获取字符串长度
来源：http://ou.chemitech.net.cn

Py:   len(s)
来源：http://nd.nszjky.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xo.wgjwhj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://oz.hahajie.cn

TS:   s.length
来源：http://dj.shtwfgs.cn

Java: s.length()
来源：http://fv.jianghongdianzi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://oc.huanxung.cn

Ruby: s.length
来源：http://hg.jianghongdianzi.cn

C#:   s.Length
来源：http://fx.newstarts.cn

[A23] 大小写转换
来源：http://uj.chemitech.net.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://dy.bjjhwx.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pl.muxihuayi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cs.521024.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cj.asd995.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://us.bjjhwx.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gk.huixinmuqiang.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qc.9csxet.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ej.chemitech.net.cn

[A24] 去除首尾空白
来源：http://iy.szsharing.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jb.panjiajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jf.colortex.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vh.bjjhwx.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hb.muxihuayi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vo.panjiajie.cn

Go:   strings.TrimSpace(s)
来源：http://vo.hahajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dw.szxytkj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ye.bjjhwx.cn

[A25] 字符串比较
来源：http://sw.bookmarksfly.cn

Py:   s1 == s2; s1 != s2
来源：http://ul.9csxet.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vp.haigaiapp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://aa.huanxung.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jn.yuntaijiaju.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ae.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kq.shtwfgs.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yu.yuntaijiaju.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://to.521024.cn

[A26] 类型转换总览
来源：http://kh.gzmigu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vu.nszjky.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zz.521024.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rr.521024.cn

TS:   Number() String() Boolean() x as number
来源：http://eq.huanxung.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gv.hnjuh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ep.chemitech.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vt.521024.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xe.hahajie.cn

================================================================================
来源：http://ov.gzmigu.cn

B. 流程控制
来源：http://xg.lnxyls.cn

================================================================================
来源：http://fj.szxytkj.cn

[B01] 条件判断 if / else
来源：http://ko.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ag.shtwfgs.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://et.wgjwhj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nn.jctech888.com.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fe.muxihuayi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vu.wgjwhj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wm.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ex.yuexingan06.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mb.jianghongdianzi.cn

[B02] 多分支 else if / elif
来源：http://rk.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ul.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fm.szxytkj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qy.wgjwhj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vr.shxzskj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sa.haigaiapp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yl.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xb.bookmarksfly.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pr.szxytkj.cn

[B03] switch / match / case
来源：http://ml.lnxyls.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dz.bjjhwx.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://je.9csxet.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ys.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aj.hahajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xv.shtwfgs.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dg.bookmarksfly.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lg.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hx.huanxung.cn

[B04] for 计数循环
来源：http://nd.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://nn.haigaiapp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ju.szsharing.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oq.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pf.521024.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tx.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ad.521024.cn

Ruby: 10.times { |i| puts i }
来源：http://ea.hnjuh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://eq.shxzskj.cn

[B05] 遍历数组 / 列表
来源：http://ak.yuexingan06.cn

Py:   for item in arr: print(item)
来源：http://rn.bjjhwx.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wf.newstarts.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mw.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://iz.colortex.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zx.jianghongdianzi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://du.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://mo.jianghongdianzi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xr.asd995.cn

[B06] 遍历字典 / 对象
来源：http://pc.jianghongdianzi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fo.shtwfgs.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ya.lnxyls.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yp.shxzskj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fm.lnxyls.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zo.nicolike.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mr.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yg.muxihuayi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jp.bjjhwx.cn

[B07] while 循环
来源：http://qo.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://ou.lnxyls.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ab.colortex.cn

JS:   while (i < 10) { i++; }
来源：http://jg.jctech888.com.cn

TS:   while (i < 10) { i++; }
来源：http://ge.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://jx.shtwfgs.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vx.hahajie.cn

Ruby: while i < 10; i += 1; end
来源：http://wx.panjiajie.cn

C#:   while (i < 10) { i++; }
来源：http://zf.szxytkj.cn

[B08] do-while（至少执行一次）
来源：http://jq.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://ch.asd995.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://oh.shtwfgs.cn

JS:   do { i++; } while (i < 10);
来源：http://sy.huixiangedu.cn

TS:   do { i++; } while (i < 10);
来源：http://cv.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://ou.nszjky.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mn.9csxet.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cq.huanxung.cn

C#:   do { i++; } while (i < 10);
来源：http://qi.asd995.cn

[B09] break 与 continue
来源：http://pg.szxytkj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tv.hnjuh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ir.colortex.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://de.muxihuayi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tf.huanxung.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ui.yuexingan06.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://db.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kz.wgjwhj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://of.huixiangedu.cn

[B10] 遍历同时拿索引
来源：http://lt.nicolike.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://os.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hs.nszjky.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cw.yuexingan06.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qo.hnjuh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://va.szsharing.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rf.521024.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fl.huixinmuqiang.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qe.huixiangedu.cn

[B11] 生成数字序列 / 区间
来源：http://tf.hahajie.cn

Py:   list(range(0, 10, 2))
来源：http://ol.bookmarksfly.cn

PHP:  range(0, 10, 2);
来源：http://fl.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vi.jianghongdianzi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sa.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ac.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yf.shtwfgs.cn

Ruby: (0...10).step(2).to_a
来源：http://zm.hahajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ao.nszjky.cn

[B12] 跳出多层循环
来源：http://on.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ze.shxzskj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ks.huixiangedu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fi.yuexingan06.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bu.nszjky.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://na.jianghongdianzi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bx.jianghongdianzi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ve.hahajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qk.huixinmuqiang.cn

[B13] 判断是否为数字
来源：http://nq.muxihuayi.cn

Py:   isinstance(x, (int, float))
来源：http://la.haigaiapp.cn

PHP:  is_numeric($x)
来源：http://rk.shxzukj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ly.huanxung.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ql.muxihuayi.cn

Java: x instanceof Number
来源：http://rn.gzmigu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://za.lnxyls.cn

Ruby: x.is_a?(Numeric)
来源：http://qn.wgjwhj.cn

C#:   x is int or double or decimal
来源：http://ke.muxihuayi.cn

[B14] 判断值是否在集合内
来源：http://af.bjjhwx.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vz.shxzskj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oe.huixinmuqiang.cn

JS:   [1, 2, 3].includes(x)
来源：http://ay.bjjhwx.cn

TS:   [1, 2, 3].includes(x)
来源：http://rs.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gw.bjjhwx.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://od.huanxung.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qp.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ip.chemitech.net.cn

[B15] 布尔运算与取反
来源：http://jf.szsharing.cn

Py:   a and b or not c
来源：http://qj.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://dn.szxytkj.cn

JS:   a && b || !c
来源：http://qj.newstarts.cn

TS:   a && b || !c
来源：http://bl.huixiangedu.cn

Java: a && b || !c
来源：http://hq.shtwfgs.cn

Go:   a && b || !c
来源：http://sr.huixinmuqiang.cn

Ruby: a && b || !c
来源：http://ap.nszjky.cn

C#:   a && b || !c
来源：http://fd.yuexingan06.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wg.huixinmuqiang.cn

Py:   if not data: return
来源：http://fh.wgjwhj.cn

PHP:  if (!$data) { return; }
来源：http://eq.newstarts.cn

JS:   if (!data) return;
来源：http://wy.jianghongdianzi.cn

TS:   if (!data) return;
来源：http://je.haigaiapp.cn

Java: if (data == null) return;
来源：http://bq.bookmarksfly.cn

Go:   if data == nil { return }
来源：http://fu.hnjuh.cn

Ruby: return if data.nil?
来源：http://qe.yuexingan06.cn

C#:   if (data == null) return;
来源：http://yi.bookmarksfly.cn

================================================================================
来源：http://xc.hahajie.cn

C. 函数与作用域
来源：http://ev.muxihuayi.cn

================================================================================
来源：http://hq.panjiajie.cn

[C01] 定义函数
来源：http://dp.gzmigu.cn

Py:   def add(a, b): return a + b
来源：http://lr.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pv.bookmarksfly.cn

JS:   function add(a, b) { return a + b; }
来源：http://qw.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oz.shtwfgs.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://th.nicolike.cn

Go:   func add(a, b int) int { return a + b }
来源：http://us.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://ea.lnxyls.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wj.shxzukj.cn

[C02] 默认参数
来源：http://gb.nicolike.cn

Py:   def greet(name="World"): return name
来源：http://gm.shtwfgs.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://el.panjiajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://hd.shxzukj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xr.huixiangedu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://np.yuexingan06.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uh.panjiajie.cn

Ruby: def greet(name = "World") = name
来源：http://ec.521024.cn

C#:   string Greet(string name = "World") => name;
来源：http://am.huanxung.cn

[C03] 可变参数
来源：http://wh.szxytkj.cn

Py:   def total(*args): return sum(args)
来源：http://kz.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tw.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rm.hnjuh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zd.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://og.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ap.nicolike.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ku.nicolike.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gb.jctech888.com.cn

[C04] 命名参数 / 关键字参数
来源：http://uh.yuntaijiaju.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gn.haigaiapp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hg.521024.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nm.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://is.jianghongdianzi.cn

Java: // 无：用 Builder 模式或 record
来源：http://cd.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://vg.9csxet.cn

Ruby: f(a: 1, b: 2)
来源：http://ae.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://ss.muxihuayi.cn

[C05] 返回多个值
来源：http://tm.nszjky.cn

Py:   return a, b
来源：http://qk.hahajie.cn

PHP:  return [$a, $b];
来源：http://is.chemitech.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://gk.lnxyls.cn

TS:   return { a, b };
来源：http://dp.yuntaijiaju.cn


<!-- 参考信息 -->