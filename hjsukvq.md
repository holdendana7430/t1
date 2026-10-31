代发 wailian999

[A14] 注释写法
来源：http://jm.huanxung.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://xm.szsharing.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hf.panjiajie.cn

JS:   // 单行；/* 多行 */
来源：http://xu.szsharing.cn

TS:   // 单行；/* 多行 */
来源：http://jf.nszjky.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gu.yuntaijiaju.cn

Go:   // 单行；/* 多行 */
来源：http://hm.huixiangedu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://on.szsharing.cn

C#:   // 单行；/* 多行 */
来源：http://wb.bookmarksfly.cn

[A15] 空值判断与默认值
来源：http://zx.hnjuh.cn

Py:   value = data or "默认值"
来源：http://tb.panjiajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://qr.gzmigu.cn

JS:   const value = data ?? "默认值";
来源：http://sd.shxzukj.cn

TS:   const value = data ?? "默认值";
来源：http://gf.yuntaijiaju.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ta.jctech888.com.cn

Go:   if data == "" { data = "默认值" }
来源：http://ex.huixinmuqiang.cn

Ruby: value = data || "默认值"
来源：http://jx.panjiajie.cn

C#:   var value = data ?? "默认值";
来源：http://dy.yuntaijiaju.cn

[A16] 真假值判断规则
来源：http://ht.newstarts.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ak.chemitech.net.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fv.nszjky.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zi.yuntaijiaju.cn

TS:   if (!x) {}
来源：http://mt.szsharing.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://sg.newstarts.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pl.hnjuh.cn

Ruby: unless x            # nil 与 false 为假
来源：http://km.shxzskj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xo.hnjuh.cn

[A17] 位运算
来源：http://cl.yuntaijiaju.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ee.shxzukj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://az.gzmigu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ku.bookmarksfly.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qd.shxzukj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://je.hnjuh.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dw.jctech888.com.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eh.shtwfgs.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wi.yuexingan06.cn

[A18] 字符与 ASCII 码互转
来源：http://zo.9csxet.cn

Py:   ord("A"); chr(65)
来源：http://ia.wgjwhj.cn

PHP:  ord("A"); chr(65)
来源：http://ph.huixinmuqiang.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qt.nszjky.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fm.gzmigu.cn

Java: (int) 'A'; (char) 65
来源：http://hf.newstarts.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nf.shxzukj.cn

Ruby: "A".ord; 65.chr
来源：http://oo.jctech888.com.cn

C#:   (int)'A'; (char)65
来源：http://hf.wgjwhj.cn

[A19] 交换两个变量
来源：http://aq.yuexingan06.cn

Py:   a, b = b, a
来源：http://fy.nicolike.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://go.szxytkj.cn

JS:   [a, b] = [b, a];
来源：http://go.newstarts.cn

TS:   [a, b] = [b, a];
来源：http://ry.szsharing.cn

Java: int t = a; a = b; b = t;
来源：http://co.shtwfgs.cn

Go:   a, b = b, a
来源：http://ey.lnxyls.cn

Ruby: a, b = b, a
来源：http://bf.nszjky.cn

C#:   (a, b) = (b, a);
来源：http://rq.bookmarksfly.cn

[A20] 读取标准输入
来源：http://or.shxzukj.cn

Py:   name = input("请输入：")
来源：http://gj.yuexingan06.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://dk.shxzukj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lx.hnjuh.cn

TS:   // Node.js：readline 模块
来源：http://ev.nszjky.cn

Java: new Scanner(System.in).nextLine()
来源：http://ty.colortex.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ls.bjjhwx.cn

Ruby: gets.chomp
来源：http://eu.muxihuayi.cn

C#:   Console.ReadLine();
来源：http://xz.huixinmuqiang.cn

[A21] 保留指定小数位输出
来源：http://hc.9csxet.cn

Py:   f"{3.14159:.2f}"
来源：http://tr.huixinmuqiang.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ye.jianghongdianzi.cn

JS:   (3.14159).toFixed(2)
来源：http://me.huanxung.cn

TS:   (3.14159).toFixed(2)
来源：http://vh.521024.cn

Java: String.format("%.2f", 3.14159)
来源：http://rn.hnjuh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kk.gzmigu.cn

Ruby: format("%.2f", 3.14159)
来源：http://vg.szsharing.cn

C#:   3.14159.ToString("F2")
来源：http://sc.chemitech.net.cn

[A22] 获取字符串长度
来源：http://eq.bjjhwx.cn

Py:   len(s)
来源：http://sw.yuntaijiaju.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cz.muxihuayi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zf.shtwfgs.cn

TS:   s.length
来源：http://sp.muxihuayi.cn

Java: s.length()
来源：http://yw.yuntaijiaju.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kz.huanxung.cn

Ruby: s.length
来源：http://rr.colortex.cn

C#:   s.Length
来源：http://fc.bjjhwx.cn

[A23] 大小写转换
来源：http://un.muxihuayi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://db.newstarts.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jc.9csxet.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yk.shxzskj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nx.shxzskj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mo.huixinmuqiang.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dv.nicolike.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cz.nszjky.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xy.panjiajie.cn

[A24] 去除首尾空白
来源：http://fn.wgjwhj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ex.521024.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vr.huixiangedu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://us.yuexingan06.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://na.huanxung.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hl.hahajie.cn

Go:   strings.TrimSpace(s)
来源：http://rx.yuntaijiaju.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://na.shtwfgs.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://uv.shtwfgs.cn

[A25] 字符串比较
来源：http://tq.szxytkj.cn

Py:   s1 == s2; s1 != s2
来源：http://gv.shtwfgs.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://za.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sc.huixiangedu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://va.shxzskj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xn.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ma.jianghongdianzi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rx.haigaiapp.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ty.shxzskj.cn

[A26] 类型转换总览
来源：http://kf.wgjwhj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ej.huixiangedu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vs.asd995.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xr.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://kc.panjiajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hf.hnjuh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ut.hnjuh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ln.lnxyls.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://km.jctech888.com.cn

================================================================================
来源：http://yb.haigaiapp.cn

B. 流程控制
来源：http://zm.huanxung.cn

================================================================================
来源：http://nr.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://fk.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lq.asd995.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ko.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ji.haigaiapp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ko.hahajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jc.panjiajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://az.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tk.shxzskj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rn.shtwfgs.cn

[B02] 多分支 else if / elif
来源：http://gg.shtwfgs.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://eg.shxzukj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xo.szsharing.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ds.shxzskj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sw.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ml.panjiajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qn.muxihuayi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kg.gzmigu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://th.nszjky.cn

[B03] switch / match / case
来源：http://gr.huanxung.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ni.yuntaijiaju.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://db.chemitech.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ql.521024.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://px.huanxung.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yo.shxzukj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ws.jianghongdianzi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ek.hnjuh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ry.gzmigu.cn

[B04] for 计数循环
来源：http://wq.nicolike.cn

Py:   for i in range(10): print(i)
来源：http://hd.colortex.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mo.wgjwhj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jb.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gn.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mj.521024.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bo.hnjuh.cn

Ruby: 10.times { |i| puts i }
来源：http://qu.newstarts.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lu.hahajie.cn

[B05] 遍历数组 / 列表
来源：http://vl.shtwfgs.cn

Py:   for item in arr: print(item)
来源：http://vk.jctech888.com.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wh.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zo.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nr.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ys.haigaiapp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xe.chemitech.net.cn

Ruby: arr.each { |item| puts item }
来源：http://gy.szsharing.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yc.chemitech.net.cn

[B06] 遍历字典 / 对象
来源：http://oy.shtwfgs.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qk.wgjwhj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://de.wgjwhj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ig.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aj.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ur.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xu.9csxet.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hy.muxihuayi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rt.asd995.cn

[B07] while 循环
来源：http://kp.hahajie.cn

Py:   while i < 10: i += 1
来源：http://bg.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ht.muxihuayi.cn

JS:   while (i < 10) { i++; }
来源：http://ye.bookmarksfly.cn

TS:   while (i < 10) { i++; }
来源：http://fy.jctech888.com.cn

Java: while (i < 10) { i++; }
来源：http://an.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uw.haigaiapp.cn

Ruby: while i < 10; i += 1; end
来源：http://pt.colortex.cn

C#:   while (i < 10) { i++; }
来源：http://iv.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://jk.szsharing.cn

Py:   # 无 do-while：用 while True + break
来源：http://hw.szsharing.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gb.yuexingan06.cn

JS:   do { i++; } while (i < 10);
来源：http://mr.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://el.szxytkj.cn

Java: do { i++; } while (i < 10);
来源：http://oo.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vl.colortex.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tj.gzmigu.cn

C#:   do { i++; } while (i < 10);
来源：http://oh.yuntaijiaju.cn

[B09] break 与 continue
来源：http://ti.9csxet.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://er.gzmigu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bb.gzmigu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hx.shxzskj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hm.huanxung.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zn.nicolike.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lt.shtwfgs.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kf.szxytkj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yd.jianghongdianzi.cn

[B10] 遍历同时拿索引
来源：http://vd.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ba.szxytkj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://te.panjiajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://in.shxzskj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://er.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ew.huanxung.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nj.gzmigu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lt.yuexingan06.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gb.hnjuh.cn

[B11] 生成数字序列 / 区间
来源：http://mf.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://um.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://qp.newstarts.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uf.szsharing.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rd.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xs.szsharing.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ha.szxytkj.cn

Ruby: (0...10).step(2).to_a
来源：http://ke.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gq.9csxet.cn

[B12] 跳出多层循环
来源：http://qi.shxzukj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://la.nicolike.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hq.hnjuh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bz.gzmigu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pa.hahajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cu.nicolike.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://he.haigaiapp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gx.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://om.shtwfgs.cn

[B13] 判断是否为数字
来源：http://wg.newstarts.cn

Py:   isinstance(x, (int, float))
来源：http://dh.haigaiapp.cn

PHP:  is_numeric($x)
来源：http://ft.jctech888.com.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xo.colortex.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oc.yuexingan06.cn

Java: x instanceof Number
来源：http://kk.jctech888.com.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gj.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://da.newstarts.cn

C#:   x is int or double or decimal
来源：http://ss.hahajie.cn

[B14] 判断值是否在集合内
来源：http://zf.bjjhwx.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nz.huixiangedu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pq.shtwfgs.cn

JS:   [1, 2, 3].includes(x)
来源：http://sq.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://tq.asd995.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mu.asd995.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vc.jianghongdianzi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jr.nszjky.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tj.chemitech.net.cn

[B15] 布尔运算与取反
来源：http://qd.jianghongdianzi.cn

Py:   a and b or not c
来源：http://rr.szsharing.cn

PHP:  $a && $b || !$c
来源：http://ow.nicolike.cn

JS:   a && b || !c
来源：http://ut.nicolike.cn

TS:   a && b || !c
来源：http://zu.nszjky.cn

Java: a && b || !c
来源：http://yg.yuntaijiaju.cn

Go:   a && b || !c
来源：http://tr.shxzukj.cn

Ruby: a && b || !c
来源：http://nf.lnxyls.cn

C#:   a && b || !c
来源：http://vi.shxzskj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mc.bookmarksfly.cn

Py:   if not data: return
来源：http://yv.chemitech.net.cn

PHP:  if (!$data) { return; }
来源：http://pc.asd995.cn

JS:   if (!data) return;
来源：http://dy.shtwfgs.cn

TS:   if (!data) return;
来源：http://ra.muxihuayi.cn

Java: if (data == null) return;
来源：http://dh.nszjky.cn

Go:   if data == nil { return }
来源：http://oo.chemitech.net.cn

Ruby: return if data.nil?
来源：http://pi.nszjky.cn

C#:   if (data == null) return;
来源：http://ma.huanxung.cn

================================================================================
来源：http://ss.nicolike.cn

C. 函数与作用域
来源：http://pk.haigaiapp.cn

================================================================================
来源：http://qa.gzmigu.cn

[C01] 定义函数
来源：http://dk.huixinmuqiang.cn

Py:   def add(a, b): return a + b
来源：http://ie.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gk.521024.cn

JS:   function add(a, b) { return a + b; }
来源：http://gp.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ea.hnjuh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tl.panjiajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ma.shxzskj.cn

Ruby: def add(a, b); a + b; end
来源：http://hg.haigaiapp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lx.shxzskj.cn

[C02] 默认参数
来源：http://hi.huixiangedu.cn

Py:   def greet(name="World"): return name
来源：http://qi.hnjuh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ve.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://bp.szxytkj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rj.huixinmuqiang.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gr.muxihuayi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://po.yuexingan06.cn

Ruby: def greet(name = "World") = name
来源：http://fz.panjiajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://io.lnxyls.cn

[C03] 可变参数
来源：http://my.szxytkj.cn

Py:   def total(*args): return sum(args)
来源：http://ty.shtwfgs.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pg.bookmarksfly.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ty.jctech888.com.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xp.huanxung.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pj.9csxet.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://an.shxzukj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kf.yuexingan06.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ya.chemitech.net.cn

[C04] 命名参数 / 关键字参数
来源：http://vz.gzmigu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xc.shxzukj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lq.colortex.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eb.521024.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tt.9csxet.cn

Java: // 无：用 Builder 模式或 record
来源：http://dy.yuexingan06.cn


<!-- 参考信息 -->