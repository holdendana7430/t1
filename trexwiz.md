代发 wailian999

Java: "第一行\n第二行"
来源：http://ro.haigaiapp.cn

Go:   "第一行\n第二行"
来源：http://hm.gzmigu.cn

Ruby: "第一行\n第二行"
来源：http://vh.gzmigu.cn

C#:   "第一行\n第二行"
来源：http://hi.shxzskj.cn

[A14] 注释写法
来源：http://rs.bookmarksfly.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://so.chemitech.net.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://mn.asd995.cn

JS:   // 单行；/* 多行 */
来源：http://hj.hahajie.cn

TS:   // 单行；/* 多行 */
来源：http://wb.shxzukj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ss.bookmarksfly.cn

Go:   // 单行；/* 多行 */
来源：http://ab.lnxyls.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hl.hnjuh.cn

C#:   // 单行；/* 多行 */
来源：http://mh.haigaiapp.cn

[A15] 空值判断与默认值
来源：http://tz.huixinmuqiang.cn

Py:   value = data or "默认值"
来源：http://jt.521024.cn

PHP:  $value = $data ?? "默认值";
来源：http://at.szsharing.cn

JS:   const value = data ?? "默认值";
来源：http://bj.9csxet.cn

TS:   const value = data ?? "默认值";
来源：http://wy.521024.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fl.nszjky.cn

Go:   if data == "" { data = "默认值" }
来源：http://eu.huixiangedu.cn

Ruby: value = data || "默认值"
来源：http://fk.hnjuh.cn

C#:   var value = data ?? "默认值";
来源：http://kc.yuntaijiaju.cn

[A16] 真假值判断规则
来源：http://zv.colortex.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ex.9csxet.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nk.szsharing.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vj.nicolike.cn

TS:   if (!x) {}
来源：http://eg.521024.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vs.huanxung.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ae.jctech888.com.cn

Ruby: unless x            # nil 与 false 为假
来源：http://eo.hahajie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ng.shxzukj.cn

[A17] 位运算
来源：http://wm.yuntaijiaju.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ih.yuexingan06.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://to.jctech888.com.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rv.muxihuayi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fw.chemitech.net.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cx.shtwfgs.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dr.bookmarksfly.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dt.szsharing.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wz.newstarts.cn

[A18] 字符与 ASCII 码互转
来源：http://zi.yuntaijiaju.cn

Py:   ord("A"); chr(65)
来源：http://gt.521024.cn

PHP:  ord("A"); chr(65)
来源：http://bm.shxzskj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sm.bjjhwx.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://py.haigaiapp.cn

Java: (int) 'A'; (char) 65
来源：http://uo.panjiajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ko.hahajie.cn

Ruby: "A".ord; 65.chr
来源：http://ur.wgjwhj.cn

C#:   (int)'A'; (char)65
来源：http://rg.wgjwhj.cn

[A19] 交换两个变量
来源：http://mq.asd995.cn

Py:   a, b = b, a
来源：http://mc.colortex.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://bu.newstarts.cn

JS:   [a, b] = [b, a];
来源：http://yg.yuntaijiaju.cn

TS:   [a, b] = [b, a];
来源：http://jn.jctech888.com.cn

Java: int t = a; a = b; b = t;
来源：http://pz.nszjky.cn

Go:   a, b = b, a
来源：http://nn.szsharing.cn

Ruby: a, b = b, a
来源：http://ac.hahajie.cn

C#:   (a, b) = (b, a);
来源：http://hk.shtwfgs.cn

[A20] 读取标准输入
来源：http://xy.jctech888.com.cn

Py:   name = input("请输入：")
来源：http://ry.yuexingan06.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ru.jctech888.com.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hd.lnxyls.cn

TS:   // Node.js：readline 模块
来源：http://sm.hahajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://tf.szsharing.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pu.panjiajie.cn

Ruby: gets.chomp
来源：http://hg.asd995.cn

C#:   Console.ReadLine();
来源：http://ki.huixinmuqiang.cn

[A21] 保留指定小数位输出
来源：http://fg.shxzskj.cn

Py:   f"{3.14159:.2f}"
来源：http://af.szxytkj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wh.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://gz.bjjhwx.cn

TS:   (3.14159).toFixed(2)
来源：http://ny.jianghongdianzi.cn

Java: String.format("%.2f", 3.14159)
来源：http://kw.yuntaijiaju.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nn.521024.cn

Ruby: format("%.2f", 3.14159)
来源：http://ud.gzmigu.cn

C#:   3.14159.ToString("F2")
来源：http://io.yuexingan06.cn

[A22] 获取字符串长度
来源：http://mr.panjiajie.cn

Py:   len(s)
来源：http://fo.lnxyls.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dx.huixinmuqiang.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yy.haigaiapp.cn

TS:   s.length
来源：http://gn.wgjwhj.cn

Java: s.length()
来源：http://tx.muxihuayi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jd.asd995.cn

Ruby: s.length
来源：http://tu.jctech888.com.cn

C#:   s.Length
来源：http://dn.hahajie.cn

[A23] 大小写转换
来源：http://rp.colortex.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://mn.chemitech.net.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yx.asd995.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yw.bookmarksfly.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qw.szxytkj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ha.hahajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vw.bookmarksfly.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://az.nicolike.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ev.chemitech.net.cn

[A24] 去除首尾空白
来源：http://ft.gzmigu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xa.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yt.gzmigu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nl.jianghongdianzi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ei.wgjwhj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gd.bookmarksfly.cn

Go:   strings.TrimSpace(s)
来源：http://mr.asd995.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ub.shtwfgs.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yo.gzmigu.cn

[A25] 字符串比较
来源：http://ke.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://ve.huixiangedu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dh.huanxung.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fa.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cw.muxihuayi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xn.nicolike.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gu.newstarts.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hm.yuntaijiaju.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xz.wgjwhj.cn

[A26] 类型转换总览
来源：http://kt.shxzskj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ji.hnjuh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://su.jianghongdianzi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gy.hahajie.cn

TS:   Number() String() Boolean() x as number
来源：http://gz.newstarts.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hl.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fd.huixiangedu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ql.newstarts.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kz.hnjuh.cn

================================================================================
来源：http://ih.asd995.cn

B. 流程控制
来源：http://tr.panjiajie.cn

================================================================================
来源：http://ct.yuexingan06.cn

[B01] 条件判断 if / else
来源：http://qa.hahajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zn.huanxung.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jf.muxihuayi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kp.huanxung.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nf.huixinmuqiang.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jo.shxzskj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://py.bjjhwx.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sk.huanxung.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fu.bjjhwx.cn

[B02] 多分支 else if / elif
来源：http://nj.hahajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ny.gzmigu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ia.gzmigu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bv.haigaiapp.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bd.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uf.muxihuayi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tp.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nv.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gd.9csxet.cn

[B03] switch / match / case
来源：http://ws.chemitech.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fu.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cq.nszjky.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mk.newstarts.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qr.hahajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rn.hnjuh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ff.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ah.huixiangedu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gr.jctech888.com.cn

[B04] for 计数循环
来源：http://cf.colortex.cn

Py:   for i in range(10): print(i)
来源：http://rv.huanxung.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sh.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kg.szsharing.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pn.hnjuh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://th.haigaiapp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qc.haigaiapp.cn

Ruby: 10.times { |i| puts i }
来源：http://en.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rh.panjiajie.cn

[B05] 遍历数组 / 列表
来源：http://ca.panjiajie.cn

Py:   for item in arr: print(item)
来源：http://vp.haigaiapp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pz.yuntaijiaju.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dr.lnxyls.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fb.szxytkj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jk.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bf.lnxyls.cn

Ruby: arr.each { |item| puts item }
来源：http://ys.huanxung.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://it.shxzskj.cn

[B06] 遍历字典 / 对象
来源：http://xi.panjiajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sj.newstarts.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://on.newstarts.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sm.haigaiapp.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cl.hnjuh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zh.newstarts.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zp.521024.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jv.521024.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kr.haigaiapp.cn

[B07] while 循环
来源：http://yi.521024.cn

Py:   while i < 10: i += 1
来源：http://sl.hahajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fk.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://su.yuntaijiaju.cn

TS:   while (i < 10) { i++; }
来源：http://az.jianghongdianzi.cn

Java: while (i < 10) { i++; }
来源：http://ui.nicolike.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bk.hahajie.cn

Ruby: while i < 10; i += 1; end
来源：http://te.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://ua.hahajie.cn

[B08] do-while（至少执行一次）
来源：http://yh.hnjuh.cn

Py:   # 无 do-while：用 while True + break
来源：http://gb.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vh.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://or.newstarts.cn

TS:   do { i++; } while (i < 10);
来源：http://if.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://go.asd995.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://uc.shxzskj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fa.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://vl.lnxyls.cn

[B09] break 与 continue
来源：http://fa.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fl.9csxet.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yf.szxytkj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vg.yuntaijiaju.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rr.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pq.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://it.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qe.521024.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wn.shtwfgs.cn

[B10] 遍历同时拿索引
来源：http://ui.wgjwhj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vr.huixiangedu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nf.colortex.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xk.hnjuh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uv.colortex.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gg.colortex.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ce.hnjuh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xq.wgjwhj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ie.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://av.jianghongdianzi.cn

Py:   list(range(0, 10, 2))
来源：http://vz.yuexingan06.cn

PHP:  range(0, 10, 2);
来源：http://zu.colortex.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://be.521024.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zw.bookmarksfly.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lt.yuntaijiaju.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ik.gzmigu.cn

Ruby: (0...10).step(2).to_a
来源：http://xq.haigaiapp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zd.haigaiapp.cn

[B12] 跳出多层循环
来源：http://hq.jctech888.com.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qv.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ix.nicolike.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://re.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ct.nszjky.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nr.haigaiapp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://du.jianghongdianzi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rx.521024.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vb.haigaiapp.cn

[B13] 判断是否为数字
来源：http://vt.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://ha.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://on.newstarts.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xi.wgjwhj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tv.nszjky.cn

Java: x instanceof Number
来源：http://gx.huanxung.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zf.hnjuh.cn

Ruby: x.is_a?(Numeric)
来源：http://fy.nicolike.cn

C#:   x is int or double or decimal
来源：http://qb.muxihuayi.cn

[B14] 判断值是否在集合内
来源：http://xo.shxzukj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xa.9csxet.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fw.bjjhwx.cn

JS:   [1, 2, 3].includes(x)
来源：http://kf.huixinmuqiang.cn

TS:   [1, 2, 3].includes(x)
来源：http://fq.9csxet.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lw.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fc.huixiangedu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ws.huanxung.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ko.newstarts.cn

[B15] 布尔运算与取反
来源：http://de.nszjky.cn

Py:   a and b or not c
来源：http://pa.hahajie.cn

PHP:  $a && $b || !$c
来源：http://ci.shxzukj.cn

JS:   a && b || !c
来源：http://zn.jctech888.com.cn

TS:   a && b || !c
来源：http://lp.bjjhwx.cn

Java: a && b || !c
来源：http://kx.shtwfgs.cn

Go:   a && b || !c
来源：http://lt.nicolike.cn

Ruby: a && b || !c
来源：http://zd.wgjwhj.cn

C#:   a && b || !c
来源：http://yo.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vt.shxzskj.cn

Py:   if not data: return
来源：http://ng.nicolike.cn

PHP:  if (!$data) { return; }
来源：http://zx.huixinmuqiang.cn

JS:   if (!data) return;
来源：http://vf.gzmigu.cn

TS:   if (!data) return;
来源：http://tr.nicolike.cn

Java: if (data == null) return;
来源：http://tb.colortex.cn

Go:   if data == nil { return }
来源：http://un.chemitech.net.cn

Ruby: return if data.nil?
来源：http://ad.newstarts.cn

C#:   if (data == null) return;
来源：http://rv.9csxet.cn

================================================================================
来源：http://wl.nicolike.cn

C. 函数与作用域
来源：http://zy.shtwfgs.cn

================================================================================
来源：http://ho.nicolike.cn

[C01] 定义函数
来源：http://bt.huixiangedu.cn

Py:   def add(a, b): return a + b
来源：http://gn.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lq.hahajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://ki.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hy.521024.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hy.shxzukj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rd.yuexingan06.cn

Ruby: def add(a, b); a + b; end
来源：http://wt.521024.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jk.9csxet.cn

[C02] 默认参数
来源：http://ct.chemitech.net.cn

Py:   def greet(name="World"): return name
来源：http://gm.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cc.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://pi.huixiangedu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yg.yuexingan06.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://da.jctech888.com.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ba.bookmarksfly.cn

Ruby: def greet(name = "World") = name
来源：http://ts.bookmarksfly.cn

C#:   string Greet(string name = "World") => name;
来源：http://af.hahajie.cn

[C03] 可变参数
来源：http://ub.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://fs.jianghongdianzi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gi.9csxet.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ok.huixinmuqiang.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yr.shtwfgs.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sz.yuexingan06.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vt.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xv.colortex.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tq.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://co.yuntaijiaju.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xo.muxihuayi.cn


<!-- 参考信息 -->