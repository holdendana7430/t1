代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://go.nszjky.cn

[A15] 空值判断与默认值
来源：http://hp.nszjky.cn

Py:   value = data or "默认值"
来源：http://co.nicolike.cn

PHP:  $value = $data ?? "默认值";
来源：http://rf.gzmigu.cn

JS:   const value = data ?? "默认值";
来源：http://zr.wgjwhj.cn

TS:   const value = data ?? "默认值";
来源：http://ab.colortex.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://uw.panjiajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://xf.bjjhwx.cn

Ruby: value = data || "默认值"
来源：http://eq.jianghongdianzi.cn

C#:   var value = data ?? "默认值";
来源：http://ex.hahajie.cn

[A16] 真假值判断规则
来源：http://vk.lnxyls.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ld.yuexingan06.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://uv.szxytkj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://el.newstarts.cn

TS:   if (!x) {}
来源：http://ib.bookmarksfly.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nq.yuexingan06.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ht.haigaiapp.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ai.shxzukj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ve.shtwfgs.cn

[A17] 位运算
来源：http://zi.yuntaijiaju.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bd.szxytkj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://um.521024.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yo.lnxyls.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qk.hnjuh.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tk.jianghongdianzi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jr.colortex.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cq.yuntaijiaju.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rp.jctech888.com.cn

[A18] 字符与 ASCII 码互转
来源：http://ad.szsharing.cn

Py:   ord("A"); chr(65)
来源：http://qx.lnxyls.cn

PHP:  ord("A"); chr(65)
来源：http://gu.colortex.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sc.jctech888.com.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ms.yuntaijiaju.cn

Java: (int) 'A'; (char) 65
来源：http://ts.szsharing.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ah.lnxyls.cn

Ruby: "A".ord; 65.chr
来源：http://sm.wgjwhj.cn

C#:   (int)'A'; (char)65
来源：http://zz.panjiajie.cn

[A19] 交换两个变量
来源：http://vk.nszjky.cn

Py:   a, b = b, a
来源：http://ry.nicolike.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://uh.gzmigu.cn

JS:   [a, b] = [b, a];
来源：http://le.shtwfgs.cn

TS:   [a, b] = [b, a];
来源：http://mb.asd995.cn

Java: int t = a; a = b; b = t;
来源：http://zn.panjiajie.cn

Go:   a, b = b, a
来源：http://mi.wgjwhj.cn

Ruby: a, b = b, a
来源：http://ix.jctech888.com.cn

C#:   (a, b) = (b, a);
来源：http://oa.shxzukj.cn

[A20] 读取标准输入
来源：http://ck.shtwfgs.cn

Py:   name = input("请输入：")
来源：http://qj.bjjhwx.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://jv.shxzukj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gd.9csxet.cn

TS:   // Node.js：readline 模块
来源：http://vi.panjiajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://oc.yuexingan06.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pm.9csxet.cn

Ruby: gets.chomp
来源：http://si.yuexingan06.cn

C#:   Console.ReadLine();
来源：http://ur.asd995.cn

[A21] 保留指定小数位输出
来源：http://ep.shxzukj.cn

Py:   f"{3.14159:.2f}"
来源：http://cb.yuexingan06.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rr.jianghongdianzi.cn

JS:   (3.14159).toFixed(2)
来源：http://lo.yuntaijiaju.cn

TS:   (3.14159).toFixed(2)
来源：http://qx.shxzskj.cn

Java: String.format("%.2f", 3.14159)
来源：http://qz.bjjhwx.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xp.hnjuh.cn

Ruby: format("%.2f", 3.14159)
来源：http://il.muxihuayi.cn

C#:   3.14159.ToString("F2")
来源：http://aw.shxzskj.cn

[A22] 获取字符串长度
来源：http://uf.gzmigu.cn

Py:   len(s)
来源：http://oz.nicolike.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wh.chemitech.net.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zs.huixinmuqiang.cn

TS:   s.length
来源：http://oh.huixinmuqiang.cn

Java: s.length()
来源：http://gg.wgjwhj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gx.newstarts.cn

Ruby: s.length
来源：http://fm.jctech888.com.cn

C#:   s.Length
来源：http://yr.bookmarksfly.cn

[A23] 大小写转换
来源：http://oh.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://uv.muxihuayi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://is.asd995.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ct.asd995.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fs.hnjuh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://oa.muxihuayi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kf.hahajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wq.bjjhwx.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jw.newstarts.cn

[A24] 去除首尾空白
来源：http://nv.shxzukj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ra.muxihuayi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fm.jianghongdianzi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://it.colortex.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cq.lnxyls.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kh.chemitech.net.cn

Go:   strings.TrimSpace(s)
来源：http://ua.shxzskj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://su.521024.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cm.jianghongdianzi.cn

[A25] 字符串比较
来源：http://vc.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://fr.nszjky.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tf.szxytkj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://om.bookmarksfly.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vu.yuntaijiaju.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://py.muxihuayi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ww.521024.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zz.muxihuayi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ly.hahajie.cn

[A26] 类型转换总览
来源：http://wx.asd995.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sz.panjiajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uk.panjiajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uv.shxzskj.cn

TS:   Number() String() Boolean() x as number
来源：http://ux.gzmigu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wh.521024.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vl.hnjuh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://xk.newstarts.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ly.huanxung.cn

================================================================================
来源：http://ms.jianghongdianzi.cn

B. 流程控制
来源：http://fn.bookmarksfly.cn

================================================================================
来源：http://ul.hahajie.cn

[B01] 条件判断 if / else
来源：http://bd.9csxet.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vx.muxihuayi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ql.shxzskj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rw.hahajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bt.szsharing.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://uh.jianghongdianzi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://is.huixinmuqiang.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yq.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vn.colortex.cn

[B02] 多分支 else if / elif
来源：http://xq.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bs.shxzskj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://iz.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kn.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xt.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://he.asd995.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ny.newstarts.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ta.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cf.hahajie.cn

[B03] switch / match / case
来源：http://fm.521024.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dz.yuntaijiaju.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vb.panjiajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mm.bookmarksfly.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ri.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nu.bookmarksfly.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ga.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pj.szsharing.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jg.yuexingan06.cn

[B04] for 计数循环
来源：http://dz.gzmigu.cn

Py:   for i in range(10): print(i)
来源：http://pd.szsharing.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cf.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vl.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ln.bjjhwx.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oo.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xk.huixinmuqiang.cn

Ruby: 10.times { |i| puts i }
来源：http://yz.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gx.huanxung.cn

[B05] 遍历数组 / 列表
来源：http://dr.huanxung.cn

Py:   for item in arr: print(item)
来源：http://ny.newstarts.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sd.hnjuh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wt.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://eb.shtwfgs.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wx.yuexingan06.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cu.jctech888.com.cn

Ruby: arr.each { |item| puts item }
来源：http://nh.gzmigu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wy.bjjhwx.cn

[B06] 遍历字典 / 对象
来源：http://zn.lnxyls.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://iz.huanxung.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yd.hahajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vw.jianghongdianzi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hr.asd995.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ie.shtwfgs.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eh.521024.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://be.asd995.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xn.hahajie.cn

[B07] while 循环
来源：http://cq.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://ac.9csxet.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ny.hnjuh.cn

JS:   while (i < 10) { i++; }
来源：http://bl.nszjky.cn

TS:   while (i < 10) { i++; }
来源：http://fp.hahajie.cn

Java: while (i < 10) { i++; }
来源：http://ek.521024.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sf.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://bc.wgjwhj.cn

C#:   while (i < 10) { i++; }
来源：http://sn.521024.cn

[B08] do-while（至少执行一次）
来源：http://qo.hnjuh.cn

Py:   # 无 do-while：用 while True + break
来源：http://au.nszjky.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rr.haigaiapp.cn

JS:   do { i++; } while (i < 10);
来源：http://sq.bookmarksfly.cn

TS:   do { i++; } while (i < 10);
来源：http://hv.szsharing.cn

Java: do { i++; } while (i < 10);
来源：http://hd.muxihuayi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fd.yuexingan06.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nf.huanxung.cn

C#:   do { i++; } while (i < 10);
来源：http://nt.szxytkj.cn

[B09] break 与 continue
来源：http://zj.wgjwhj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uv.muxihuayi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://be.szxytkj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vt.wgjwhj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vh.hahajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ft.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cq.jianghongdianzi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vl.panjiajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xg.bookmarksfly.cn

[B10] 遍历同时拿索引
来源：http://yh.shxzskj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gb.shxzukj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://se.nicolike.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qe.newstarts.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bp.newstarts.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ih.asd995.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rf.szsharing.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sl.huanxung.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vf.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://ta.521024.cn

Py:   list(range(0, 10, 2))
来源：http://gq.nicolike.cn

PHP:  range(0, 10, 2);
来源：http://xw.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ea.shxzskj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ct.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zp.nszjky.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zm.yuexingan06.cn

Ruby: (0...10).step(2).to_a
来源：http://kd.jctech888.com.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oj.huixiangedu.cn

[B12] 跳出多层循环
来源：http://nc.jctech888.com.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ov.521024.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nn.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qv.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ng.521024.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ut.bookmarksfly.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ze.huixiangedu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kz.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://am.panjiajie.cn

[B13] 判断是否为数字
来源：http://eo.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://jg.asd995.cn

PHP:  is_numeric($x)
来源：http://ny.yuntaijiaju.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mz.bookmarksfly.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oz.shxzukj.cn

Java: x instanceof Number
来源：http://db.jctech888.com.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hq.szxytkj.cn

Ruby: x.is_a?(Numeric)
来源：http://np.huanxung.cn

C#:   x is int or double or decimal
来源：http://el.9csxet.cn

[B14] 判断值是否在集合内
来源：http://nr.jianghongdianzi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://of.panjiajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ff.shxzskj.cn

JS:   [1, 2, 3].includes(x)
来源：http://mq.jctech888.com.cn

TS:   [1, 2, 3].includes(x)
来源：http://nf.shxzukj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bu.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://om.jianghongdianzi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xy.newstarts.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cw.huixiangedu.cn

[B15] 布尔运算与取反
来源：http://yp.haigaiapp.cn

Py:   a and b or not c
来源：http://cz.colortex.cn

PHP:  $a && $b || !$c
来源：http://bj.nszjky.cn

JS:   a && b || !c
来源：http://ee.wgjwhj.cn

TS:   a && b || !c
来源：http://go.shtwfgs.cn

Java: a && b || !c
来源：http://xb.szsharing.cn

Go:   a && b || !c
来源：http://ts.muxihuayi.cn

Ruby: a && b || !c
来源：http://br.newstarts.cn

C#:   a && b || !c
来源：http://rq.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pi.shtwfgs.cn

Py:   if not data: return
来源：http://pn.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://lh.newstarts.cn

JS:   if (!data) return;
来源：http://wv.panjiajie.cn

TS:   if (!data) return;
来源：http://mu.jctech888.com.cn

Java: if (data == null) return;
来源：http://wd.yuntaijiaju.cn

Go:   if data == nil { return }
来源：http://gt.yuntaijiaju.cn

Ruby: return if data.nil?
来源：http://gx.lnxyls.cn

C#:   if (data == null) return;
来源：http://cb.lnxyls.cn

================================================================================
来源：http://cb.lnxyls.cn

C. 函数与作用域
来源：http://lr.nicolike.cn

================================================================================
来源：http://kv.hnjuh.cn

[C01] 定义函数
来源：http://fz.9csxet.cn

Py:   def add(a, b): return a + b
来源：http://lr.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eu.newstarts.cn

JS:   function add(a, b) { return a + b; }
来源：http://ob.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rz.521024.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rd.bookmarksfly.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zy.jctech888.com.cn

Ruby: def add(a, b); a + b; end
来源：http://so.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ns.muxihuayi.cn

[C02] 默认参数
来源：http://kx.haigaiapp.cn

Py:   def greet(name="World"): return name
来源：http://xx.muxihuayi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qb.shtwfgs.cn

JS:   function greet(name = "World") { return name; }
来源：http://rf.bjjhwx.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://kz.shtwfgs.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cx.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vy.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://pb.shxzskj.cn

C#:   string Greet(string name = "World") => name;
来源：http://yp.chemitech.net.cn

[C03] 可变参数
来源：http://st.hnjuh.cn

Py:   def total(*args): return sum(args)
来源：http://su.521024.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://eg.shtwfgs.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zq.asd995.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uy.jianghongdianzi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mh.9csxet.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fe.bookmarksfly.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nm.wgjwhj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ws.shtwfgs.cn

[C04] 命名参数 / 关键字参数
来源：http://id.haigaiapp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vp.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wo.huixinmuqiang.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wj.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qx.szsharing.cn

Java: // 无：用 Builder 模式或 record
来源：http://ps.521024.cn

Go:   // 无：用配置结构体参数
来源：http://nq.haigaiapp.cn

Ruby: f(a: 1, b: 2)
来源：http://vw.szxytkj.cn

C#:   f(a: 1, b: 2)
来源：http://ah.yuntaijiaju.cn

[C05] 返回多个值
来源：http://qt.colortex.cn

Py:   return a, b
来源：http://yq.jctech888.com.cn

PHP:  return [$a, $b];
来源：http://yg.bookmarksfly.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://iu.bjjhwx.cn

TS:   return { a, b };
来源：http://ig.asd995.cn


<!-- 参考信息 -->