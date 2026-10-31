代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yy.yuntaijiaju.cn

Ruby: "Hello, #{name}!"
来源：http://zs.jianghongdianzi.cn

C#:   $"Hello, {name}!"
来源：http://qf.jianghongdianzi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ar.yuntaijiaju.cn

Py:   "第一行\n第二行"
来源：http://tw.lnxyls.cn

PHP:  "第一行\n第二行"
来源：http://rg.yuexingan06.cn

JS:   "第一行\n第二行"
来源：http://mi.szsharing.cn

TS:   "第一行\n第二行"
来源：http://td.haigaiapp.cn

Java: "第一行\n第二行"
来源：http://ny.chemitech.net.cn

Go:   "第一行\n第二行"
来源：http://br.bjjhwx.cn

Ruby: "第一行\n第二行"
来源：http://za.szsharing.cn

C#:   "第一行\n第二行"
来源：http://ss.yuntaijiaju.cn

[A14] 注释写法
来源：http://tq.lnxyls.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ib.bjjhwx.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://jn.jctech888.com.cn

JS:   // 单行；/* 多行 */
来源：http://vy.colortex.cn

TS:   // 单行；/* 多行 */
来源：http://hi.szsharing.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nd.panjiajie.cn

Go:   // 单行；/* 多行 */
来源：http://nn.9csxet.cn

Ruby: # 单行；=begin 多行 =end
来源：http://eo.muxihuayi.cn

C#:   // 单行；/* 多行 */
来源：http://hp.huixinmuqiang.cn

[A15] 空值判断与默认值
来源：http://yv.muxihuayi.cn

Py:   value = data or "默认值"
来源：http://og.jctech888.com.cn

PHP:  $value = $data ?? "默认值";
来源：http://wv.bjjhwx.cn

JS:   const value = data ?? "默认值";
来源：http://mu.nszjky.cn

TS:   const value = data ?? "默认值";
来源：http://ys.szxytkj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hr.huixinmuqiang.cn

Go:   if data == "" { data = "默认值" }
来源：http://ts.yuntaijiaju.cn

Ruby: value = data || "默认值"
来源：http://um.szsharing.cn

C#:   var value = data ?? "默认值";
来源：http://hj.newstarts.cn

[A16] 真假值判断规则
来源：http://wt.huanxung.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xk.bookmarksfly.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bi.jianghongdianzi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mt.hahajie.cn

TS:   if (!x) {}
来源：http://nu.huanxung.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qv.hahajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ak.hahajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xa.szxytkj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sw.wgjwhj.cn

[A17] 位运算
来源：http://hw.szxytkj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://os.jianghongdianzi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nn.nszjky.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mq.hahajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dg.hnjuh.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wy.szsharing.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kx.shxzukj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yz.shxzskj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rb.yuntaijiaju.cn

[A18] 字符与 ASCII 码互转
来源：http://jg.gzmigu.cn

Py:   ord("A"); chr(65)
来源：http://tp.szxytkj.cn

PHP:  ord("A"); chr(65)
来源：http://br.nicolike.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pf.shxzskj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uk.nszjky.cn

Java: (int) 'A'; (char) 65
来源：http://go.shxzukj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wz.lnxyls.cn

Ruby: "A".ord; 65.chr
来源：http://rs.muxihuayi.cn

C#:   (int)'A'; (char)65
来源：http://vq.shxzskj.cn

[A19] 交换两个变量
来源：http://gs.gzmigu.cn

Py:   a, b = b, a
来源：http://ot.huixiangedu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://dg.wgjwhj.cn

JS:   [a, b] = [b, a];
来源：http://xc.colortex.cn

TS:   [a, b] = [b, a];
来源：http://ll.muxihuayi.cn

Java: int t = a; a = b; b = t;
来源：http://xg.huixinmuqiang.cn

Go:   a, b = b, a
来源：http://nv.szxytkj.cn

Ruby: a, b = b, a
来源：http://xv.shtwfgs.cn

C#:   (a, b) = (b, a);
来源：http://nk.hnjuh.cn

[A20] 读取标准输入
来源：http://xz.jctech888.com.cn

Py:   name = input("请输入：")
来源：http://ry.newstarts.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://di.shxzukj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sn.huixinmuqiang.cn

TS:   // Node.js：readline 模块
来源：http://wf.jianghongdianzi.cn

Java: new Scanner(System.in).nextLine()
来源：http://mi.shxzskj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://op.huanxung.cn

Ruby: gets.chomp
来源：http://in.jianghongdianzi.cn

C#:   Console.ReadLine();
来源：http://bf.521024.cn

[A21] 保留指定小数位输出
来源：http://xy.nszjky.cn

Py:   f"{3.14159:.2f}"
来源：http://mb.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zu.jianghongdianzi.cn

JS:   (3.14159).toFixed(2)
来源：http://wa.521024.cn

TS:   (3.14159).toFixed(2)
来源：http://gl.hnjuh.cn

Java: String.format("%.2f", 3.14159)
来源：http://de.yuexingan06.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yr.shtwfgs.cn

Ruby: format("%.2f", 3.14159)
来源：http://dd.huanxung.cn

C#:   3.14159.ToString("F2")
来源：http://xl.nszjky.cn

[A22] 获取字符串长度
来源：http://gs.jianghongdianzi.cn

Py:   len(s)
来源：http://bk.jctech888.com.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mr.nszjky.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://he.huixiangedu.cn

TS:   s.length
来源：http://yk.yuntaijiaju.cn

Java: s.length()
来源：http://bb.haigaiapp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bv.shxzukj.cn

Ruby: s.length
来源：http://gw.hahajie.cn

C#:   s.Length
来源：http://bh.wgjwhj.cn

[A23] 大小写转换
来源：http://mo.chemitech.net.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ao.colortex.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rl.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ui.huixinmuqiang.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://az.jctech888.com.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://my.gzmigu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jp.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hq.lnxyls.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gv.hnjuh.cn

[A24] 去除首尾空白
来源：http://te.szsharing.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fm.gzmigu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yr.jctech888.com.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fs.szxytkj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vn.asd995.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fl.yuexingan06.cn

Go:   strings.TrimSpace(s)
来源：http://fj.szxytkj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xw.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qz.shxzukj.cn

[A25] 字符串比较
来源：http://vw.bookmarksfly.cn

Py:   s1 == s2; s1 != s2
来源：http://ga.asd995.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cl.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yh.521024.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kk.wgjwhj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sm.shxzukj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mt.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://eu.bookmarksfly.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cj.9csxet.cn

[A26] 类型转换总览
来源：http://td.521024.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hc.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://id.shxzukj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://td.bjjhwx.cn

TS:   Number() String() Boolean() x as number
来源：http://tc.chemitech.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pn.jianghongdianzi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zq.colortex.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kq.colortex.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pw.colortex.cn

================================================================================
来源：http://ub.jctech888.com.cn

B. 流程控制
来源：http://tm.jctech888.com.cn

================================================================================
来源：http://nf.huixiangedu.cn

[B01] 条件判断 if / else
来源：http://er.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xq.huixinmuqiang.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ul.jctech888.com.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nw.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gv.jianghongdianzi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xj.nicolike.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://am.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zt.newstarts.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jz.bjjhwx.cn

[B02] 多分支 else if / elif
来源：http://ge.shxzskj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://er.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ji.szxytkj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://al.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lu.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gc.szsharing.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://oi.panjiajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pr.hahajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xo.newstarts.cn

[B03] switch / match / case
来源：http://ey.shtwfgs.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jw.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gu.wgjwhj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://le.lnxyls.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vf.bookmarksfly.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://oy.shxzskj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qf.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://na.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://es.shxzukj.cn

[B04] for 计数循环
来源：http://hi.yuntaijiaju.cn

Py:   for i in range(10): print(i)
来源：http://hh.huixinmuqiang.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cc.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xi.szxytkj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yp.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qu.panjiajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vc.wgjwhj.cn

Ruby: 10.times { |i| puts i }
来源：http://zm.newstarts.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tl.yuexingan06.cn

[B05] 遍历数组 / 列表
来源：http://jn.lnxyls.cn

Py:   for item in arr: print(item)
来源：http://lv.shtwfgs.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ia.shtwfgs.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://al.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hk.chemitech.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nq.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sr.yuexingan06.cn

Ruby: arr.each { |item| puts item }
来源：http://bv.huanxung.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nq.jctech888.com.cn

[B06] 遍历字典 / 对象
来源：http://hs.wgjwhj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ci.huixiangedu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sv.panjiajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ih.521024.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uq.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gn.gzmigu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ln.huixinmuqiang.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gy.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jc.muxihuayi.cn

[B07] while 循环
来源：http://ue.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://po.huanxung.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gm.jctech888.com.cn

JS:   while (i < 10) { i++; }
来源：http://oq.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://pf.521024.cn

Java: while (i < 10) { i++; }
来源：http://fb.muxihuayi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rl.hnjuh.cn

Ruby: while i < 10; i += 1; end
来源：http://nn.chemitech.net.cn

C#:   while (i < 10) { i++; }
来源：http://ur.shxzskj.cn

[B08] do-while（至少执行一次）
来源：http://zd.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://ok.nicolike.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vr.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://fc.hnjuh.cn

TS:   do { i++; } while (i < 10);
来源：http://ka.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://tv.jianghongdianzi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mr.yuexingan06.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ua.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://hl.newstarts.cn

[B09] break 与 continue
来源：http://ip.hnjuh.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pf.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cj.szsharing.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gy.muxihuayi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ka.panjiajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fm.chemitech.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bv.yuexingan06.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ds.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zg.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://pj.huixiangedu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vt.yuntaijiaju.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://px.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ww.chemitech.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qo.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ym.jctech888.com.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sp.huixiangedu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rh.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kw.hnjuh.cn

[B11] 生成数字序列 / 区间
来源：http://cv.nicolike.cn

Py:   list(range(0, 10, 2))
来源：http://lz.bjjhwx.cn

PHP:  range(0, 10, 2);
来源：http://lg.wgjwhj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ij.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fa.huixiangedu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ew.szsharing.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tw.yuntaijiaju.cn

Ruby: (0...10).step(2).to_a
来源：http://xb.hahajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ea.bookmarksfly.cn

[B12] 跳出多层循环
来源：http://dk.9csxet.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wm.colortex.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pj.gzmigu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dy.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rz.newstarts.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vy.jctech888.com.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ju.gzmigu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xd.shxzukj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hy.hahajie.cn

[B13] 判断是否为数字
来源：http://pd.szxytkj.cn

Py:   isinstance(x, (int, float))
来源：http://eh.haigaiapp.cn

PHP:  is_numeric($x)
来源：http://iv.szsharing.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bf.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dk.colortex.cn

Java: x instanceof Number
来源：http://rk.huixinmuqiang.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cz.yuexingan06.cn

Ruby: x.is_a?(Numeric)
来源：http://lq.nicolike.cn

C#:   x is int or double or decimal
来源：http://am.huanxung.cn

[B14] 判断值是否在集合内
来源：http://ej.bjjhwx.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sl.huanxung.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jj.bjjhwx.cn

JS:   [1, 2, 3].includes(x)
来源：http://lp.huixiangedu.cn

TS:   [1, 2, 3].includes(x)
来源：http://uv.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ki.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qh.huixinmuqiang.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zv.huixiangedu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qg.shxzskj.cn

[B15] 布尔运算与取反
来源：http://cl.panjiajie.cn

Py:   a and b or not c
来源：http://dx.jianghongdianzi.cn

PHP:  $a && $b || !$c
来源：http://eu.521024.cn

JS:   a && b || !c
来源：http://gm.jctech888.com.cn

TS:   a && b || !c
来源：http://wk.lnxyls.cn

Java: a && b || !c
来源：http://cl.muxihuayi.cn

Go:   a && b || !c
来源：http://ru.muxihuayi.cn

Ruby: a && b || !c
来源：http://th.chemitech.net.cn

C#:   a && b || !c
来源：http://kn.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kh.asd995.cn

Py:   if not data: return
来源：http://nw.shtwfgs.cn

PHP:  if (!$data) { return; }
来源：http://is.shxzukj.cn

JS:   if (!data) return;
来源：http://xu.bjjhwx.cn

TS:   if (!data) return;
来源：http://lp.panjiajie.cn

Java: if (data == null) return;
来源：http://vf.muxihuayi.cn

Go:   if data == nil { return }
来源：http://fk.wgjwhj.cn

Ruby: return if data.nil?
来源：http://af.newstarts.cn

C#:   if (data == null) return;
来源：http://wl.nicolike.cn

================================================================================
来源：http://ef.huixiangedu.cn

C. 函数与作用域
来源：http://nx.gzmigu.cn

================================================================================
来源：http://as.chemitech.net.cn

[C01] 定义函数
来源：http://ng.hnjuh.cn

Py:   def add(a, b): return a + b
来源：http://pf.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ld.shxzukj.cn

JS:   function add(a, b) { return a + b; }
来源：http://la.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fy.jctech888.com.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nt.9csxet.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ha.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://qj.newstarts.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ig.newstarts.cn

[C02] 默认参数
来源：http://hk.yuexingan06.cn

Py:   def greet(name="World"): return name
来源：http://ba.shxzukj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yz.521024.cn

JS:   function greet(name = "World") { return name; }
来源：http://kr.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ya.jctech888.com.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ya.haigaiapp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://iq.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://rp.hahajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://ry.9csxet.cn

[C03] 可变参数
来源：http://pw.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://fk.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ri.newstarts.cn


<!-- 参考信息 -->