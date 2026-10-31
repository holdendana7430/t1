代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fe.panjiajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ry.shtwfgs.cn

TS:   if (!x) {}
来源：http://mc.yuexingan06.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ka.shxzskj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bw.wgjwhj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gz.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://er.shxzukj.cn

[A17] 位运算
来源：http://xy.haigaiapp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bv.panjiajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://to.haigaiapp.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nt.nicolike.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rm.chemitech.net.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dl.bookmarksfly.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bq.bjjhwx.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gw.jctech888.com.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bw.yuexingan06.cn

[A18] 字符与 ASCII 码互转
来源：http://dk.huanxung.cn

Py:   ord("A"); chr(65)
来源：http://ge.szsharing.cn

PHP:  ord("A"); chr(65)
来源：http://lo.nszjky.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tj.9csxet.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ij.newstarts.cn

Java: (int) 'A'; (char) 65
来源：http://ir.huixiangedu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dr.nszjky.cn

Ruby: "A".ord; 65.chr
来源：http://om.yuntaijiaju.cn

C#:   (int)'A'; (char)65
来源：http://xo.chemitech.net.cn

[A19] 交换两个变量
来源：http://dl.bjjhwx.cn

Py:   a, b = b, a
来源：http://jy.haigaiapp.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://hc.muxihuayi.cn

JS:   [a, b] = [b, a];
来源：http://rm.newstarts.cn

TS:   [a, b] = [b, a];
来源：http://mo.521024.cn

Java: int t = a; a = b; b = t;
来源：http://gm.nicolike.cn

Go:   a, b = b, a
来源：http://og.jianghongdianzi.cn

Ruby: a, b = b, a
来源：http://uq.huixinmuqiang.cn

C#:   (a, b) = (b, a);
来源：http://mx.szsharing.cn

[A20] 读取标准输入
来源：http://km.lnxyls.cn

Py:   name = input("请输入：")
来源：http://bk.haigaiapp.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://md.hnjuh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://uz.yuexingan06.cn

TS:   // Node.js：readline 模块
来源：http://wi.shxzukj.cn

Java: new Scanner(System.in).nextLine()
来源：http://qw.wgjwhj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nt.lnxyls.cn

Ruby: gets.chomp
来源：http://qz.lnxyls.cn

C#:   Console.ReadLine();
来源：http://js.wgjwhj.cn

[A21] 保留指定小数位输出
来源：http://xq.shxzskj.cn

Py:   f"{3.14159:.2f}"
来源：http://ze.szxytkj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qp.asd995.cn

JS:   (3.14159).toFixed(2)
来源：http://bj.jctech888.com.cn

TS:   (3.14159).toFixed(2)
来源：http://vk.jctech888.com.cn

Java: String.format("%.2f", 3.14159)
来源：http://hj.yuexingan06.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ez.muxihuayi.cn

Ruby: format("%.2f", 3.14159)
来源：http://wr.szxytkj.cn

C#:   3.14159.ToString("F2")
来源：http://jo.szsharing.cn

[A22] 获取字符串长度
来源：http://oz.panjiajie.cn

Py:   len(s)
来源：http://fj.huixinmuqiang.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dv.jctech888.com.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ol.lnxyls.cn

TS:   s.length
来源：http://zx.nszjky.cn

Java: s.length()
来源：http://ib.9csxet.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pj.521024.cn

Ruby: s.length
来源：http://la.shxzskj.cn

C#:   s.Length
来源：http://xh.hahajie.cn

[A23] 大小写转换
来源：http://ur.muxihuayi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rd.chemitech.net.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://sn.szxytkj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pa.chemitech.net.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ef.panjiajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kc.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bv.huanxung.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bg.wgjwhj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ij.9csxet.cn

[A24] 去除首尾空白
来源：http://vc.shtwfgs.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pn.haigaiapp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bu.shxzukj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kb.huanxung.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fo.newstarts.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ds.bookmarksfly.cn

Go:   strings.TrimSpace(s)
来源：http://vq.jctech888.com.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vd.wgjwhj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xp.huixiangedu.cn

[A25] 字符串比较
来源：http://zz.jctech888.com.cn

Py:   s1 == s2; s1 != s2
来源：http://yn.asd995.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sq.chemitech.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://er.bookmarksfly.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://js.panjiajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ym.hahajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://it.asd995.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wl.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bo.shxzukj.cn

[A26] 类型转换总览
来源：http://kx.panjiajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jx.szxytkj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uj.shtwfgs.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://oy.shxzukj.cn

TS:   Number() String() Boolean() x as number
来源：http://ec.asd995.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nv.asd995.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://su.panjiajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bo.nszjky.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ke.yuexingan06.cn

================================================================================
来源：http://jz.haigaiapp.cn

B. 流程控制
来源：http://bp.shxzukj.cn

================================================================================
来源：http://sc.nszjky.cn

[B01] 条件判断 if / else
来源：http://sc.huixiangedu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zs.hnjuh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ao.hahajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vj.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qa.bookmarksfly.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fx.haigaiapp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dy.nszjky.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nx.shtwfgs.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rz.huanxung.cn

[B02] 多分支 else if / elif
来源：http://jf.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hw.hahajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zu.hnjuh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ma.jianghongdianzi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tz.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://je.shxzskj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lg.shtwfgs.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://il.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lz.jianghongdianzi.cn

[B03] switch / match / case
来源：http://aa.521024.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lh.jctech888.com.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dd.9csxet.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zd.bookmarksfly.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bb.wgjwhj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gj.wgjwhj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xh.szxytkj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vo.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bu.hnjuh.cn

[B04] for 计数循环
来源：http://nh.asd995.cn

Py:   for i in range(10): print(i)
来源：http://td.shxzukj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fd.bjjhwx.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xb.chemitech.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fj.gzmigu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://he.nszjky.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fs.asd995.cn

Ruby: 10.times { |i| puts i }
来源：http://ju.9csxet.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uf.huanxung.cn

[B05] 遍历数组 / 列表
来源：http://zi.9csxet.cn

Py:   for item in arr: print(item)
来源：http://fy.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dm.nszjky.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wb.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://py.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://uu.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cj.haigaiapp.cn

Ruby: arr.each { |item| puts item }
来源：http://aa.jctech888.com.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tr.521024.cn

[B06] 遍历字典 / 对象
来源：http://jw.jctech888.com.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wj.shxzukj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hb.szxytkj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sg.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xf.nszjky.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ca.haigaiapp.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://br.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yp.newstarts.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cq.panjiajie.cn

[B07] while 循环
来源：http://hw.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://bb.yuntaijiaju.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nu.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://hl.shxzukj.cn

TS:   while (i < 10) { i++; }
来源：http://jk.jianghongdianzi.cn

Java: while (i < 10) { i++; }
来源：http://ko.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bw.hahajie.cn

Ruby: while i < 10; i += 1; end
来源：http://cj.szxytkj.cn

C#:   while (i < 10) { i++; }
来源：http://dz.colortex.cn

[B08] do-while（至少执行一次）
来源：http://mr.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://ri.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jo.szxytkj.cn

JS:   do { i++; } while (i < 10);
来源：http://cc.colortex.cn

TS:   do { i++; } while (i < 10);
来源：http://sx.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://eo.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wj.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ni.nicolike.cn

C#:   do { i++; } while (i < 10);
来源：http://io.521024.cn

[B09] break 与 continue
来源：http://oj.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ov.nicolike.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rc.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fn.yuexingan06.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ih.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xw.521024.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ck.asd995.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vf.panjiajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pc.yuntaijiaju.cn

[B10] 遍历同时拿索引
来源：http://iq.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zh.hahajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yw.shtwfgs.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ob.yuntaijiaju.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zz.shxzskj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ff.gzmigu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ja.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ca.yuexingan06.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kv.jctech888.com.cn

[B11] 生成数字序列 / 区间
来源：http://aa.colortex.cn

Py:   list(range(0, 10, 2))
来源：http://ps.chemitech.net.cn

PHP:  range(0, 10, 2);
来源：http://xl.9csxet.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://im.gzmigu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bv.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fx.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vy.asd995.cn

Ruby: (0...10).step(2).to_a
来源：http://zi.9csxet.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qy.hnjuh.cn

[B12] 跳出多层循环
来源：http://jw.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://si.huixinmuqiang.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://we.jianghongdianzi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://px.bookmarksfly.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rx.szxytkj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ym.szsharing.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xl.chemitech.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vz.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://px.muxihuayi.cn

[B13] 判断是否为数字
来源：http://uj.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://lm.nicolike.cn

PHP:  is_numeric($x)
来源：http://fz.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pg.asd995.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pf.hahajie.cn

Java: x instanceof Number
来源：http://dp.szsharing.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vo.newstarts.cn

Ruby: x.is_a?(Numeric)
来源：http://ma.bjjhwx.cn

C#:   x is int or double or decimal
来源：http://me.muxihuayi.cn

[B14] 判断值是否在集合内
来源：http://qj.lnxyls.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sj.shtwfgs.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://om.chemitech.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://iy.hahajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://ck.huixiangedu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yl.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ap.asd995.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cs.asd995.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bp.colortex.cn

[B15] 布尔运算与取反
来源：http://un.shxzskj.cn

Py:   a and b or not c
来源：http://ob.wgjwhj.cn

PHP:  $a && $b || !$c
来源：http://fa.huixiangedu.cn

JS:   a && b || !c
来源：http://ea.hahajie.cn

TS:   a && b || !c
来源：http://cr.lnxyls.cn

Java: a && b || !c
来源：http://jt.huixinmuqiang.cn

Go:   a && b || !c
来源：http://we.chemitech.net.cn

Ruby: a && b || !c
来源：http://cd.yuexingan06.cn

C#:   a && b || !c
来源：http://wm.jctech888.com.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zd.panjiajie.cn

Py:   if not data: return
来源：http://jh.bjjhwx.cn

PHP:  if (!$data) { return; }
来源：http://da.shxzskj.cn

JS:   if (!data) return;
来源：http://cw.colortex.cn

TS:   if (!data) return;
来源：http://ms.panjiajie.cn

Java: if (data == null) return;
来源：http://et.muxihuayi.cn

Go:   if data == nil { return }
来源：http://kq.nszjky.cn

Ruby: return if data.nil?
来源：http://jn.hnjuh.cn

C#:   if (data == null) return;
来源：http://fl.colortex.cn

================================================================================
来源：http://ah.szsharing.cn

C. 函数与作用域
来源：http://tb.shxzukj.cn

================================================================================
来源：http://xg.huanxung.cn

[C01] 定义函数
来源：http://nz.nszjky.cn

Py:   def add(a, b): return a + b
来源：http://xd.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ok.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://ae.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pl.haigaiapp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ub.huixinmuqiang.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ah.jianghongdianzi.cn

Ruby: def add(a, b); a + b; end
来源：http://xp.huanxung.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://iz.huanxung.cn

[C02] 默认参数
来源：http://gl.szsharing.cn

Py:   def greet(name="World"): return name
来源：http://xg.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yt.haigaiapp.cn

JS:   function greet(name = "World") { return name; }
来源：http://pt.asd995.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fu.muxihuayi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zv.newstarts.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vu.bjjhwx.cn

Ruby: def greet(name = "World") = name
来源：http://vb.wgjwhj.cn

C#:   string Greet(string name = "World") => name;
来源：http://jj.huixiangedu.cn

[C03] 可变参数
来源：http://kz.shxzskj.cn

Py:   def total(*args): return sum(args)
来源：http://ts.huixinmuqiang.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tz.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yb.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://oy.asd995.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ix.muxihuayi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://oj.shxzukj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wp.gzmigu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bu.chemitech.net.cn

[C04] 命名参数 / 关键字参数
来源：http://sx.huixiangedu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lb.huanxung.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tb.asd995.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ts.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://li.lnxyls.cn

Java: // 无：用 Builder 模式或 record
来源：http://bz.gzmigu.cn

Go:   // 无：用配置结构体参数
来源：http://kt.asd995.cn

Ruby: f(a: 1, b: 2)
来源：http://vk.hnjuh.cn

C#:   f(a: 1, b: 2)
来源：http://lo.shtwfgs.cn

[C05] 返回多个值
来源：http://fp.huixiangedu.cn

Py:   return a, b
来源：http://ht.yuntaijiaju.cn

PHP:  return [$a, $b];
来源：http://lv.jianghongdianzi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ol.muxihuayi.cn

TS:   return { a, b };
来源：http://bp.asd995.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://di.haigaiapp.cn

Go:   return a, b
来源：http://qd.colortex.cn

Ruby: return a, b
来源：http://np.jctech888.com.cn

C#:   return (a, b);              // ValueTuple
来源：http://ru.huixiangedu.cn

[C06] 匿名函数 / lambda
来源：http://oc.szsharing.cn

Py:   square = lambda x: x * x
来源：http://xr.shxzukj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pd.szsharing.cn

JS:   const square = x => x * x;
来源：http://tz.bookmarksfly.cn

TS:   const square = (x: number): number => x * x;
来源：http://jz.shxzukj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zh.colortex.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ra.panjiajie.cn

Ruby: square = ->(x) { x * x }
来源：http://dq.yuexingan06.cn


<!-- 参考信息 -->