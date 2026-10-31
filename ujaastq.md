代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://ml.gzmigu.cn

TS:   const value = data ?? "默认值";
来源：http://xf.bookmarksfly.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vq.yuntaijiaju.cn

Go:   if data == "" { data = "默认值" }
来源：http://bp.gzmigu.cn

Ruby: value = data || "默认值"
来源：http://xq.hahajie.cn

C#:   var value = data ?? "默认值";
来源：http://jy.wgjwhj.cn

[A16] 真假值判断规则
来源：http://lz.yuexingan06.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pi.gzmigu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://iw.bjjhwx.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ls.haigaiapp.cn

TS:   if (!x) {}
来源：http://sy.yuntaijiaju.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://se.shtwfgs.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vy.nszjky.cn

Ruby: unless x            # nil 与 false 为假
来源：http://oh.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fa.lnxyls.cn

[A17] 位运算
来源：http://kz.wgjwhj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zo.huanxung.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pl.lnxyls.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://md.huixiangedu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zc.colortex.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hu.newstarts.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kz.shxzukj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://js.newstarts.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pd.panjiajie.cn

[A18] 字符与 ASCII 码互转
来源：http://jq.gzmigu.cn

Py:   ord("A"); chr(65)
来源：http://zr.newstarts.cn

PHP:  ord("A"); chr(65)
来源：http://yo.szsharing.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yp.9csxet.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ja.huixiangedu.cn

Java: (int) 'A'; (char) 65
来源：http://nb.panjiajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://df.yuntaijiaju.cn

Ruby: "A".ord; 65.chr
来源：http://ei.haigaiapp.cn

C#:   (int)'A'; (char)65
来源：http://el.wgjwhj.cn

[A19] 交换两个变量
来源：http://lq.yuexingan06.cn

Py:   a, b = b, a
来源：http://ja.muxihuayi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://wz.bjjhwx.cn

JS:   [a, b] = [b, a];
来源：http://xx.newstarts.cn

TS:   [a, b] = [b, a];
来源：http://ca.huanxung.cn

Java: int t = a; a = b; b = t;
来源：http://uf.shxzukj.cn

Go:   a, b = b, a
来源：http://rm.huixiangedu.cn

Ruby: a, b = b, a
来源：http://kx.huixinmuqiang.cn

C#:   (a, b) = (b, a);
来源：http://kz.newstarts.cn

[A20] 读取标准输入
来源：http://ff.colortex.cn

Py:   name = input("请输入：")
来源：http://tp.chemitech.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://lo.gzmigu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://do.shtwfgs.cn

TS:   // Node.js：readline 模块
来源：http://ij.yuntaijiaju.cn

Java: new Scanner(System.in).nextLine()
来源：http://jx.haigaiapp.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://iw.521024.cn

Ruby: gets.chomp
来源：http://yg.panjiajie.cn

C#:   Console.ReadLine();
来源：http://nt.nszjky.cn

[A21] 保留指定小数位输出
来源：http://yq.wgjwhj.cn

Py:   f"{3.14159:.2f}"
来源：http://gn.muxihuayi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jq.panjiajie.cn

JS:   (3.14159).toFixed(2)
来源：http://jj.yuntaijiaju.cn

TS:   (3.14159).toFixed(2)
来源：http://ce.521024.cn

Java: String.format("%.2f", 3.14159)
来源：http://iz.lnxyls.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ag.hnjuh.cn

Ruby: format("%.2f", 3.14159)
来源：http://wj.bjjhwx.cn

C#:   3.14159.ToString("F2")
来源：http://mm.521024.cn

[A22] 获取字符串长度
来源：http://ia.newstarts.cn

Py:   len(s)
来源：http://uo.hnjuh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.521024.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ak.newstarts.cn

TS:   s.length
来源：http://xz.asd995.cn

Java: s.length()
来源：http://lp.shxzukj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ht.shtwfgs.cn

Ruby: s.length
来源：http://hm.shxzukj.cn

C#:   s.Length
来源：http://is.nszjky.cn

[A23] 大小写转换
来源：http://bb.wgjwhj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://iu.newstarts.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cp.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ob.yuexingan06.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cv.haigaiapp.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nr.shxzskj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gp.bjjhwx.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ig.huanxung.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ib.wgjwhj.cn

[A24] 去除首尾空白
来源：http://tv.9csxet.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ss.hahajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://po.szsharing.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fq.szsharing.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yv.shxzskj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://et.nszjky.cn

Go:   strings.TrimSpace(s)
来源：http://rd.huixiangedu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xu.lnxyls.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://aw.muxihuayi.cn

[A25] 字符串比较
来源：http://qx.panjiajie.cn

Py:   s1 == s2; s1 != s2
来源：http://uv.muxihuayi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lp.colortex.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://an.jctech888.com.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bl.bjjhwx.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cx.bookmarksfly.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sm.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ih.521024.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tg.szxytkj.cn

[A26] 类型转换总览
来源：http://ql.chemitech.net.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mr.hnjuh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gq.panjiajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://th.haigaiapp.cn

TS:   Number() String() Boolean() x as number
来源：http://qs.lnxyls.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ul.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pj.asd995.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://to.bjjhwx.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ls.asd995.cn

================================================================================
来源：http://bp.haigaiapp.cn

B. 流程控制
来源：http://uc.newstarts.cn

================================================================================
来源：http://mf.bjjhwx.cn

[B01] 条件判断 if / else
来源：http://bu.gzmigu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hc.chemitech.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uj.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hf.yuntaijiaju.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vs.szsharing.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rz.nszjky.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bv.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://st.chemitech.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tt.shxzskj.cn

[B02] 多分支 else if / elif
来源：http://dj.shtwfgs.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mw.newstarts.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mw.huixiangedu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qn.huixinmuqiang.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ot.panjiajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rc.shxzukj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xu.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vl.bookmarksfly.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qf.jianghongdianzi.cn

[B03] switch / match / case
来源：http://ky.jianghongdianzi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kn.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fe.colortex.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ke.bookmarksfly.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tn.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ho.szxytkj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://og.shxzskj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nh.shtwfgs.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ad.szxytkj.cn

[B04] for 计数循环
来源：http://od.huixinmuqiang.cn

Py:   for i in range(10): print(i)
来源：http://cs.colortex.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hh.haigaiapp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vl.shtwfgs.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wb.asd995.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://da.asd995.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zg.szsharing.cn

Ruby: 10.times { |i| puts i }
来源：http://yr.nszjky.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dt.shtwfgs.cn

[B05] 遍历数组 / 列表
来源：http://lo.huixinmuqiang.cn

Py:   for item in arr: print(item)
来源：http://wr.hnjuh.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kt.521024.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qj.gzmigu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jf.shtwfgs.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yk.huixinmuqiang.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mc.hnjuh.cn

Ruby: arr.each { |item| puts item }
来源：http://dd.muxihuayi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mv.jianghongdianzi.cn

[B06] 遍历字典 / 对象
来源：http://tk.shtwfgs.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://oh.bjjhwx.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vn.huixinmuqiang.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ms.panjiajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ct.bookmarksfly.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dh.huixiangedu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sk.bjjhwx.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://go.shxzukj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gp.jianghongdianzi.cn

[B07] while 循环
来源：http://iy.huanxung.cn

Py:   while i < 10: i += 1
来源：http://gn.shxzukj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mm.nszjky.cn

JS:   while (i < 10) { i++; }
来源：http://qw.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://sl.panjiajie.cn

Java: while (i < 10) { i++; }
来源：http://og.shtwfgs.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hf.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://un.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://sl.yuexingan06.cn

[B08] do-while（至少执行一次）
来源：http://ol.newstarts.cn

Py:   # 无 do-while：用 while True + break
来源：http://sw.bjjhwx.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://be.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://zb.huixinmuqiang.cn

TS:   do { i++; } while (i < 10);
来源：http://zm.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://wv.muxihuayi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mv.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ls.huixinmuqiang.cn

C#:   do { i++; } while (i < 10);
来源：http://aw.gzmigu.cn

[B09] break 与 continue
来源：http://ry.9csxet.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yf.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hv.yuntaijiaju.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vv.gzmigu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pj.lnxyls.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rk.panjiajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lt.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hv.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ds.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://zv.huixiangedu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://io.colortex.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gv.shxzskj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lk.nicolike.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rc.asd995.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://es.huanxung.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mj.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pd.jianghongdianzi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ed.hnjuh.cn

[B11] 生成数字序列 / 区间
来源：http://cf.wgjwhj.cn

Py:   list(range(0, 10, 2))
来源：http://eo.chemitech.net.cn

PHP:  range(0, 10, 2);
来源：http://kq.huixinmuqiang.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uo.haigaiapp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qr.shtwfgs.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hj.szxytkj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://la.newstarts.cn

Ruby: (0...10).step(2).to_a
来源：http://oh.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pq.gzmigu.cn

[B12] 跳出多层循环
来源：http://sn.hnjuh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cz.huixinmuqiang.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kq.bookmarksfly.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zu.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fb.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zw.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jk.521024.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mt.hnjuh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oy.nszjky.cn

[B13] 判断是否为数字
来源：http://ku.muxihuayi.cn

Py:   isinstance(x, (int, float))
来源：http://wk.shxzukj.cn

PHP:  is_numeric($x)
来源：http://em.huixiangedu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yo.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uw.asd995.cn

Java: x instanceof Number
来源：http://iv.szxytkj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ig.yuexingan06.cn

Ruby: x.is_a?(Numeric)
来源：http://mv.hahajie.cn

C#:   x is int or double or decimal
来源：http://me.szsharing.cn

[B14] 判断值是否在集合内
来源：http://ut.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vk.9csxet.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sr.nszjky.cn

JS:   [1, 2, 3].includes(x)
来源：http://hv.colortex.cn

TS:   [1, 2, 3].includes(x)
来源：http://wk.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dn.jianghongdianzi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ss.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ac.bookmarksfly.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fz.lnxyls.cn

[B15] 布尔运算与取反
来源：http://lz.shxzukj.cn

Py:   a and b or not c
来源：http://me.jianghongdianzi.cn

PHP:  $a && $b || !$c
来源：http://xt.yuntaijiaju.cn

JS:   a && b || !c
来源：http://om.9csxet.cn

TS:   a && b || !c
来源：http://ib.nicolike.cn

Java: a && b || !c
来源：http://ia.muxihuayi.cn

Go:   a && b || !c
来源：http://jh.shxzukj.cn

Ruby: a && b || !c
来源：http://mx.shxzskj.cn

C#:   a && b || !c
来源：http://ah.nicolike.cn

[B16] 卫语句：不满足条件提前返回
来源：http://uc.haigaiapp.cn

Py:   if not data: return
来源：http://kb.nszjky.cn

PHP:  if (!$data) { return; }
来源：http://xl.huanxung.cn

JS:   if (!data) return;
来源：http://oh.9csxet.cn

TS:   if (!data) return;
来源：http://rx.szsharing.cn

Java: if (data == null) return;
来源：http://br.jianghongdianzi.cn

Go:   if data == nil { return }
来源：http://du.lnxyls.cn

Ruby: return if data.nil?
来源：http://xj.gzmigu.cn

C#:   if (data == null) return;
来源：http://wi.huixinmuqiang.cn

================================================================================
来源：http://rc.nicolike.cn

C. 函数与作用域
来源：http://od.newstarts.cn

================================================================================
来源：http://in.szsharing.cn

[C01] 定义函数
来源：http://pj.huanxung.cn

Py:   def add(a, b): return a + b
来源：http://do.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://et.colortex.cn

JS:   function add(a, b) { return a + b; }
来源：http://mw.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ce.nicolike.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tw.hnjuh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jz.jctech888.com.cn

Ruby: def add(a, b); a + b; end
来源：http://ut.hahajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://or.gzmigu.cn

[C02] 默认参数
来源：http://ee.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://nc.shtwfgs.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hv.wgjwhj.cn

JS:   function greet(name = "World") { return name; }
来源：http://gh.haigaiapp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://md.9csxet.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rt.yuexingan06.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fl.shxzskj.cn

Ruby: def greet(name = "World") = name
来源：http://cf.huixiangedu.cn

C#:   string Greet(string name = "World") => name;
来源：http://ua.shtwfgs.cn

[C03] 可变参数
来源：http://ag.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://wu.asd995.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dt.colortex.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ck.panjiajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gl.gzmigu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yh.huixiangedu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gv.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kz.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ch.jctech888.com.cn

[C04] 命名参数 / 关键字参数
来源：http://dz.szsharing.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://um.szsharing.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ag.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wv.yuexingan06.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gm.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://rx.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://uo.521024.cn

Ruby: f(a: 1, b: 2)
来源：http://ks.huixiangedu.cn

C#:   f(a: 1, b: 2)
来源：http://gj.huixiangedu.cn

[C05] 返回多个值
来源：http://gw.wgjwhj.cn

Py:   return a, b
来源：http://ad.huixinmuqiang.cn

PHP:  return [$a, $b];
来源：http://jp.shxzukj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vl.hahajie.cn

TS:   return { a, b };
来源：http://ty.colortex.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qb.gzmigu.cn

Go:   return a, b
来源：http://we.lnxyls.cn

Ruby: return a, b
来源：http://ll.newstarts.cn

C#:   return (a, b);              // ValueTuple
来源：http://dd.huixinmuqiang.cn


<!-- 参考信息 -->