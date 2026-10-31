代发 wailian999

Java: "第一行\n第二行"
来源：http://gf.haigaiapp.cn

Go:   "第一行\n第二行"
来源：http://sj.huixiangedu.cn

Ruby: "第一行\n第二行"
来源：http://sq.huixinmuqiang.cn

C#:   "第一行\n第二行"
来源：http://tt.haigaiapp.cn

[A14] 注释写法
来源：http://dx.panjiajie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ya.asd995.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://he.hnjuh.cn

JS:   // 单行；/* 多行 */
来源：http://wo.521024.cn

TS:   // 单行；/* 多行 */
来源：http://rp.panjiajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fi.shtwfgs.cn

Go:   // 单行；/* 多行 */
来源：http://lj.hnjuh.cn

Ruby: # 单行；=begin 多行 =end
来源：http://kv.shtwfgs.cn

C#:   // 单行；/* 多行 */
来源：http://pa.shxzskj.cn

[A15] 空值判断与默认值
来源：http://rc.nicolike.cn

Py:   value = data or "默认值"
来源：http://yb.shxzukj.cn

PHP:  $value = $data ?? "默认值";
来源：http://ka.chemitech.net.cn

JS:   const value = data ?? "默认值";
来源：http://zw.asd995.cn

TS:   const value = data ?? "默认值";
来源：http://bc.jctech888.com.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ko.hnjuh.cn

Go:   if data == "" { data = "默认值" }
来源：http://lx.panjiajie.cn

Ruby: value = data || "默认值"
来源：http://bk.shtwfgs.cn

C#:   var value = data ?? "默认值";
来源：http://ca.szsharing.cn

[A16] 真假值判断规则
来源：http://yo.nszjky.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jt.huixinmuqiang.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dc.gzmigu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qu.jianghongdianzi.cn

TS:   if (!x) {}
来源：http://ey.nicolike.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uq.bookmarksfly.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pu.shxzukj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://rs.521024.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mi.shxzskj.cn

[A17] 位运算
来源：http://xv.jctech888.com.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vj.colortex.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qc.nicolike.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tb.asd995.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lx.hnjuh.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://id.shxzskj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://za.huanxung.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ik.yuntaijiaju.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gz.jctech888.com.cn

[A18] 字符与 ASCII 码互转
来源：http://me.huixiangedu.cn

Py:   ord("A"); chr(65)
来源：http://rb.shxzukj.cn

PHP:  ord("A"); chr(65)
来源：http://gp.nicolike.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://il.szxytkj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nd.shxzskj.cn

Java: (int) 'A'; (char) 65
来源：http://bx.huanxung.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://av.huanxung.cn

Ruby: "A".ord; 65.chr
来源：http://go.szsharing.cn

C#:   (int)'A'; (char)65
来源：http://fw.asd995.cn

[A19] 交换两个变量
来源：http://ae.chemitech.net.cn

Py:   a, b = b, a
来源：http://fl.huanxung.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://xv.yuntaijiaju.cn

JS:   [a, b] = [b, a];
来源：http://xy.nicolike.cn

TS:   [a, b] = [b, a];
来源：http://gt.gzmigu.cn

Java: int t = a; a = b; b = t;
来源：http://oe.muxihuayi.cn

Go:   a, b = b, a
来源：http://rr.asd995.cn

Ruby: a, b = b, a
来源：http://hf.hahajie.cn

C#:   (a, b) = (b, a);
来源：http://ln.bjjhwx.cn

[A20] 读取标准输入
来源：http://yh.huixinmuqiang.cn

Py:   name = input("请输入：")
来源：http://lz.jctech888.com.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://co.shtwfgs.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mv.521024.cn

TS:   // Node.js：readline 模块
来源：http://yf.lnxyls.cn

Java: new Scanner(System.in).nextLine()
来源：http://jx.szsharing.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dw.haigaiapp.cn

Ruby: gets.chomp
来源：http://aa.colortex.cn

C#:   Console.ReadLine();
来源：http://tl.hahajie.cn

[A21] 保留指定小数位输出
来源：http://qu.colortex.cn

Py:   f"{3.14159:.2f}"
来源：http://ey.hnjuh.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dp.521024.cn

JS:   (3.14159).toFixed(2)
来源：http://sn.bookmarksfly.cn

TS:   (3.14159).toFixed(2)
来源：http://gb.hahajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://ca.szsharing.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ep.szsharing.cn

Ruby: format("%.2f", 3.14159)
来源：http://ke.shxzukj.cn

C#:   3.14159.ToString("F2")
来源：http://qe.haigaiapp.cn

[A22] 获取字符串长度
来源：http://am.panjiajie.cn

Py:   len(s)
来源：http://jz.nszjky.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://os.chemitech.net.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zz.huixinmuqiang.cn

TS:   s.length
来源：http://pu.huixinmuqiang.cn

Java: s.length()
来源：http://vw.huixiangedu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://if.shxzskj.cn

Ruby: s.length
来源：http://xv.huixiangedu.cn

C#:   s.Length
来源：http://zo.huanxung.cn

[A23] 大小写转换
来源：http://vp.colortex.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xt.yuntaijiaju.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bf.nicolike.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pq.bookmarksfly.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ot.asd995.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ww.szsharing.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mg.shtwfgs.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ez.lnxyls.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xg.bjjhwx.cn

[A24] 去除首尾空白
来源：http://cc.shxzskj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://iw.9csxet.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dh.521024.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ga.szxytkj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rh.newstarts.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xe.jianghongdianzi.cn

Go:   strings.TrimSpace(s)
来源：http://ix.jctech888.com.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xe.jianghongdianzi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://my.szsharing.cn

[A25] 字符串比较
来源：http://og.muxihuayi.cn

Py:   s1 == s2; s1 != s2
来源：http://je.szxytkj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ui.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zc.lnxyls.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rp.gzmigu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://id.hahajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://iw.haigaiapp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rp.shxzukj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tr.asd995.cn

[A26] 类型转换总览
来源：http://aa.szsharing.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xj.521024.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pc.muxihuayi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dl.lnxyls.cn

TS:   Number() String() Boolean() x as number
来源：http://yv.nicolike.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fo.hnjuh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xd.hnjuh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ly.asd995.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gx.shxzskj.cn

================================================================================
来源：http://sm.muxihuayi.cn

B. 流程控制
来源：http://hv.jianghongdianzi.cn

================================================================================
来源：http://mh.asd995.cn

[B01] 条件判断 if / else
来源：http://hr.haigaiapp.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xo.huanxung.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uw.panjiajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yp.shxzskj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tm.newstarts.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qn.jianghongdianzi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ug.9csxet.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://io.szsharing.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uw.colortex.cn

[B02] 多分支 else if / elif
来源：http://vt.jianghongdianzi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vz.521024.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mc.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rg.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pe.muxihuayi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hq.bookmarksfly.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tn.bookmarksfly.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gw.lnxyls.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yl.chemitech.net.cn

[B03] switch / match / case
来源：http://kj.nszjky.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qx.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jk.newstarts.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vh.yuexingan06.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vj.newstarts.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ul.gzmigu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ki.huanxung.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://df.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ky.chemitech.net.cn

[B04] for 计数循环
来源：http://ma.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://qa.yuntaijiaju.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wi.gzmigu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sp.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ps.huixinmuqiang.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pf.jctech888.com.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ep.bjjhwx.cn

Ruby: 10.times { |i| puts i }
来源：http://us.shtwfgs.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kv.colortex.cn

[B05] 遍历数组 / 列表
来源：http://pu.lnxyls.cn

Py:   for item in arr: print(item)
来源：http://ae.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jx.shtwfgs.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wj.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://up.hnjuh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ga.szxytkj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://un.chemitech.net.cn

Ruby: arr.each { |item| puts item }
来源：http://fy.newstarts.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ms.nicolike.cn

[B06] 遍历字典 / 对象
来源：http://pb.jctech888.com.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bv.nicolike.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sn.9csxet.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lj.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xj.szxytkj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vl.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pl.muxihuayi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ll.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://py.szsharing.cn

[B07] while 循环
来源：http://bx.szsharing.cn

Py:   while i < 10: i += 1
来源：http://zl.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://et.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://hn.shxzukj.cn

TS:   while (i < 10) { i++; }
来源：http://xr.wgjwhj.cn

Java: while (i < 10) { i++; }
来源：http://on.9csxet.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ls.asd995.cn

Ruby: while i < 10; i += 1; end
来源：http://gf.shxzskj.cn

C#:   while (i < 10) { i++; }
来源：http://dz.haigaiapp.cn

[B08] do-while（至少执行一次）
来源：http://ak.huixiangedu.cn

Py:   # 无 do-while：用 while True + break
来源：http://sz.shtwfgs.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vv.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://zb.newstarts.cn

TS:   do { i++; } while (i < 10);
来源：http://an.jctech888.com.cn

Java: do { i++; } while (i < 10);
来源：http://st.asd995.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gh.colortex.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cv.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://iu.jianghongdianzi.cn

[B09] break 与 continue
来源：http://bj.haigaiapp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vl.huanxung.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bj.szxytkj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://if.hahajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dm.bookmarksfly.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zn.jianghongdianzi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hm.521024.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hg.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ts.hnjuh.cn

[B10] 遍历同时拿索引
来源：http://pq.hnjuh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://du.shtwfgs.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tp.yuexingan06.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ce.asd995.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fe.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dh.huixinmuqiang.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://so.muxihuayi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tn.asd995.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ka.colortex.cn

[B11] 生成数字序列 / 区间
来源：http://dp.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://yq.huixinmuqiang.cn

PHP:  range(0, 10, 2);
来源：http://of.asd995.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hy.muxihuayi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kk.shxzskj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zu.yuntaijiaju.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://aj.9csxet.cn

Ruby: (0...10).step(2).to_a
来源：http://ar.szxytkj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ec.lnxyls.cn

[B12] 跳出多层循环
来源：http://le.huixiangedu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hx.lnxyls.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ty.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://id.gzmigu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bv.yuexingan06.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://va.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ah.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xv.nszjky.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zu.bookmarksfly.cn

[B13] 判断是否为数字
来源：http://th.lnxyls.cn

Py:   isinstance(x, (int, float))
来源：http://bh.newstarts.cn

PHP:  is_numeric($x)
来源：http://yx.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yp.panjiajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lg.panjiajie.cn

Java: x instanceof Number
来源：http://qi.gzmigu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hl.panjiajie.cn

Ruby: x.is_a?(Numeric)
来源：http://zl.hnjuh.cn

C#:   x is int or double or decimal
来源：http://au.shtwfgs.cn

[B14] 判断值是否在集合内
来源：http://bm.asd995.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sh.jianghongdianzi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ms.shxzukj.cn

JS:   [1, 2, 3].includes(x)
来源：http://jt.bookmarksfly.cn

TS:   [1, 2, 3].includes(x)
来源：http://uz.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rt.haigaiapp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tz.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gc.szsharing.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pf.huixinmuqiang.cn

[B15] 布尔运算与取反
来源：http://uc.jianghongdianzi.cn

Py:   a and b or not c
来源：http://xa.yuntaijiaju.cn

PHP:  $a && $b || !$c
来源：http://wx.shtwfgs.cn

JS:   a && b || !c
来源：http://pa.bjjhwx.cn

TS:   a && b || !c
来源：http://gp.szxytkj.cn

Java: a && b || !c
来源：http://bp.huixiangedu.cn

Go:   a && b || !c
来源：http://fp.huixiangedu.cn

Ruby: a && b || !c
来源：http://zl.haigaiapp.cn

C#:   a && b || !c
来源：http://au.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dp.shxzskj.cn

Py:   if not data: return
来源：http://uu.bjjhwx.cn

PHP:  if (!$data) { return; }
来源：http://hp.huixinmuqiang.cn

JS:   if (!data) return;
来源：http://dw.asd995.cn

TS:   if (!data) return;
来源：http://qa.yuexingan06.cn

Java: if (data == null) return;
来源：http://bx.wgjwhj.cn

Go:   if data == nil { return }
来源：http://wm.newstarts.cn

Ruby: return if data.nil?
来源：http://ox.shxzskj.cn

C#:   if (data == null) return;
来源：http://oj.szxytkj.cn

================================================================================
来源：http://cp.lnxyls.cn

C. 函数与作用域
来源：http://uo.9csxet.cn

================================================================================
来源：http://oa.hnjuh.cn

[C01] 定义函数
来源：http://lt.asd995.cn

Py:   def add(a, b): return a + b
来源：http://xm.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fg.szsharing.cn

JS:   function add(a, b) { return a + b; }
来源：http://kc.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ha.muxihuayi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://uc.chemitech.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ko.jianghongdianzi.cn

Ruby: def add(a, b); a + b; end
来源：http://sk.colortex.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oa.bjjhwx.cn

[C02] 默认参数
来源：http://fw.newstarts.cn

Py:   def greet(name="World"): return name
来源：http://bt.nszjky.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jd.asd995.cn

JS:   function greet(name = "World") { return name; }
来源：http://ak.huixiangedu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ma.bjjhwx.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rh.huixinmuqiang.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sy.muxihuayi.cn

Ruby: def greet(name = "World") = name
来源：http://at.huixiangedu.cn

C#:   string Greet(string name = "World") => name;
来源：http://gx.panjiajie.cn

[C03] 可变参数
来源：http://tf.nicolike.cn

Py:   def total(*args): return sum(args)
来源：http://qn.wgjwhj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ty.nszjky.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://re.huixiangedu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pj.muxihuayi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nk.bjjhwx.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lm.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gg.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://az.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://vu.yuntaijiaju.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wz.newstarts.cn


<!-- 参考信息 -->