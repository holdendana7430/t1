代发 wailian999

Java: "第一行\n第二行"
来源：http://dz.colortex.cn

Go:   "第一行\n第二行"
来源：http://qr.szsharing.cn

Ruby: "第一行\n第二行"
来源：http://eb.chemitech.net.cn

C#:   "第一行\n第二行"
来源：http://kw.wgjwhj.cn

[A14] 注释写法
来源：http://lw.szsharing.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://lr.lnxyls.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wh.huanxung.cn

JS:   // 单行；/* 多行 */
来源：http://gn.shxzukj.cn

TS:   // 单行；/* 多行 */
来源：http://bs.shxzukj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://em.panjiajie.cn

Go:   // 单行；/* 多行 */
来源：http://cx.shxzukj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xr.lnxyls.cn

C#:   // 单行；/* 多行 */
来源：http://pg.colortex.cn

[A15] 空值判断与默认值
来源：http://fm.nicolike.cn

Py:   value = data or "默认值"
来源：http://xn.nicolike.cn

PHP:  $value = $data ?? "默认值";
来源：http://tu.huixiangedu.cn

JS:   const value = data ?? "默认值";
来源：http://rd.newstarts.cn

TS:   const value = data ?? "默认值";
来源：http://gu.hnjuh.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://sx.haigaiapp.cn

Go:   if data == "" { data = "默认值" }
来源：http://yn.jctech888.com.cn

Ruby: value = data || "默认值"
来源：http://wx.huixiangedu.cn

C#:   var value = data ?? "默认值";
来源：http://zx.huixiangedu.cn

[A16] 真假值判断规则
来源：http://dc.szsharing.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pl.szsharing.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://aw.9csxet.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ra.huixiangedu.cn

TS:   if (!x) {}
来源：http://ax.newstarts.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rx.bookmarksfly.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ze.chemitech.net.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hk.asd995.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://uy.shxzskj.cn

[A17] 位运算
来源：http://pe.jctech888.com.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jz.szsharing.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qh.chemitech.net.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://um.haigaiapp.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fu.wgjwhj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ui.hahajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ca.szxytkj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iq.haigaiapp.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dg.nszjky.cn

[A18] 字符与 ASCII 码互转
来源：http://vu.gzmigu.cn

Py:   ord("A"); chr(65)
来源：http://ux.shxzukj.cn

PHP:  ord("A"); chr(65)
来源：http://sk.hahajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jt.bookmarksfly.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://at.huanxung.cn

Java: (int) 'A'; (char) 65
来源：http://vo.jctech888.com.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ns.521024.cn

Ruby: "A".ord; 65.chr
来源：http://ly.bookmarksfly.cn

C#:   (int)'A'; (char)65
来源：http://bx.asd995.cn

[A19] 交换两个变量
来源：http://yd.huanxung.cn

Py:   a, b = b, a
来源：http://rs.yuntaijiaju.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tf.panjiajie.cn

JS:   [a, b] = [b, a];
来源：http://ha.521024.cn

TS:   [a, b] = [b, a];
来源：http://hl.gzmigu.cn

Java: int t = a; a = b; b = t;
来源：http://kv.panjiajie.cn

Go:   a, b = b, a
来源：http://vr.shtwfgs.cn

Ruby: a, b = b, a
来源：http://ll.muxihuayi.cn

C#:   (a, b) = (b, a);
来源：http://mu.asd995.cn

[A20] 读取标准输入
来源：http://cr.hnjuh.cn

Py:   name = input("请输入：")
来源：http://pq.asd995.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://em.shxzukj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pf.szxytkj.cn

TS:   // Node.js：readline 模块
来源：http://zr.huanxung.cn

Java: new Scanner(System.in).nextLine()
来源：http://sg.nszjky.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gq.chemitech.net.cn

Ruby: gets.chomp
来源：http://pv.huixiangedu.cn

C#:   Console.ReadLine();
来源：http://ou.hahajie.cn

[A21] 保留指定小数位输出
来源：http://cv.huixiangedu.cn

Py:   f"{3.14159:.2f}"
来源：http://hb.colortex.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hi.jianghongdianzi.cn

JS:   (3.14159).toFixed(2)
来源：http://io.lnxyls.cn

TS:   (3.14159).toFixed(2)
来源：http://an.shxzukj.cn

Java: String.format("%.2f", 3.14159)
来源：http://if.yuexingan06.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zg.yuntaijiaju.cn

Ruby: format("%.2f", 3.14159)
来源：http://gy.muxihuayi.cn

C#:   3.14159.ToString("F2")
来源：http://ly.jianghongdianzi.cn

[A22] 获取字符串长度
来源：http://st.hahajie.cn

Py:   len(s)
来源：http://kn.szsharing.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gu.nicolike.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wy.huixiangedu.cn

TS:   s.length
来源：http://ag.huixiangedu.cn

Java: s.length()
来源：http://co.wgjwhj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mv.colortex.cn

Ruby: s.length
来源：http://op.9csxet.cn

C#:   s.Length
来源：http://uv.yuexingan06.cn

[A23] 大小写转换
来源：http://ml.nicolike.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://eo.shtwfgs.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://iw.muxihuayi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fc.huanxung.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yc.colortex.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mx.colortex.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cc.jianghongdianzi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gk.bookmarksfly.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wj.bookmarksfly.cn

[A24] 去除首尾空白
来源：http://rv.newstarts.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://re.shxzskj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qx.nszjky.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iu.521024.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iq.nszjky.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ue.jianghongdianzi.cn

Go:   strings.TrimSpace(s)
来源：http://yz.yuntaijiaju.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ra.huanxung.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ew.szsharing.cn

[A25] 字符串比较
来源：http://hd.521024.cn

Py:   s1 == s2; s1 != s2
来源：http://lg.yuexingan06.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vn.chemitech.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yh.hahajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yt.521024.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fp.lnxyls.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://im.521024.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ap.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ib.muxihuayi.cn

[A26] 类型转换总览
来源：http://jo.colortex.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gx.huanxung.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ic.muxihuayi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://an.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://ms.yuexingan06.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ry.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://uc.yuntaijiaju.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rd.huixinmuqiang.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://do.muxihuayi.cn

================================================================================
来源：http://ju.panjiajie.cn

B. 流程控制
来源：http://kl.muxihuayi.cn

================================================================================
来源：http://wp.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://lr.bjjhwx.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://td.asd995.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xr.shxzukj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qw.huixinmuqiang.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ig.asd995.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tn.nicolike.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hf.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://na.hahajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yl.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://ml.chemitech.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ue.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fx.panjiajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qr.521024.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bp.szsharing.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ew.muxihuayi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qd.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jw.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ay.nszjky.cn

[B03] switch / match / case
来源：http://of.newstarts.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ov.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://si.nicolike.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jn.szxytkj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dh.hahajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nf.521024.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kl.gzmigu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://of.colortex.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zz.huanxung.cn

[B04] for 计数循环
来源：http://go.nicolike.cn

Py:   for i in range(10): print(i)
来源：http://kd.521024.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zt.colortex.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jm.hnjuh.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pf.yuntaijiaju.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nq.asd995.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gz.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://ms.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://of.bjjhwx.cn

[B05] 遍历数组 / 列表
来源：http://bz.yuexingan06.cn

Py:   for item in arr: print(item)
来源：http://zz.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gd.shtwfgs.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ke.shxzskj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pr.521024.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://au.shxzukj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tl.shtwfgs.cn

Ruby: arr.each { |item| puts item }
来源：http://sk.haigaiapp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ui.huanxung.cn

[B06] 遍历字典 / 对象
来源：http://ei.wgjwhj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://oq.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://oh.hahajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nm.wgjwhj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lg.huixinmuqiang.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cr.yuexingan06.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bo.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ss.shxzukj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://og.hnjuh.cn

[B07] while 循环
来源：http://ca.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://yo.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vi.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://oh.panjiajie.cn

TS:   while (i < 10) { i++; }
来源：http://mk.shxzskj.cn

Java: while (i < 10) { i++; }
来源：http://mv.nicolike.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dc.jctech888.com.cn

Ruby: while i < 10; i += 1; end
来源：http://pv.shtwfgs.cn

C#:   while (i < 10) { i++; }
来源：http://lj.hnjuh.cn

[B08] do-while（至少执行一次）
来源：http://mc.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://iv.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pa.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://ga.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://qr.panjiajie.cn

Java: do { i++; } while (i < 10);
来源：http://fj.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://oq.asd995.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ic.521024.cn

C#:   do { i++; } while (i < 10);
来源：http://oz.asd995.cn

[B09] break 与 continue
来源：http://mc.asd995.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uw.szsharing.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ti.asd995.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xb.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wf.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://th.521024.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://at.hahajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ka.huanxung.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yu.colortex.cn

[B10] 遍历同时拿索引
来源：http://iq.huanxung.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jp.jianghongdianzi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lh.asd995.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://oi.yuntaijiaju.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mg.jianghongdianzi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ff.yuntaijiaju.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ne.hahajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ky.asd995.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ox.huixinmuqiang.cn

[B11] 生成数字序列 / 区间
来源：http://sp.hahajie.cn

Py:   list(range(0, 10, 2))
来源：http://zm.szxytkj.cn

PHP:  range(0, 10, 2);
来源：http://ej.szxytkj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cl.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://px.jianghongdianzi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lp.colortex.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zm.huixinmuqiang.cn

Ruby: (0...10).step(2).to_a
来源：http://vl.nicolike.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hf.shxzskj.cn

[B12] 跳出多层循环
来源：http://lg.hahajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cb.521024.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fm.muxihuayi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fh.wgjwhj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ev.shxzskj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://es.bookmarksfly.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cs.szxytkj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://un.nszjky.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vs.huixinmuqiang.cn

[B13] 判断是否为数字
来源：http://oz.huixiangedu.cn

Py:   isinstance(x, (int, float))
来源：http://sk.nicolike.cn

PHP:  is_numeric($x)
来源：http://sd.huixinmuqiang.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ik.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dz.521024.cn

Java: x instanceof Number
来源：http://rz.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bl.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://gx.shxzukj.cn

C#:   x is int or double or decimal
来源：http://fk.hnjuh.cn

[B14] 判断值是否在集合内
来源：http://yf.huanxung.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pi.nszjky.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ec.nicolike.cn

JS:   [1, 2, 3].includes(x)
来源：http://ia.shxzukj.cn

TS:   [1, 2, 3].includes(x)
来源：http://lw.panjiajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hm.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ey.szxytkj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://em.lnxyls.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rm.huanxung.cn

[B15] 布尔运算与取反
来源：http://tq.bookmarksfly.cn

Py:   a and b or not c
来源：http://ae.lnxyls.cn

PHP:  $a && $b || !$c
来源：http://ef.bookmarksfly.cn

JS:   a && b || !c
来源：http://hr.lnxyls.cn

TS:   a && b || !c
来源：http://yb.huanxung.cn

Java: a && b || !c
来源：http://pe.shxzukj.cn

Go:   a && b || !c
来源：http://iz.colortex.cn

Ruby: a && b || !c
来源：http://et.haigaiapp.cn

C#:   a && b || !c
来源：http://xf.jctech888.com.cn

[B16] 卫语句：不满足条件提前返回
来源：http://io.panjiajie.cn

Py:   if not data: return
来源：http://ft.asd995.cn

PHP:  if (!$data) { return; }
来源：http://zl.nicolike.cn

JS:   if (!data) return;
来源：http://nz.newstarts.cn

TS:   if (!data) return;
来源：http://df.nszjky.cn

Java: if (data == null) return;
来源：http://bc.szxytkj.cn

Go:   if data == nil { return }
来源：http://cf.hahajie.cn

Ruby: return if data.nil?
来源：http://sk.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://vd.wgjwhj.cn

================================================================================
来源：http://ti.nszjky.cn

C. 函数与作用域
来源：http://qp.newstarts.cn

================================================================================
来源：http://sd.hahajie.cn

[C01] 定义函数
来源：http://wq.hahajie.cn

Py:   def add(a, b): return a + b
来源：http://ei.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hs.521024.cn

JS:   function add(a, b) { return a + b; }
来源：http://gx.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xy.colortex.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hc.bookmarksfly.cn

Go:   func add(a, b int) int { return a + b }
来源：http://aq.szsharing.cn

Ruby: def add(a, b); a + b; end
来源：http://vu.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fj.muxihuayi.cn

[C02] 默认参数
来源：http://ch.haigaiapp.cn

Py:   def greet(name="World"): return name
来源：http://wc.haigaiapp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xx.bjjhwx.cn

JS:   function greet(name = "World") { return name; }
来源：http://ll.huixinmuqiang.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://kx.colortex.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://aw.asd995.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yc.jctech888.com.cn

Ruby: def greet(name = "World") = name
来源：http://ls.wgjwhj.cn

C#:   string Greet(string name = "World") => name;
来源：http://zv.hnjuh.cn

[C03] 可变参数
来源：http://th.gzmigu.cn

Py:   def total(*args): return sum(args)
来源：http://vs.szxytkj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kp.panjiajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xg.nszjky.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://oj.szxytkj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ta.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zw.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ql.wgjwhj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ns.hahajie.cn

[C04] 命名参数 / 关键字参数
来源：http://oz.wgjwhj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fv.szxytkj.cn


<!-- 参考信息 -->