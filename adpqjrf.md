代发 wailian999

Ruby: value = data || "默认值"
来源：http://jw.shtwfgs.cn

C#:   var value = data ?? "默认值";
来源：http://pg.bookmarksfly.cn

[A16] 真假值判断规则
来源：http://ip.521024.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kv.shxzukj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gu.jctech888.com.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dt.shtwfgs.cn

TS:   if (!x) {}
来源：http://zo.szsharing.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ns.panjiajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dd.colortex.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ow.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fe.panjiajie.cn

[A17] 位运算
来源：http://at.gzmigu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://am.newstarts.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ig.wgjwhj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cs.yuntaijiaju.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ge.szsharing.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xr.panjiajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wf.newstarts.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ru.jianghongdianzi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wt.lnxyls.cn

[A18] 字符与 ASCII 码互转
来源：http://st.shxzskj.cn

Py:   ord("A"); chr(65)
来源：http://us.huanxung.cn

PHP:  ord("A"); chr(65)
来源：http://ie.yuntaijiaju.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mm.shxzskj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cl.haigaiapp.cn

Java: (int) 'A'; (char) 65
来源：http://ye.shxzskj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://sy.yuexingan06.cn

Ruby: "A".ord; 65.chr
来源：http://gj.shxzskj.cn

C#:   (int)'A'; (char)65
来源：http://sd.huixiangedu.cn

[A19] 交换两个变量
来源：http://wp.szxytkj.cn

Py:   a, b = b, a
来源：http://dt.shxzskj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://lp.jianghongdianzi.cn

JS:   [a, b] = [b, a];
来源：http://tc.yuntaijiaju.cn

TS:   [a, b] = [b, a];
来源：http://sk.szsharing.cn

Java: int t = a; a = b; b = t;
来源：http://zi.nszjky.cn

Go:   a, b = b, a
来源：http://mi.bjjhwx.cn

Ruby: a, b = b, a
来源：http://of.shtwfgs.cn

C#:   (a, b) = (b, a);
来源：http://td.haigaiapp.cn

[A20] 读取标准输入
来源：http://uh.haigaiapp.cn

Py:   name = input("请输入：")
来源：http://cb.yuntaijiaju.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://hn.yuexingan06.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://oq.yuexingan06.cn

TS:   // Node.js：readline 模块
来源：http://ge.wgjwhj.cn

Java: new Scanner(System.in).nextLine()
来源：http://nh.hahajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ux.hahajie.cn

Ruby: gets.chomp
来源：http://zk.shxzskj.cn

C#:   Console.ReadLine();
来源：http://jc.shxzukj.cn

[A21] 保留指定小数位输出
来源：http://pg.wgjwhj.cn

Py:   f"{3.14159:.2f}"
来源：http://fa.chemitech.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ay.huixiangedu.cn

JS:   (3.14159).toFixed(2)
来源：http://fl.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://sj.yuntaijiaju.cn

Java: String.format("%.2f", 3.14159)
来源：http://tf.nszjky.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bt.szsharing.cn

Ruby: format("%.2f", 3.14159)
来源：http://lu.huixinmuqiang.cn

C#:   3.14159.ToString("F2")
来源：http://vv.521024.cn

[A22] 获取字符串长度
来源：http://hl.lnxyls.cn

Py:   len(s)
来源：http://fn.huanxung.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://be.9csxet.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ye.hnjuh.cn

TS:   s.length
来源：http://sx.shtwfgs.cn

Java: s.length()
来源：http://ej.muxihuayi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ee.wgjwhj.cn

Ruby: s.length
来源：http://ov.newstarts.cn

C#:   s.Length
来源：http://xc.hahajie.cn

[A23] 大小写转换
来源：http://to.hahajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qk.muxihuayi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hj.hnjuh.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ad.521024.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bs.shxzukj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dm.chemitech.net.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://uo.yuntaijiaju.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ko.shxzukj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ah.huixiangedu.cn

[A24] 去除首尾空白
来源：http://bw.shxzskj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ry.shxzukj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ba.asd995.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mp.bookmarksfly.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ca.lnxyls.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://he.colortex.cn

Go:   strings.TrimSpace(s)
来源：http://pz.jianghongdianzi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wv.yuntaijiaju.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://od.huixiangedu.cn

[A25] 字符串比较
来源：http://sf.huanxung.cn

Py:   s1 == s2; s1 != s2
来源：http://nx.jctech888.com.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uu.nszjky.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hh.haigaiapp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lf.szsharing.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hh.shxzskj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tk.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ii.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jz.hahajie.cn

[A26] 类型转换总览
来源：http://yu.haigaiapp.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rb.9csxet.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bl.521024.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bt.szsharing.cn

TS:   Number() String() Boolean() x as number
来源：http://iz.huixiangedu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pw.521024.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ro.chemitech.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://sw.hnjuh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jf.shxzskj.cn

================================================================================
来源：http://ko.jctech888.com.cn

B. 流程控制
来源：http://ok.yuntaijiaju.cn

================================================================================
来源：http://rc.521024.cn

[B01] 条件判断 if / else
来源：http://po.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mk.huixinmuqiang.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://te.521024.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://eu.yuntaijiaju.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ch.jianghongdianzi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zi.chemitech.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://le.colortex.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ss.chemitech.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ln.asd995.cn

[B02] 多分支 else if / elif
来源：http://zb.muxihuayi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xy.nicolike.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gs.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://te.newstarts.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gf.yuntaijiaju.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ds.yuexingan06.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jk.newstarts.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://om.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fe.huanxung.cn

[B03] switch / match / case
来源：http://va.yuexingan06.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://my.9csxet.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uw.szsharing.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ke.muxihuayi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wn.hnjuh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ps.haigaiapp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ny.9csxet.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://io.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zc.521024.cn

[B04] for 计数循环
来源：http://fk.shtwfgs.cn

Py:   for i in range(10): print(i)
来源：http://ap.huanxung.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xu.yuntaijiaju.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ax.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kt.panjiajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vd.bookmarksfly.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ns.jianghongdianzi.cn

Ruby: 10.times { |i| puts i }
来源：http://bv.szxytkj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vp.hahajie.cn

[B05] 遍历数组 / 列表
来源：http://wx.hnjuh.cn

Py:   for item in arr: print(item)
来源：http://px.lnxyls.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tf.jianghongdianzi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ts.hahajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qg.bjjhwx.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mp.szxytkj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yv.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://bp.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zm.muxihuayi.cn

[B06] 遍历字典 / 对象
来源：http://ve.yuntaijiaju.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://br.hnjuh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://of.shtwfgs.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iu.bjjhwx.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sm.szxytkj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yz.lnxyls.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oj.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nn.lnxyls.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gk.hnjuh.cn

[B07] while 循环
来源：http://dr.colortex.cn

Py:   while i < 10: i += 1
来源：http://bz.panjiajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nk.9csxet.cn

JS:   while (i < 10) { i++; }
来源：http://oa.shtwfgs.cn

TS:   while (i < 10) { i++; }
来源：http://ad.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://nk.shtwfgs.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kh.nszjky.cn

Ruby: while i < 10; i += 1; end
来源：http://rx.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://lo.shtwfgs.cn

[B08] do-while（至少执行一次）
来源：http://is.yuntaijiaju.cn

Py:   # 无 do-while：用 while True + break
来源：http://vh.wgjwhj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://op.nszjky.cn

JS:   do { i++; } while (i < 10);
来源：http://gp.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://aa.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://jb.shxzskj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sz.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://du.chemitech.net.cn

C#:   do { i++; } while (i < 10);
来源：http://sx.huixinmuqiang.cn

[B09] break 与 continue
来源：http://ll.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://js.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gb.nszjky.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bi.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pb.asd995.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ol.jianghongdianzi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hb.asd995.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ox.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jp.jianghongdianzi.cn

[B10] 遍历同时拿索引
来源：http://md.yuexingan06.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ns.panjiajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://la.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lx.hnjuh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://un.asd995.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gw.szsharing.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ss.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ko.newstarts.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fa.521024.cn

[B11] 生成数字序列 / 区间
来源：http://fo.colortex.cn

Py:   list(range(0, 10, 2))
来源：http://ji.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://fr.jianghongdianzi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hn.hnjuh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oo.jianghongdianzi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ad.szsharing.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hk.gzmigu.cn

Ruby: (0...10).step(2).to_a
来源：http://ux.haigaiapp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fu.yuexingan06.cn

[B12] 跳出多层循环
来源：http://oi.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cb.yuexingan06.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nl.huixinmuqiang.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sb.bjjhwx.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mp.huixinmuqiang.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sr.bjjhwx.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lq.lnxyls.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vy.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pl.9csxet.cn

[B13] 判断是否为数字
来源：http://kr.nicolike.cn

Py:   isinstance(x, (int, float))
来源：http://qp.nicolike.cn

PHP:  is_numeric($x)
来源：http://sv.asd995.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ll.shxzukj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xn.chemitech.net.cn

Java: x instanceof Number
来源：http://jt.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ky.nicolike.cn

Ruby: x.is_a?(Numeric)
来源：http://zx.lnxyls.cn

C#:   x is int or double or decimal
来源：http://ex.colortex.cn

[B14] 判断值是否在集合内
来源：http://lu.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uo.shtwfgs.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jk.hahajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://he.521024.cn

TS:   [1, 2, 3].includes(x)
来源：http://rh.szxytkj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dh.yuexingan06.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lj.bookmarksfly.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gk.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dv.jctech888.com.cn

[B15] 布尔运算与取反
来源：http://dr.nszjky.cn

Py:   a and b or not c
来源：http://gi.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://ug.nicolike.cn

JS:   a && b || !c
来源：http://kf.yuexingan06.cn

TS:   a && b || !c
来源：http://su.huixinmuqiang.cn

Java: a && b || !c
来源：http://cc.yuexingan06.cn

Go:   a && b || !c
来源：http://jy.gzmigu.cn

Ruby: a && b || !c
来源：http://bd.gzmigu.cn

C#:   a && b || !c
来源：http://qf.521024.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bx.szsharing.cn

Py:   if not data: return
来源：http://qs.colortex.cn

PHP:  if (!$data) { return; }
来源：http://rc.lnxyls.cn

JS:   if (!data) return;
来源：http://eu.chemitech.net.cn

TS:   if (!data) return;
来源：http://od.nicolike.cn

Java: if (data == null) return;
来源：http://op.muxihuayi.cn

Go:   if data == nil { return }
来源：http://pf.wgjwhj.cn

Ruby: return if data.nil?
来源：http://pf.yuntaijiaju.cn

C#:   if (data == null) return;
来源：http://oq.bjjhwx.cn

================================================================================
来源：http://ds.bookmarksfly.cn

C. 函数与作用域
来源：http://tp.asd995.cn

================================================================================
来源：http://ry.bookmarksfly.cn

[C01] 定义函数
来源：http://lk.nicolike.cn

Py:   def add(a, b): return a + b
来源：http://ve.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gp.bjjhwx.cn

JS:   function add(a, b) { return a + b; }
来源：http://lt.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gl.newstarts.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fn.asd995.cn

Go:   func add(a, b int) int { return a + b }
来源：http://am.yuntaijiaju.cn

Ruby: def add(a, b); a + b; end
来源：http://fs.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xu.wgjwhj.cn

[C02] 默认参数
来源：http://kh.huixinmuqiang.cn

Py:   def greet(name="World"): return name
来源：http://ho.shtwfgs.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://df.hahajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://fg.yuexingan06.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://uk.newstarts.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fu.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ms.szxytkj.cn

Ruby: def greet(name = "World") = name
来源：http://ol.shtwfgs.cn

C#:   string Greet(string name = "World") => name;
来源：http://zf.yuexingan06.cn

[C03] 可变参数
来源：http://zj.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://ec.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hr.shxzskj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mv.shtwfgs.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cf.hahajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zo.hnjuh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gv.wgjwhj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mi.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fq.hahajie.cn

[C04] 命名参数 / 关键字参数
来源：http://mb.huixinmuqiang.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jb.haigaiapp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sl.asd995.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yj.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://iy.hnjuh.cn

Java: // 无：用 Builder 模式或 record
来源：http://bu.bookmarksfly.cn

Go:   // 无：用配置结构体参数
来源：http://xm.jctech888.com.cn

Ruby: f(a: 1, b: 2)
来源：http://bs.hahajie.cn

C#:   f(a: 1, b: 2)
来源：http://qt.nszjky.cn

[C05] 返回多个值
来源：http://jx.lnxyls.cn

Py:   return a, b
来源：http://at.hnjuh.cn

PHP:  return [$a, $b];
来源：http://he.haigaiapp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jy.huanxung.cn

TS:   return { a, b };
来源：http://hv.bjjhwx.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vl.haigaiapp.cn

Go:   return a, b
来源：http://ro.yuexingan06.cn

Ruby: return a, b
来源：http://ek.chemitech.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://za.shtwfgs.cn

[C06] 匿名函数 / lambda
来源：http://ya.bjjhwx.cn

Py:   square = lambda x: x * x
来源：http://la.nszjky.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kp.wgjwhj.cn

JS:   const square = x => x * x;
来源：http://kh.jianghongdianzi.cn


<!-- 参考信息 -->