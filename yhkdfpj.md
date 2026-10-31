代发 wailian999

[A14] 注释写法
来源：http://oq.jctech888.com.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://td.szsharing.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tc.hahajie.cn

JS:   // 单行；/* 多行 */
来源：http://bl.lnxyls.cn

TS:   // 单行；/* 多行 */
来源：http://nl.yuntaijiaju.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://za.9csxet.cn

Go:   // 单行；/* 多行 */
来源：http://cm.521024.cn

Ruby: # 单行；=begin 多行 =end
来源：http://jt.szxytkj.cn

C#:   // 单行；/* 多行 */
来源：http://xv.muxihuayi.cn

[A15] 空值判断与默认值
来源：http://sp.huixiangedu.cn

Py:   value = data or "默认值"
来源：http://nc.bookmarksfly.cn

PHP:  $value = $data ?? "默认值";
来源：http://lz.gzmigu.cn

JS:   const value = data ?? "默认值";
来源：http://it.colortex.cn

TS:   const value = data ?? "默认值";
来源：http://yq.huixinmuqiang.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://lk.hahajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://zl.521024.cn

Ruby: value = data || "默认值"
来源：http://dm.nicolike.cn

C#:   var value = data ?? "默认值";
来源：http://rr.huanxung.cn

[A16] 真假值判断规则
来源：http://wm.nszjky.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lc.colortex.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://sh.hahajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mq.yuntaijiaju.cn

TS:   if (!x) {}
来源：http://zh.colortex.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dy.bookmarksfly.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wg.szxytkj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xf.hahajie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gy.bookmarksfly.cn

[A17] 位运算
来源：http://oq.huixiangedu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kp.hahajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.huanxung.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sf.panjiajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qe.yuntaijiaju.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mj.jctech888.com.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://li.shxzskj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bh.nicolike.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wv.haigaiapp.cn

[A18] 字符与 ASCII 码互转
来源：http://ps.hahajie.cn

Py:   ord("A"); chr(65)
来源：http://wx.colortex.cn

PHP:  ord("A"); chr(65)
来源：http://fu.muxihuayi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cj.newstarts.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xk.shxzukj.cn

Java: (int) 'A'; (char) 65
来源：http://ep.shxzskj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qd.shtwfgs.cn

Ruby: "A".ord; 65.chr
来源：http://zr.nszjky.cn

C#:   (int)'A'; (char)65
来源：http://ed.asd995.cn

[A19] 交换两个变量
来源：http://of.lnxyls.cn

Py:   a, b = b, a
来源：http://nb.yuexingan06.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://se.shxzukj.cn

JS:   [a, b] = [b, a];
来源：http://jo.colortex.cn

TS:   [a, b] = [b, a];
来源：http://ma.bjjhwx.cn

Java: int t = a; a = b; b = t;
来源：http://cb.bjjhwx.cn

Go:   a, b = b, a
来源：http://mm.szsharing.cn

Ruby: a, b = b, a
来源：http://uv.jianghongdianzi.cn

C#:   (a, b) = (b, a);
来源：http://dy.haigaiapp.cn

[A20] 读取标准输入
来源：http://gk.shxzskj.cn

Py:   name = input("请输入：")
来源：http://us.panjiajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://eq.gzmigu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wm.huixinmuqiang.cn

TS:   // Node.js：readline 模块
来源：http://ay.jianghongdianzi.cn

Java: new Scanner(System.in).nextLine()
来源：http://tu.hahajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://th.hahajie.cn

Ruby: gets.chomp
来源：http://wb.newstarts.cn

C#:   Console.ReadLine();
来源：http://eq.yuexingan06.cn

[A21] 保留指定小数位输出
来源：http://bz.huanxung.cn

Py:   f"{3.14159:.2f}"
来源：http://yj.haigaiapp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mb.yuexingan06.cn

JS:   (3.14159).toFixed(2)
来源：http://sc.jianghongdianzi.cn

TS:   (3.14159).toFixed(2)
来源：http://vy.nszjky.cn

Java: String.format("%.2f", 3.14159)
来源：http://sv.hnjuh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ag.huixinmuqiang.cn

Ruby: format("%.2f", 3.14159)
来源：http://qu.chemitech.net.cn

C#:   3.14159.ToString("F2")
来源：http://aw.jctech888.com.cn

[A22] 获取字符串长度
来源：http://xr.newstarts.cn

Py:   len(s)
来源：http://ww.hahajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://um.shtwfgs.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ee.szsharing.cn

TS:   s.length
来源：http://kg.szsharing.cn

Java: s.length()
来源：http://sy.hnjuh.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nk.yuexingan06.cn

Ruby: s.length
来源：http://jl.huanxung.cn

C#:   s.Length
来源：http://iz.huanxung.cn

[A23] 大小写转换
来源：http://ag.szxytkj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qm.521024.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hy.colortex.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mt.shtwfgs.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ez.bjjhwx.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ye.wgjwhj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wd.yuntaijiaju.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xy.hahajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gb.lnxyls.cn

[A24] 去除首尾空白
来源：http://cr.colortex.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ev.muxihuayi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://os.hnjuh.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lo.shtwfgs.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ha.nicolike.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://oq.chemitech.net.cn

Go:   strings.TrimSpace(s)
来源：http://mg.yuexingan06.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fa.shtwfgs.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wr.521024.cn

[A25] 字符串比较
来源：http://td.shxzskj.cn

Py:   s1 == s2; s1 != s2
来源：http://gm.huixiangedu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://of.nicolike.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bt.chemitech.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ti.jctech888.com.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ot.shtwfgs.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zf.bjjhwx.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nd.shtwfgs.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fk.huixiangedu.cn

[A26] 类型转换总览
来源：http://dh.chemitech.net.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sa.szxytkj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sk.huanxung.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fl.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://bk.colortex.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sf.shxzukj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://av.szsharing.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ce.huixinmuqiang.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wj.haigaiapp.cn

================================================================================
来源：http://ia.panjiajie.cn

B. 流程控制
来源：http://sy.huixinmuqiang.cn

================================================================================
来源：http://wu.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://kd.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gl.hahajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nh.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bf.gzmigu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jj.hahajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sg.hnjuh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fl.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qr.hnjuh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://da.jianghongdianzi.cn

[B02] 多分支 else if / elif
来源：http://vf.wgjwhj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://px.bjjhwx.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ya.huanxung.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yj.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pv.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vw.newstarts.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://em.jianghongdianzi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jl.jianghongdianzi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cu.shxzskj.cn

[B03] switch / match / case
来源：http://ey.bookmarksfly.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nr.newstarts.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://iy.asd995.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pi.bjjhwx.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://km.gzmigu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qi.huanxung.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hl.bjjhwx.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jy.shxzukj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ck.jctech888.com.cn

[B04] for 计数循环
来源：http://lq.shtwfgs.cn

Py:   for i in range(10): print(i)
来源：http://oq.nszjky.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ly.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://af.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lb.newstarts.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bi.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rw.haigaiapp.cn

Ruby: 10.times { |i| puts i }
来源：http://ey.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.huixinmuqiang.cn

[B05] 遍历数组 / 列表
来源：http://se.9csxet.cn

Py:   for item in arr: print(item)
来源：http://bh.chemitech.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rw.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qv.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yr.shtwfgs.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yj.jianghongdianzi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qc.szsharing.cn

Ruby: arr.each { |item| puts item }
来源：http://cj.colortex.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ag.panjiajie.cn

[B06] 遍历字典 / 对象
来源：http://yg.szxytkj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://np.huixiangedu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jz.lnxyls.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wu.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jx.muxihuayi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ve.hahajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tn.panjiajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lj.9csxet.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fi.shtwfgs.cn

[B07] while 循环
来源：http://oo.newstarts.cn

Py:   while i < 10: i += 1
来源：http://lw.huanxung.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mz.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://mw.huixiangedu.cn

TS:   while (i < 10) { i++; }
来源：http://un.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://ia.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ur.521024.cn

Ruby: while i < 10; i += 1; end
来源：http://yv.asd995.cn

C#:   while (i < 10) { i++; }
来源：http://af.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://ch.szsharing.cn

Py:   # 无 do-while：用 while True + break
来源：http://ly.bjjhwx.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qb.newstarts.cn

JS:   do { i++; } while (i < 10);
来源：http://bx.huanxung.cn

TS:   do { i++; } while (i < 10);
来源：http://ww.wgjwhj.cn

Java: do { i++; } while (i < 10);
来源：http://tm.colortex.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sa.jianghongdianzi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://om.hahajie.cn

C#:   do { i++; } while (i < 10);
来源：http://dt.chemitech.net.cn

[B09] break 与 continue
来源：http://mw.yuntaijiaju.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dh.nszjky.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gk.szsharing.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://or.nszjky.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rp.huixiangedu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fh.panjiajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sw.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ju.9csxet.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gf.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://ft.shxzukj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dt.huanxung.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qu.shxzukj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zt.wgjwhj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fp.chemitech.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ji.gzmigu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ac.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mw.yuntaijiaju.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://um.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://ng.hnjuh.cn

Py:   list(range(0, 10, 2))
来源：http://pd.wgjwhj.cn

PHP:  range(0, 10, 2);
来源：http://ey.lnxyls.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bg.nicolike.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cv.hahajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xi.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://au.colortex.cn

Ruby: (0...10).step(2).to_a
来源：http://vh.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tv.szxytkj.cn

[B12] 跳出多层循环
来源：http://jv.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://dz.shtwfgs.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bn.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hu.huixiangedu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sl.newstarts.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hq.521024.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tt.colortex.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ug.yuntaijiaju.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fa.chemitech.net.cn

[B13] 判断是否为数字
来源：http://lu.lnxyls.cn

Py:   isinstance(x, (int, float))
来源：http://lr.9csxet.cn

PHP:  is_numeric($x)
来源：http://yf.chemitech.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fs.hahajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uf.jctech888.com.cn

Java: x instanceof Number
来源：http://ag.huixiangedu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tk.hnjuh.cn

Ruby: x.is_a?(Numeric)
来源：http://zf.huixiangedu.cn

C#:   x is int or double or decimal
来源：http://wv.shtwfgs.cn

[B14] 判断值是否在集合内
来源：http://gm.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qi.lnxyls.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ip.wgjwhj.cn

JS:   [1, 2, 3].includes(x)
来源：http://nk.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://oe.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://of.newstarts.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ka.lnxyls.cn

Ruby: [1, 2, 3].include?(x)
来源：http://se.chemitech.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://eo.9csxet.cn

[B15] 布尔运算与取反
来源：http://mw.jianghongdianzi.cn

Py:   a and b or not c
来源：http://gw.haigaiapp.cn

PHP:  $a && $b || !$c
来源：http://ph.bookmarksfly.cn

JS:   a && b || !c
来源：http://ti.newstarts.cn

TS:   a && b || !c
来源：http://om.bookmarksfly.cn

Java: a && b || !c
来源：http://rt.hnjuh.cn

Go:   a && b || !c
来源：http://vw.hnjuh.cn

Ruby: a && b || !c
来源：http://jp.yuntaijiaju.cn

C#:   a && b || !c
来源：http://zs.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qq.huanxung.cn

Py:   if not data: return
来源：http://dk.huixinmuqiang.cn

PHP:  if (!$data) { return; }
来源：http://mc.bookmarksfly.cn

JS:   if (!data) return;
来源：http://ad.hnjuh.cn

TS:   if (!data) return;
来源：http://ln.huixiangedu.cn

Java: if (data == null) return;
来源：http://dw.yuexingan06.cn

Go:   if data == nil { return }
来源：http://io.521024.cn

Ruby: return if data.nil?
来源：http://ff.gzmigu.cn

C#:   if (data == null) return;
来源：http://pr.9csxet.cn

================================================================================
来源：http://kp.shxzukj.cn

C. 函数与作用域
来源：http://xt.huixiangedu.cn

================================================================================
来源：http://uy.hahajie.cn

[C01] 定义函数
来源：http://ie.nicolike.cn

Py:   def add(a, b): return a + b
来源：http://nu.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ds.521024.cn

JS:   function add(a, b) { return a + b; }
来源：http://mp.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gm.huixiangedu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yy.huixinmuqiang.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xt.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://zw.huanxung.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ye.lnxyls.cn

[C02] 默认参数
来源：http://vu.haigaiapp.cn

Py:   def greet(name="World"): return name
来源：http://wg.yuntaijiaju.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://aq.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://em.colortex.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://za.shtwfgs.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pv.yuntaijiaju.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fh.shxzskj.cn

Ruby: def greet(name = "World") = name
来源：http://pl.jctech888.com.cn

C#:   string Greet(string name = "World") => name;
来源：http://nn.muxihuayi.cn

[C03] 可变参数
来源：http://gc.huixiangedu.cn

Py:   def total(*args): return sum(args)
来源：http://eh.newstarts.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tg.szxytkj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lw.huixinmuqiang.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zb.nicolike.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://th.wgjwhj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://md.asd995.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qs.panjiajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dp.newstarts.cn

[C04] 命名参数 / 关键字参数
来源：http://yr.szxytkj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zh.shtwfgs.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bw.shxzskj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ni.szxytkj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ef.szxytkj.cn

Java: // 无：用 Builder 模式或 record
来源：http://fr.gzmigu.cn


<!-- 参考信息 -->