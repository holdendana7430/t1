代发 wailian999

[A14] 注释写法
来源：http://cp.gzmigu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ul.asd995.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ep.huanxung.cn

JS:   // 单行；/* 多行 */
来源：http://cw.gzmigu.cn

TS:   // 单行；/* 多行 */
来源：http://nl.jianghongdianzi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ud.szxytkj.cn

Go:   // 单行；/* 多行 */
来源：http://lt.jctech888.com.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vz.bookmarksfly.cn

C#:   // 单行；/* 多行 */
来源：http://zm.yuntaijiaju.cn

[A15] 空值判断与默认值
来源：http://rg.szsharing.cn

Py:   value = data or "默认值"
来源：http://sn.szxytkj.cn

PHP:  $value = $data ?? "默认值";
来源：http://nr.panjiajie.cn

JS:   const value = data ?? "默认值";
来源：http://oj.huanxung.cn

TS:   const value = data ?? "默认值";
来源：http://kx.bookmarksfly.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ac.muxihuayi.cn

Go:   if data == "" { data = "默认值" }
来源：http://vh.hnjuh.cn

Ruby: value = data || "默认值"
来源：http://kk.huixiangedu.cn

C#:   var value = data ?? "默认值";
来源：http://wh.521024.cn

[A16] 真假值判断规则
来源：http://je.yuntaijiaju.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://uo.szxytkj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cm.hnjuh.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cu.newstarts.cn

TS:   if (!x) {}
来源：http://tg.wgjwhj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qf.jctech888.com.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bx.szsharing.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xs.lnxyls.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://is.shxzskj.cn

[A17] 位运算
来源：http://fg.yuntaijiaju.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ys.szsharing.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ui.newstarts.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://db.colortex.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wl.huixinmuqiang.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rl.asd995.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ee.szsharing.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://we.wgjwhj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ac.shxzukj.cn

[A18] 字符与 ASCII 码互转
来源：http://nv.chemitech.net.cn

Py:   ord("A"); chr(65)
来源：http://ps.wgjwhj.cn

PHP:  ord("A"); chr(65)
来源：http://ls.shxzskj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lh.hahajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wk.bookmarksfly.cn

Java: (int) 'A'; (char) 65
来源：http://sa.9csxet.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bl.9csxet.cn

Ruby: "A".ord; 65.chr
来源：http://yd.chemitech.net.cn

C#:   (int)'A'; (char)65
来源：http://sl.hnjuh.cn

[A19] 交换两个变量
来源：http://cf.szxytkj.cn

Py:   a, b = b, a
来源：http://jv.huixiangedu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fn.bookmarksfly.cn

JS:   [a, b] = [b, a];
来源：http://dq.bjjhwx.cn

TS:   [a, b] = [b, a];
来源：http://ii.colortex.cn

Java: int t = a; a = b; b = t;
来源：http://cj.haigaiapp.cn

Go:   a, b = b, a
来源：http://cg.9csxet.cn

Ruby: a, b = b, a
来源：http://fe.huixiangedu.cn

C#:   (a, b) = (b, a);
来源：http://lj.jctech888.com.cn

[A20] 读取标准输入
来源：http://eq.chemitech.net.cn

Py:   name = input("请输入：")
来源：http://at.huanxung.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://my.szsharing.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lp.colortex.cn

TS:   // Node.js：readline 模块
来源：http://ww.nszjky.cn

Java: new Scanner(System.in).nextLine()
来源：http://rj.huanxung.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ef.nszjky.cn

Ruby: gets.chomp
来源：http://pr.gzmigu.cn

C#:   Console.ReadLine();
来源：http://dt.szsharing.cn

[A21] 保留指定小数位输出
来源：http://oa.lnxyls.cn

Py:   f"{3.14159:.2f}"
来源：http://ey.asd995.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yx.hnjuh.cn

JS:   (3.14159).toFixed(2)
来源：http://ln.shxzskj.cn

TS:   (3.14159).toFixed(2)
来源：http://bk.bjjhwx.cn

Java: String.format("%.2f", 3.14159)
来源：http://ql.haigaiapp.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ts.shxzskj.cn

Ruby: format("%.2f", 3.14159)
来源：http://cg.szsharing.cn

C#:   3.14159.ToString("F2")
来源：http://ok.huixiangedu.cn

[A22] 获取字符串长度
来源：http://fr.haigaiapp.cn

Py:   len(s)
来源：http://zj.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://do.huanxung.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fz.asd995.cn

TS:   s.length
来源：http://aa.chemitech.net.cn

Java: s.length()
来源：http://ax.colortex.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ae.szsharing.cn

Ruby: s.length
来源：http://oc.haigaiapp.cn

C#:   s.Length
来源：http://br.jianghongdianzi.cn

[A23] 大小写转换
来源：http://nh.hahajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kc.yuntaijiaju.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ds.newstarts.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://iq.shxzukj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://co.9csxet.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zx.hnjuh.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ib.9csxet.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dq.shxzskj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://tc.shxzukj.cn

[A24] 去除首尾空白
来源：http://lw.lnxyls.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ub.gzmigu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qn.huixinmuqiang.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://il.panjiajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fb.yuntaijiaju.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ug.nszjky.cn

Go:   strings.TrimSpace(s)
来源：http://rc.nicolike.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bh.521024.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mz.jctech888.com.cn

[A25] 字符串比较
来源：http://cq.bookmarksfly.cn

Py:   s1 == s2; s1 != s2
来源：http://fw.szxytkj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rh.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cs.huanxung.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rf.shxzukj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jp.jctech888.com.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fv.521024.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bs.yuexingan06.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rl.hahajie.cn

[A26] 类型转换总览
来源：http://gk.shxzukj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qh.hnjuh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qk.huixinmuqiang.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dt.hahajie.cn

TS:   Number() String() Boolean() x as number
来源：http://ec.colortex.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cs.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bq.yuexingan06.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://oq.chemitech.net.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pc.gzmigu.cn

================================================================================
来源：http://hp.szsharing.cn

B. 流程控制
来源：http://no.521024.cn

================================================================================
来源：http://xz.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://pn.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xf.chemitech.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bt.lnxyls.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wy.haigaiapp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ed.panjiajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tv.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xd.haigaiapp.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tv.nszjky.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ui.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://bm.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tq.yuexingan06.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gv.521024.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rt.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qa.nicolike.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fr.jctech888.com.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pa.521024.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yv.huanxung.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fz.colortex.cn

[B03] switch / match / case
来源：http://oy.hahajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vq.szsharing.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pb.bjjhwx.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hj.hnjuh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ev.shtwfgs.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ev.panjiajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tp.huanxung.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xp.huixinmuqiang.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gl.chemitech.net.cn

[B04] for 计数循环
来源：http://ks.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://ol.yuntaijiaju.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kx.lnxyls.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://th.bjjhwx.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rm.bookmarksfly.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yl.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wu.lnxyls.cn

Ruby: 10.times { |i| puts i }
来源：http://ro.bjjhwx.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pr.szsharing.cn

[B05] 遍历数组 / 列表
来源：http://ci.hnjuh.cn

Py:   for item in arr: print(item)
来源：http://nm.bookmarksfly.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zw.nszjky.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ky.colortex.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sl.wgjwhj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rs.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qf.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://la.lnxyls.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fc.nicolike.cn

[B06] 遍历字典 / 对象
来源：http://ip.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xi.huanxung.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://eh.hnjuh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yc.haigaiapp.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hh.521024.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hi.lnxyls.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lx.szxytkj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bg.jianghongdianzi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ii.newstarts.cn

[B07] while 循环
来源：http://xn.yuntaijiaju.cn

Py:   while i < 10: i += 1
来源：http://ok.huixiangedu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://sy.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://py.asd995.cn

TS:   while (i < 10) { i++; }
来源：http://sz.asd995.cn

Java: while (i < 10) { i++; }
来源：http://ci.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cp.nicolike.cn

Ruby: while i < 10; i += 1; end
来源：http://eb.yuexingan06.cn

C#:   while (i < 10) { i++; }
来源：http://qq.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://nx.hnjuh.cn

Py:   # 无 do-while：用 while True + break
来源：http://pj.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://re.muxihuayi.cn

JS:   do { i++; } while (i < 10);
来源：http://fn.panjiajie.cn

TS:   do { i++; } while (i < 10);
来源：http://wa.jianghongdianzi.cn

Java: do { i++; } while (i < 10);
来源：http://tt.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wr.chemitech.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dc.chemitech.net.cn

C#:   do { i++; } while (i < 10);
来源：http://sq.szsharing.cn

[B09] break 与 continue
来源：http://zr.jianghongdianzi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jo.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mf.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tw.muxihuayi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ul.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jw.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nl.yuexingan06.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wl.jianghongdianzi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pc.shxzukj.cn

[B10] 遍历同时拿索引
来源：http://sz.yuexingan06.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ho.szxytkj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fy.bjjhwx.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ev.szsharing.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qy.shxzukj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ug.hahajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mn.9csxet.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zy.hnjuh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gg.lnxyls.cn

[B11] 生成数字序列 / 区间
来源：http://hr.jctech888.com.cn

Py:   list(range(0, 10, 2))
来源：http://eb.huanxung.cn

PHP:  range(0, 10, 2);
来源：http://si.521024.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hr.gzmigu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zm.yuntaijiaju.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qe.bjjhwx.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wy.chemitech.net.cn

Ruby: (0...10).step(2).to_a
来源：http://ty.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vy.nicolike.cn

[B12] 跳出多层循环
来源：http://vz.szsharing.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uh.hahajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://uv.huixinmuqiang.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://er.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mc.huanxung.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ig.nicolike.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lo.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ux.bjjhwx.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pd.colortex.cn

[B13] 判断是否为数字
来源：http://nm.asd995.cn

Py:   isinstance(x, (int, float))
来源：http://zz.huixiangedu.cn

PHP:  is_numeric($x)
来源：http://es.hnjuh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mg.hahajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nr.gzmigu.cn

Java: x instanceof Number
来源：http://ik.muxihuayi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://iv.bookmarksfly.cn

Ruby: x.is_a?(Numeric)
来源：http://ho.szxytkj.cn

C#:   x is int or double or decimal
来源：http://bu.gzmigu.cn

[B14] 判断值是否在集合内
来源：http://js.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://is.huanxung.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gi.jianghongdianzi.cn

JS:   [1, 2, 3].includes(x)
来源：http://cv.panjiajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://nw.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pr.nicolike.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ft.muxihuayi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ya.szxytkj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zi.haigaiapp.cn

[B15] 布尔运算与取反
来源：http://yp.9csxet.cn

Py:   a and b or not c
来源：http://zj.521024.cn

PHP:  $a && $b || !$c
来源：http://ta.chemitech.net.cn

JS:   a && b || !c
来源：http://kr.yuexingan06.cn

TS:   a && b || !c
来源：http://tj.hahajie.cn

Java: a && b || !c
来源：http://pd.jianghongdianzi.cn

Go:   a && b || !c
来源：http://tw.yuntaijiaju.cn

Ruby: a && b || !c
来源：http://vu.szxytkj.cn

C#:   a && b || !c
来源：http://hq.hahajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gy.shxzukj.cn

Py:   if not data: return
来源：http://mx.shtwfgs.cn

PHP:  if (!$data) { return; }
来源：http://fa.haigaiapp.cn

JS:   if (!data) return;
来源：http://zd.521024.cn

TS:   if (!data) return;
来源：http://nr.szxytkj.cn

Java: if (data == null) return;
来源：http://of.newstarts.cn

Go:   if data == nil { return }
来源：http://sa.gzmigu.cn

Ruby: return if data.nil?
来源：http://gg.huixinmuqiang.cn

C#:   if (data == null) return;
来源：http://ir.huixiangedu.cn

================================================================================
来源：http://mw.hnjuh.cn

C. 函数与作用域
来源：http://hp.nszjky.cn

================================================================================
来源：http://bg.wgjwhj.cn

[C01] 定义函数
来源：http://nf.huixiangedu.cn

Py:   def add(a, b): return a + b
来源：http://qc.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ir.huanxung.cn

JS:   function add(a, b) { return a + b; }
来源：http://jq.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://au.nicolike.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kg.haigaiapp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ul.newstarts.cn

Ruby: def add(a, b); a + b; end
来源：http://yf.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ys.shxzskj.cn

[C02] 默认参数
来源：http://qa.muxihuayi.cn

Py:   def greet(name="World"): return name
来源：http://lm.hnjuh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://re.wgjwhj.cn

JS:   function greet(name = "World") { return name; }
来源：http://ra.hnjuh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qd.9csxet.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rw.muxihuayi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vy.panjiajie.cn

Ruby: def greet(name = "World") = name
来源：http://rw.asd995.cn

C#:   string Greet(string name = "World") => name;
来源：http://sb.yuntaijiaju.cn

[C03] 可变参数
来源：http://xv.muxihuayi.cn

Py:   def total(*args): return sum(args)
来源：http://xz.hnjuh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hd.haigaiapp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gq.nicolike.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ki.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ka.9csxet.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sa.9csxet.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zv.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ut.huixiangedu.cn

[C04] 命名参数 / 关键字参数
来源：http://dn.huixiangedu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kk.hnjuh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mp.shtwfgs.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://te.jianghongdianzi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ww.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://ev.521024.cn


<!-- 参考信息 -->