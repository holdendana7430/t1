代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://te.newstarts.cn

[A15] 空值判断与默认值
来源：http://mo.szsharing.cn

Py:   value = data or "默认值"
来源：http://vy.hnjuh.cn

PHP:  $value = $data ?? "默认值";
来源：http://kr.asd995.cn

JS:   const value = data ?? "默认值";
来源：http://yp.muxihuayi.cn

TS:   const value = data ?? "默认值";
来源：http://se.nicolike.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hu.jctech888.com.cn

Go:   if data == "" { data = "默认值" }
来源：http://zw.bjjhwx.cn

Ruby: value = data || "默认值"
来源：http://gn.yuntaijiaju.cn

C#:   var value = data ?? "默认值";
来源：http://zi.huixinmuqiang.cn

[A16] 真假值判断规则
来源：http://lf.wgjwhj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nt.haigaiapp.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qg.haigaiapp.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yn.nicolike.cn

TS:   if (!x) {}
来源：http://oy.haigaiapp.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wu.nicolike.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bd.panjiajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zo.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lq.hnjuh.cn

[A17] 位运算
来源：http://fk.gzmigu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iz.shxzskj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vv.wgjwhj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://js.huanxung.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zt.panjiajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://im.haigaiapp.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nd.bookmarksfly.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aa.yuexingan06.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pa.szsharing.cn

[A18] 字符与 ASCII 码互转
来源：http://qu.lnxyls.cn

Py:   ord("A"); chr(65)
来源：http://er.huixiangedu.cn

PHP:  ord("A"); chr(65)
来源：http://gi.nszjky.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fb.hahajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wm.huixinmuqiang.cn

Java: (int) 'A'; (char) 65
来源：http://ja.muxihuayi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ah.lnxyls.cn

Ruby: "A".ord; 65.chr
来源：http://tg.muxihuayi.cn

C#:   (int)'A'; (char)65
来源：http://vu.bookmarksfly.cn

[A19] 交换两个变量
来源：http://kk.9csxet.cn

Py:   a, b = b, a
来源：http://tu.shtwfgs.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ae.shxzukj.cn

JS:   [a, b] = [b, a];
来源：http://tf.haigaiapp.cn

TS:   [a, b] = [b, a];
来源：http://qm.lnxyls.cn

Java: int t = a; a = b; b = t;
来源：http://af.colortex.cn

Go:   a, b = b, a
来源：http://cw.chemitech.net.cn

Ruby: a, b = b, a
来源：http://uy.gzmigu.cn

C#:   (a, b) = (b, a);
来源：http://vb.shxzskj.cn

[A20] 读取标准输入
来源：http://qu.jctech888.com.cn

Py:   name = input("请输入：")
来源：http://pn.newstarts.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://xz.bookmarksfly.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fc.szsharing.cn

TS:   // Node.js：readline 模块
来源：http://tx.panjiajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://vt.nszjky.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://so.hahajie.cn

Ruby: gets.chomp
来源：http://ip.shxzskj.cn

C#:   Console.ReadLine();
来源：http://vu.shtwfgs.cn

[A21] 保留指定小数位输出
来源：http://wa.lnxyls.cn

Py:   f"{3.14159:.2f}"
来源：http://ur.shxzskj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://sd.szxytkj.cn

JS:   (3.14159).toFixed(2)
来源：http://ux.hahajie.cn

TS:   (3.14159).toFixed(2)
来源：http://kj.haigaiapp.cn

Java: String.format("%.2f", 3.14159)
来源：http://mq.gzmigu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://to.jianghongdianzi.cn

Ruby: format("%.2f", 3.14159)
来源：http://pf.huixinmuqiang.cn

C#:   3.14159.ToString("F2")
来源：http://xi.shxzukj.cn

[A22] 获取字符串长度
来源：http://yg.521024.cn

Py:   len(s)
来源：http://ck.nszjky.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://la.szsharing.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bb.colortex.cn

TS:   s.length
来源：http://qa.panjiajie.cn

Java: s.length()
来源：http://um.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sn.huixiangedu.cn

Ruby: s.length
来源：http://ap.szxytkj.cn

C#:   s.Length
来源：http://mm.panjiajie.cn

[A23] 大小写转换
来源：http://rt.muxihuayi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wm.huixiangedu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mo.jianghongdianzi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gi.nszjky.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ys.gzmigu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://oy.hnjuh.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ny.gzmigu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nc.chemitech.net.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rx.shxzukj.cn

[A24] 去除首尾空白
来源：http://hv.yuntaijiaju.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://eo.521024.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mn.huixiangedu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rx.nszjky.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cy.bjjhwx.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vv.9csxet.cn

Go:   strings.TrimSpace(s)
来源：http://vs.panjiajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ro.jctech888.com.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vf.521024.cn

[A25] 字符串比较
来源：http://id.haigaiapp.cn

Py:   s1 == s2; s1 != s2
来源：http://kt.huanxung.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://py.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dh.wgjwhj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lb.shxzukj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ru.wgjwhj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bw.jianghongdianzi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ay.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fx.chemitech.net.cn

[A26] 类型转换总览
来源：http://db.haigaiapp.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gt.newstarts.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hc.9csxet.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gq.szxytkj.cn

TS:   Number() String() Boolean() x as number
来源：http://pb.asd995.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://br.asd995.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sb.521024.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hd.szsharing.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wv.hnjuh.cn

================================================================================
来源：http://xj.nicolike.cn

B. 流程控制
来源：http://rb.shtwfgs.cn

================================================================================
来源：http://xa.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://bu.huixinmuqiang.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cu.huixinmuqiang.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hj.shtwfgs.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sk.muxihuayi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fy.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bo.wgjwhj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cl.9csxet.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zu.muxihuayi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mx.szxytkj.cn

[B02] 多分支 else if / elif
来源：http://gd.szxytkj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vw.wgjwhj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hw.huixinmuqiang.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fx.chemitech.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://em.nicolike.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yc.shtwfgs.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ml.huixinmuqiang.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qr.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ft.wgjwhj.cn

[B03] switch / match / case
来源：http://lm.panjiajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://aw.asd995.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sn.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vz.shxzukj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://st.colortex.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yx.521024.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ve.newstarts.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zl.jianghongdianzi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dw.szxytkj.cn

[B04] for 计数循环
来源：http://yg.gzmigu.cn

Py:   for i in range(10): print(i)
来源：http://ot.shxzukj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sv.lnxyls.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ox.newstarts.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rh.colortex.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cx.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xc.colortex.cn

Ruby: 10.times { |i| puts i }
来源：http://zp.shxzskj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ws.szxytkj.cn

[B05] 遍历数组 / 列表
来源：http://qn.chemitech.net.cn

Py:   for item in arr: print(item)
来源：http://yx.szxytkj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ak.lnxyls.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hk.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fi.bjjhwx.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pw.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://go.colortex.cn

Ruby: arr.each { |item| puts item }
来源：http://bk.haigaiapp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kh.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://af.shxzskj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gg.huixiangedu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://oh.nszjky.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ya.9csxet.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fk.9csxet.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qk.shtwfgs.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zv.bookmarksfly.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rx.huixiangedu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jx.asd995.cn

[B07] while 循环
来源：http://gf.muxihuayi.cn

Py:   while i < 10: i += 1
来源：http://fd.szsharing.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vg.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://ed.panjiajie.cn

TS:   while (i < 10) { i++; }
来源：http://nl.yuexingan06.cn

Java: while (i < 10) { i++; }
来源：http://so.wgjwhj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vb.shtwfgs.cn

Ruby: while i < 10; i += 1; end
来源：http://qc.lnxyls.cn

C#:   while (i < 10) { i++; }
来源：http://ha.bookmarksfly.cn

[B08] do-while（至少执行一次）
来源：http://zf.chemitech.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://kg.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://iw.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://et.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://ko.521024.cn

Java: do { i++; } while (i < 10);
来源：http://lb.szxytkj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wm.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kb.huixinmuqiang.cn

C#:   do { i++; } while (i < 10);
来源：http://vy.muxihuayi.cn

[B09] break 与 continue
来源：http://vc.521024.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vg.haigaiapp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zf.shtwfgs.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aw.jctech888.com.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mf.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fh.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ng.huixiangedu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hc.huanxung.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cj.9csxet.cn

[B10] 遍历同时拿索引
来源：http://ry.521024.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qq.shxzukj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pi.gzmigu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wd.wgjwhj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dm.nszjky.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bw.gzmigu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cz.521024.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ye.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gn.nszjky.cn

[B11] 生成数字序列 / 区间
来源：http://ze.shxzukj.cn

Py:   list(range(0, 10, 2))
来源：http://wy.bookmarksfly.cn

PHP:  range(0, 10, 2);
来源：http://hc.yuexingan06.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lt.hnjuh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zw.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qu.9csxet.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xd.yuntaijiaju.cn

Ruby: (0...10).step(2).to_a
来源：http://ae.asd995.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xg.shxzskj.cn

[B12] 跳出多层循环
来源：http://ok.jianghongdianzi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ct.colortex.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://oa.yuntaijiaju.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fb.nicolike.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wq.panjiajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hd.szsharing.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jd.muxihuayi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tw.shxzukj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://aq.bjjhwx.cn

[B13] 判断是否为数字
来源：http://wx.huixiangedu.cn

Py:   isinstance(x, (int, float))
来源：http://kn.nszjky.cn

PHP:  is_numeric($x)
来源：http://js.hnjuh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://is.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bb.shxzukj.cn

Java: x instanceof Number
来源：http://qr.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jw.bjjhwx.cn

Ruby: x.is_a?(Numeric)
来源：http://ng.shxzukj.cn

C#:   x is int or double or decimal
来源：http://yj.bookmarksfly.cn

[B14] 判断值是否在集合内
来源：http://la.huixinmuqiang.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nh.haigaiapp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pc.shtwfgs.cn

JS:   [1, 2, 3].includes(x)
来源：http://hm.9csxet.cn

TS:   [1, 2, 3].includes(x)
来源：http://hr.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ok.szsharing.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cw.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nk.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tz.wgjwhj.cn

[B15] 布尔运算与取反
来源：http://pu.szxytkj.cn

Py:   a and b or not c
来源：http://nn.9csxet.cn

PHP:  $a && $b || !$c
来源：http://ul.nszjky.cn

JS:   a && b || !c
来源：http://va.chemitech.net.cn

TS:   a && b || !c
来源：http://eq.bjjhwx.cn

Java: a && b || !c
来源：http://ud.szsharing.cn

Go:   a && b || !c
来源：http://js.bjjhwx.cn

Ruby: a && b || !c
来源：http://in.huixinmuqiang.cn

C#:   a && b || !c
来源：http://yn.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sg.shxzukj.cn

Py:   if not data: return
来源：http://wi.nicolike.cn

PHP:  if (!$data) { return; }
来源：http://we.hnjuh.cn

JS:   if (!data) return;
来源：http://rv.jctech888.com.cn

TS:   if (!data) return;
来源：http://yc.bookmarksfly.cn

Java: if (data == null) return;
来源：http://ed.bjjhwx.cn

Go:   if data == nil { return }
来源：http://nk.szxytkj.cn

Ruby: return if data.nil?
来源：http://uc.bjjhwx.cn

C#:   if (data == null) return;
来源：http://uq.newstarts.cn

================================================================================
来源：http://kz.shtwfgs.cn

C. 函数与作用域
来源：http://dm.jctech888.com.cn

================================================================================
来源：http://dw.muxihuayi.cn

[C01] 定义函数
来源：http://sh.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://cp.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tu.huanxung.cn

JS:   function add(a, b) { return a + b; }
来源：http://qm.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ta.bjjhwx.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wd.szxytkj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qb.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://jm.nszjky.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vy.lnxyls.cn

[C02] 默认参数
来源：http://wg.hnjuh.cn

Py:   def greet(name="World"): return name
来源：http://ob.szxytkj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ka.shtwfgs.cn

JS:   function greet(name = "World") { return name; }
来源：http://ka.hnjuh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ai.shtwfgs.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ls.jctech888.com.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sg.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://ez.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://aw.gzmigu.cn

[C03] 可变参数
来源：http://ud.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://ug.hnjuh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://na.shxzukj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wx.haigaiapp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mo.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gy.bjjhwx.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://es.lnxyls.cn

Ruby: def total(*nums); nums.sum; end
来源：http://in.jianghongdianzi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tm.szxytkj.cn

[C04] 命名参数 / 关键字参数
来源：http://jk.nicolike.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wq.shxzskj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ni.hnjuh.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wj.jianghongdianzi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://es.szxytkj.cn

Java: // 无：用 Builder 模式或 record
来源：http://rj.hnjuh.cn

Go:   // 无：用配置结构体参数
来源：http://ea.huixiangedu.cn

Ruby: f(a: 1, b: 2)
来源：http://pg.panjiajie.cn

C#:   f(a: 1, b: 2)
来源：http://sp.colortex.cn

[C05] 返回多个值
来源：http://hg.wgjwhj.cn

Py:   return a, b
来源：http://az.lnxyls.cn

PHP:  return [$a, $b];
来源：http://ij.bjjhwx.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://of.shtwfgs.cn

TS:   return { a, b };
来源：http://xs.chemitech.net.cn


<!-- 参考信息 -->