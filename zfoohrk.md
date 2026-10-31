代发 wailian999

[A14] 注释写法
来源：http://jh.szxytkj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://jz.shxzskj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wh.szsharing.cn

JS:   // 单行；/* 多行 */
来源：http://sk.9csxet.cn

TS:   // 单行；/* 多行 */
来源：http://ad.jianghongdianzi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ms.nszjky.cn

Go:   // 单行；/* 多行 */
来源：http://nt.haigaiapp.cn

Ruby: # 单行；=begin 多行 =end
来源：http://kt.chemitech.net.cn

C#:   // 单行；/* 多行 */
来源：http://av.muxihuayi.cn

[A15] 空值判断与默认值
来源：http://qt.muxihuayi.cn

Py:   value = data or "默认值"
来源：http://ak.bjjhwx.cn

PHP:  $value = $data ?? "默认值";
来源：http://co.hahajie.cn

JS:   const value = data ?? "默认值";
来源：http://iu.huixinmuqiang.cn

TS:   const value = data ?? "默认值";
来源：http://kn.521024.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cj.bookmarksfly.cn

Go:   if data == "" { data = "默认值" }
来源：http://vx.hnjuh.cn

Ruby: value = data || "默认值"
来源：http://sr.asd995.cn

C#:   var value = data ?? "默认值";
来源：http://bb.asd995.cn

[A16] 真假值判断规则
来源：http://uj.shxzskj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yf.wgjwhj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hc.muxihuayi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ai.yuntaijiaju.cn

TS:   if (!x) {}
来源：http://xb.gzmigu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fe.huixinmuqiang.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://og.newstarts.cn

Ruby: unless x            # nil 与 false 为假
来源：http://nb.shxzukj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yk.gzmigu.cn

[A17] 位运算
来源：http://fu.huixiangedu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kg.shtwfgs.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://oo.bjjhwx.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wf.muxihuayi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://iz.muxihuayi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rz.muxihuayi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mf.shtwfgs.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vo.hnjuh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tb.shtwfgs.cn

[A18] 字符与 ASCII 码互转
来源：http://ip.colortex.cn

Py:   ord("A"); chr(65)
来源：http://fi.hahajie.cn

PHP:  ord("A"); chr(65)
来源：http://vn.9csxet.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nu.huixiangedu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://om.gzmigu.cn

Java: (int) 'A'; (char) 65
来源：http://wo.newstarts.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mk.nszjky.cn

Ruby: "A".ord; 65.chr
来源：http://tc.huixinmuqiang.cn

C#:   (int)'A'; (char)65
来源：http://rv.bjjhwx.cn

[A19] 交换两个变量
来源：http://jw.shxzskj.cn

Py:   a, b = b, a
来源：http://ff.hnjuh.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://mm.yuexingan06.cn

JS:   [a, b] = [b, a];
来源：http://ss.bjjhwx.cn

TS:   [a, b] = [b, a];
来源：http://nl.muxihuayi.cn

Java: int t = a; a = b; b = t;
来源：http://dz.haigaiapp.cn

Go:   a, b = b, a
来源：http://ph.haigaiapp.cn

Ruby: a, b = b, a
来源：http://dh.nicolike.cn

C#:   (a, b) = (b, a);
来源：http://oa.jianghongdianzi.cn

[A20] 读取标准输入
来源：http://zu.bjjhwx.cn

Py:   name = input("请输入：")
来源：http://dl.bjjhwx.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://da.hnjuh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vm.huixinmuqiang.cn

TS:   // Node.js：readline 模块
来源：http://mo.jctech888.com.cn

Java: new Scanner(System.in).nextLine()
来源：http://ld.haigaiapp.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://aj.nicolike.cn

Ruby: gets.chomp
来源：http://cl.bjjhwx.cn

C#:   Console.ReadLine();
来源：http://kf.asd995.cn

[A21] 保留指定小数位输出
来源：http://nu.yuexingan06.cn

Py:   f"{3.14159:.2f}"
来源：http://rx.haigaiapp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bo.nicolike.cn

JS:   (3.14159).toFixed(2)
来源：http://yu.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://jh.shxzskj.cn

Java: String.format("%.2f", 3.14159)
来源：http://ka.huixinmuqiang.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://an.9csxet.cn

Ruby: format("%.2f", 3.14159)
来源：http://mo.521024.cn

C#:   3.14159.ToString("F2")
来源：http://jx.wgjwhj.cn

[A22] 获取字符串长度
来源：http://sk.szxytkj.cn

Py:   len(s)
来源：http://rn.jianghongdianzi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xm.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vo.nszjky.cn

TS:   s.length
来源：http://oe.asd995.cn

Java: s.length()
来源：http://ha.lnxyls.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wh.bjjhwx.cn

Ruby: s.length
来源：http://jq.nszjky.cn

C#:   s.Length
来源：http://iy.521024.cn

[A23] 大小写转换
来源：http://un.jctech888.com.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ez.shxzskj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://am.lnxyls.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://py.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://us.yuexingan06.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ei.hnjuh.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ma.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fy.shxzukj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xg.jctech888.com.cn

[A24] 去除首尾空白
来源：http://jf.nicolike.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tw.hnjuh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gu.hnjuh.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ey.shtwfgs.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cb.nszjky.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nx.huanxung.cn

Go:   strings.TrimSpace(s)
来源：http://en.yuexingan06.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ne.bookmarksfly.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hv.huixiangedu.cn

[A25] 字符串比较
来源：http://hm.lnxyls.cn

Py:   s1 == s2; s1 != s2
来源：http://wo.521024.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hd.muxihuayi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tr.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ib.newstarts.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sb.yuexingan06.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yd.jctech888.com.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://up.chemitech.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vn.colortex.cn

[A26] 类型转换总览
来源：http://ai.jctech888.com.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sz.shxzskj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rm.lnxyls.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hg.chemitech.net.cn

TS:   Number() String() Boolean() x as number
来源：http://ka.huanxung.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://me.lnxyls.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gz.szsharing.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zc.newstarts.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sv.huixinmuqiang.cn

================================================================================
来源：http://oy.chemitech.net.cn

B. 流程控制
来源：http://sh.9csxet.cn

================================================================================
来源：http://ze.panjiajie.cn

[B01] 条件判断 if / else
来源：http://ya.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://tb.521024.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ep.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ab.colortex.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://my.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rt.nszjky.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ol.jianghongdianzi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hh.nszjky.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vw.lnxyls.cn

[B02] 多分支 else if / elif
来源：http://hl.shxzukj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qh.nicolike.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ob.hahajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mp.hnjuh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rm.szxytkj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zy.lnxyls.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rf.gzmigu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ww.szxytkj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jq.lnxyls.cn

[B03] switch / match / case
来源：http://pv.jianghongdianzi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xt.newstarts.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vb.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dh.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://om.panjiajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xn.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uo.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fh.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mw.szsharing.cn

[B04] for 计数循环
来源：http://pr.bjjhwx.cn

Py:   for i in range(10): print(i)
来源：http://hs.asd995.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pf.bookmarksfly.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uc.huixiangedu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zu.shxzskj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ga.yuexingan06.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ap.newstarts.cn

Ruby: 10.times { |i| puts i }
来源：http://xw.nicolike.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pz.lnxyls.cn

[B05] 遍历数组 / 列表
来源：http://ls.hnjuh.cn

Py:   for item in arr: print(item)
来源：http://ha.yuexingan06.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nl.szxytkj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://um.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rv.521024.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zi.nszjky.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rf.jctech888.com.cn

Ruby: arr.each { |item| puts item }
来源：http://tm.hahajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yr.shtwfgs.cn

[B06] 遍历字典 / 对象
来源：http://uw.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tl.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gw.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yo.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qu.szxytkj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rc.asd995.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lx.panjiajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dj.yuntaijiaju.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cn.panjiajie.cn

[B07] while 循环
来源：http://qx.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://fe.9csxet.cn

PHP:  while ($i < 10) { $i++; }
来源：http://im.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://hf.gzmigu.cn

TS:   while (i < 10) { i++; }
来源：http://cx.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://ig.colortex.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ul.9csxet.cn

Ruby: while i < 10; i += 1; end
来源：http://cg.colortex.cn

C#:   while (i < 10) { i++; }
来源：http://rc.lnxyls.cn

[B08] do-while（至少执行一次）
来源：http://ij.muxihuayi.cn

Py:   # 无 do-while：用 while True + break
来源：http://wm.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pu.bookmarksfly.cn

JS:   do { i++; } while (i < 10);
来源：http://cf.shtwfgs.cn

TS:   do { i++; } while (i < 10);
来源：http://ns.chemitech.net.cn

Java: do { i++; } while (i < 10);
来源：http://zf.szsharing.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jb.shxzskj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xr.haigaiapp.cn

C#:   do { i++; } while (i < 10);
来源：http://po.huixiangedu.cn

[B09] break 与 continue
来源：http://wp.colortex.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lb.bjjhwx.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.colortex.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lz.521024.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kc.jctech888.com.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fh.chemitech.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cz.9csxet.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qa.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sq.hahajie.cn

[B10] 遍历同时拿索引
来源：http://ey.newstarts.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ln.haigaiapp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sc.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zr.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kf.yuntaijiaju.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ip.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hx.gzmigu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mr.yuntaijiaju.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qu.newstarts.cn

[B11] 生成数字序列 / 区间
来源：http://on.colortex.cn

Py:   list(range(0, 10, 2))
来源：http://nh.huanxung.cn

PHP:  range(0, 10, 2);
来源：http://lr.asd995.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ga.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ul.asd995.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ep.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://km.9csxet.cn

Ruby: (0...10).step(2).to_a
来源：http://zw.szxytkj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fg.huixiangedu.cn

[B12] 跳出多层循环
来源：http://wg.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vs.newstarts.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vg.hahajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tl.hnjuh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://my.jianghongdianzi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ky.jctech888.com.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pj.haigaiapp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cx.jianghongdianzi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yl.szsharing.cn

[B13] 判断是否为数字
来源：http://ma.colortex.cn

Py:   isinstance(x, (int, float))
来源：http://ys.huixinmuqiang.cn

PHP:  is_numeric($x)
来源：http://gz.chemitech.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sl.bookmarksfly.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://no.haigaiapp.cn

Java: x instanceof Number
来源：http://hk.szxytkj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wk.muxihuayi.cn

Ruby: x.is_a?(Numeric)
来源：http://nv.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://nj.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://an.hahajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://de.muxihuayi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kk.bookmarksfly.cn

JS:   [1, 2, 3].includes(x)
来源：http://ii.gzmigu.cn

TS:   [1, 2, 3].includes(x)
来源：http://rk.szxytkj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rw.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xw.shtwfgs.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jz.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vi.hahajie.cn

[B15] 布尔运算与取反
来源：http://tq.shxzskj.cn

Py:   a and b or not c
来源：http://hf.9csxet.cn

PHP:  $a && $b || !$c
来源：http://zu.jctech888.com.cn

JS:   a && b || !c
来源：http://dx.hnjuh.cn

TS:   a && b || !c
来源：http://im.shtwfgs.cn

Java: a && b || !c
来源：http://md.haigaiapp.cn

Go:   a && b || !c
来源：http://ir.hahajie.cn

Ruby: a && b || !c
来源：http://kw.hnjuh.cn

C#:   a && b || !c
来源：http://hv.shxzskj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gn.newstarts.cn

Py:   if not data: return
来源：http://jw.shxzukj.cn

PHP:  if (!$data) { return; }
来源：http://mo.jianghongdianzi.cn

JS:   if (!data) return;
来源：http://qk.yuntaijiaju.cn

TS:   if (!data) return;
来源：http://qc.bjjhwx.cn

Java: if (data == null) return;
来源：http://bm.gzmigu.cn

Go:   if data == nil { return }
来源：http://ea.newstarts.cn

Ruby: return if data.nil?
来源：http://xt.newstarts.cn

C#:   if (data == null) return;
来源：http://zr.jianghongdianzi.cn

================================================================================
来源：http://hk.newstarts.cn

C. 函数与作用域
来源：http://xb.shxzskj.cn

================================================================================
来源：http://ck.shxzukj.cn

[C01] 定义函数
来源：http://rv.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://br.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tl.wgjwhj.cn

JS:   function add(a, b) { return a + b; }
来源：http://vq.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lp.yuntaijiaju.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zh.szxytkj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kk.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://pc.haigaiapp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oy.wgjwhj.cn

[C02] 默认参数
来源：http://dl.yuexingan06.cn

Py:   def greet(name="World"): return name
来源：http://pe.521024.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jp.shxzskj.cn

JS:   function greet(name = "World") { return name; }
来源：http://hs.muxihuayi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pk.yuntaijiaju.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vg.bjjhwx.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fr.wgjwhj.cn

Ruby: def greet(name = "World") = name
来源：http://fr.hnjuh.cn

C#:   string Greet(string name = "World") => name;
来源：http://kq.lnxyls.cn

[C03] 可变参数
来源：http://uo.asd995.cn

Py:   def total(*args): return sum(args)
来源：http://ep.szxytkj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ym.nicolike.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lz.newstarts.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mm.shxzskj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xl.bjjhwx.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jv.lnxyls.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xo.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tr.lnxyls.cn

[C04] 命名参数 / 关键字参数
来源：http://vu.yuntaijiaju.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hv.yuexingan06.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qq.huanxung.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pm.shtwfgs.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vs.haigaiapp.cn

Java: // 无：用 Builder 模式或 record
来源：http://fq.nszjky.cn


<!-- 参考信息 -->