代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ow.yuexingan06.cn

Ruby: "Hello, #{name}!"
来源：http://vu.shxzukj.cn

C#:   $"Hello, {name}!"
来源：http://rc.nicolike.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://zy.szxytkj.cn

Py:   "第一行\n第二行"
来源：http://ez.gzmigu.cn

PHP:  "第一行\n第二行"
来源：http://ul.wgjwhj.cn

JS:   "第一行\n第二行"
来源：http://ws.hnjuh.cn

TS:   "第一行\n第二行"
来源：http://lg.wgjwhj.cn

Java: "第一行\n第二行"
来源：http://zp.yuntaijiaju.cn

Go:   "第一行\n第二行"
来源：http://hg.shxzukj.cn

Ruby: "第一行\n第二行"
来源：http://fc.huixiangedu.cn

C#:   "第一行\n第二行"
来源：http://hi.lnxyls.cn

[A14] 注释写法
来源：http://fx.yuntaijiaju.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://xk.muxihuayi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ih.shxzskj.cn

JS:   // 单行；/* 多行 */
来源：http://bx.shtwfgs.cn

TS:   // 单行；/* 多行 */
来源：http://wo.lnxyls.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tr.panjiajie.cn

Go:   // 单行；/* 多行 */
来源：http://to.newstarts.cn

Ruby: # 单行；=begin 多行 =end
来源：http://gz.huixinmuqiang.cn

C#:   // 单行；/* 多行 */
来源：http://eo.hahajie.cn

[A15] 空值判断与默认值
来源：http://ze.jctech888.com.cn

Py:   value = data or "默认值"
来源：http://db.shxzskj.cn

PHP:  $value = $data ?? "默认值";
来源：http://dw.newstarts.cn

JS:   const value = data ?? "默认值";
来源：http://ro.nicolike.cn

TS:   const value = data ?? "默认值";
来源：http://vl.lnxyls.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bo.haigaiapp.cn

Go:   if data == "" { data = "默认值" }
来源：http://gr.szxytkj.cn

Ruby: value = data || "默认值"
来源：http://sv.bjjhwx.cn

C#:   var value = data ?? "默认值";
来源：http://sk.szxytkj.cn

[A16] 真假值判断规则
来源：http://cm.yuntaijiaju.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dn.huanxung.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://kq.shxzskj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dp.panjiajie.cn

TS:   if (!x) {}
来源：http://cu.asd995.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://oy.nszjky.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qa.yuntaijiaju.cn

Ruby: unless x            # nil 与 false 为假
来源：http://pb.szsharing.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://eu.huixinmuqiang.cn

[A17] 位运算
来源：http://cn.chemitech.net.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oj.jctech888.com.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vu.yuexingan06.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ky.9csxet.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nc.shtwfgs.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://te.bjjhwx.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://sz.hahajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ri.shtwfgs.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xx.nicolike.cn

[A18] 字符与 ASCII 码互转
来源：http://kv.huixinmuqiang.cn

Py:   ord("A"); chr(65)
来源：http://im.bookmarksfly.cn

PHP:  ord("A"); chr(65)
来源：http://co.szxytkj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ii.haigaiapp.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ao.huixinmuqiang.cn

Java: (int) 'A'; (char) 65
来源：http://qx.yuexingan06.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dk.szxytkj.cn

Ruby: "A".ord; 65.chr
来源：http://gd.gzmigu.cn

C#:   (int)'A'; (char)65
来源：http://ox.shtwfgs.cn

[A19] 交换两个变量
来源：http://ic.nicolike.cn

Py:   a, b = b, a
来源：http://ne.huanxung.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://wc.shxzskj.cn

JS:   [a, b] = [b, a];
来源：http://gr.huanxung.cn

TS:   [a, b] = [b, a];
来源：http://ve.hnjuh.cn

Java: int t = a; a = b; b = t;
来源：http://rt.nszjky.cn

Go:   a, b = b, a
来源：http://om.haigaiapp.cn

Ruby: a, b = b, a
来源：http://co.szsharing.cn

C#:   (a, b) = (b, a);
来源：http://it.szxytkj.cn

[A20] 读取标准输入
来源：http://aa.nszjky.cn

Py:   name = input("请输入：")
来源：http://gr.9csxet.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://tc.huanxung.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ow.asd995.cn

TS:   // Node.js：readline 模块
来源：http://ep.szsharing.cn

Java: new Scanner(System.in).nextLine()
来源：http://do.shxzukj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zs.chemitech.net.cn

Ruby: gets.chomp
来源：http://tm.gzmigu.cn

C#:   Console.ReadLine();
来源：http://lu.wgjwhj.cn

[A21] 保留指定小数位输出
来源：http://cb.colortex.cn

Py:   f"{3.14159:.2f}"
来源：http://dl.wgjwhj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ic.yuexingan06.cn

JS:   (3.14159).toFixed(2)
来源：http://op.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://cl.szxytkj.cn

Java: String.format("%.2f", 3.14159)
来源：http://hm.szsharing.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ux.bookmarksfly.cn

Ruby: format("%.2f", 3.14159)
来源：http://qe.huixiangedu.cn

C#:   3.14159.ToString("F2")
来源：http://la.colortex.cn

[A22] 获取字符串长度
来源：http://eb.hnjuh.cn

Py:   len(s)
来源：http://qy.jianghongdianzi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wx.jctech888.com.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rm.gzmigu.cn

TS:   s.length
来源：http://mw.wgjwhj.cn

Java: s.length()
来源：http://vq.shtwfgs.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kv.nszjky.cn

Ruby: s.length
来源：http://fp.chemitech.net.cn

C#:   s.Length
来源：http://fv.bjjhwx.cn

[A23] 大小写转换
来源：http://gm.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gb.wgjwhj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fb.yuexingan06.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ak.shxzskj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ph.huixiangedu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bn.haigaiapp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sh.haigaiapp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gy.szxytkj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://yt.jianghongdianzi.cn

[A24] 去除首尾空白
来源：http://bz.chemitech.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://im.nszjky.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cn.newstarts.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uo.szxytkj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xh.szxytkj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://iv.gzmigu.cn

Go:   strings.TrimSpace(s)
来源：http://ut.newstarts.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://my.newstarts.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ne.hnjuh.cn

[A25] 字符串比较
来源：http://ar.hahajie.cn

Py:   s1 == s2; s1 != s2
来源：http://nx.newstarts.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cb.bookmarksfly.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sz.haigaiapp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://oe.jctech888.com.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bz.newstarts.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ot.jianghongdianzi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vs.muxihuayi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dc.521024.cn

[A26] 类型转换总览
来源：http://tk.nszjky.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vf.szsharing.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vp.jctech888.com.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cc.bjjhwx.cn

TS:   Number() String() Boolean() x as number
来源：http://vu.bookmarksfly.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://co.muxihuayi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rm.asd995.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dp.muxihuayi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rf.hahajie.cn

================================================================================
来源：http://yj.huanxung.cn

B. 流程控制
来源：http://mt.panjiajie.cn

================================================================================
来源：http://nr.nszjky.cn

[B01] 条件判断 if / else
来源：http://jk.yuexingan06.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cv.muxihuayi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rp.huixinmuqiang.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gj.9csxet.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ho.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vu.panjiajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kh.huixiangedu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sm.bjjhwx.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://it.yuntaijiaju.cn

[B02] 多分支 else if / elif
来源：http://vt.asd995.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tz.asd995.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qk.yuntaijiaju.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iy.hahajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oi.haigaiapp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eb.newstarts.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ks.lnxyls.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xf.wgjwhj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vr.9csxet.cn

[B03] switch / match / case
来源：http://vt.jctech888.com.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wn.hnjuh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sr.huanxung.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pi.521024.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tn.nicolike.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dt.hahajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uq.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ck.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lp.huanxung.cn

[B04] for 计数循环
来源：http://xp.yuexingan06.cn

Py:   for i in range(10): print(i)
来源：http://fg.hnjuh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ap.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bg.9csxet.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cg.asd995.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vz.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lb.muxihuayi.cn

Ruby: 10.times { |i| puts i }
来源：http://mw.lnxyls.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://im.newstarts.cn

[B05] 遍历数组 / 列表
来源：http://cl.colortex.cn

Py:   for item in arr: print(item)
来源：http://yq.521024.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://di.hnjuh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ec.colortex.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qh.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wu.asd995.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ed.lnxyls.cn

Ruby: arr.each { |item| puts item }
来源：http://dy.bjjhwx.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jk.panjiajie.cn

[B06] 遍历字典 / 对象
来源：http://qu.wgjwhj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hn.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ei.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ft.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tt.szsharing.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ss.yuntaijiaju.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qk.jctech888.com.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qv.newstarts.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ju.shxzskj.cn

[B07] while 循环
来源：http://sx.muxihuayi.cn

Py:   while i < 10: i += 1
来源：http://fq.jianghongdianzi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mi.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://pe.nicolike.cn

TS:   while (i < 10) { i++; }
来源：http://ue.asd995.cn

Java: while (i < 10) { i++; }
来源：http://az.yuntaijiaju.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uz.jianghongdianzi.cn

Ruby: while i < 10; i += 1; end
来源：http://gh.huixiangedu.cn

C#:   while (i < 10) { i++; }
来源：http://wu.bookmarksfly.cn

[B08] do-while（至少执行一次）
来源：http://fe.jctech888.com.cn

Py:   # 无 do-while：用 while True + break
来源：http://fv.szsharing.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qj.huanxung.cn

JS:   do { i++; } while (i < 10);
来源：http://tt.hahajie.cn

TS:   do { i++; } while (i < 10);
来源：http://my.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://wk.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wp.szxytkj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rz.huanxung.cn

C#:   do { i++; } while (i < 10);
来源：http://wl.szxytkj.cn

[B09] break 与 continue
来源：http://qc.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ws.gzmigu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ya.9csxet.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ix.colortex.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rz.wgjwhj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sq.bookmarksfly.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rs.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kk.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gp.hahajie.cn

[B10] 遍历同时拿索引
来源：http://xr.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ea.panjiajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oi.szsharing.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gf.szsharing.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lp.wgjwhj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zx.nicolike.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://an.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pk.lnxyls.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vf.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://ef.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://zj.wgjwhj.cn

PHP:  range(0, 10, 2);
来源：http://dt.colortex.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kj.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wt.gzmigu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pw.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kn.bookmarksfly.cn

Ruby: (0...10).step(2).to_a
来源：http://xx.yuntaijiaju.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ct.chemitech.net.cn

[B12] 跳出多层循环
来源：http://em.huixiangedu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://oi.nszjky.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hj.nicolike.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ex.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ka.szsharing.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yt.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qi.muxihuayi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fm.hahajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pg.huanxung.cn

[B13] 判断是否为数字
来源：http://tq.huixinmuqiang.cn

Py:   isinstance(x, (int, float))
来源：http://sn.haigaiapp.cn

PHP:  is_numeric($x)
来源：http://qc.jctech888.com.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xl.huanxung.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gt.haigaiapp.cn

Java: x instanceof Number
来源：http://sn.huanxung.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://aq.szsharing.cn

Ruby: x.is_a?(Numeric)
来源：http://pn.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://qs.panjiajie.cn

[B14] 判断值是否在集合内
来源：http://ru.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nz.yuntaijiaju.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kl.newstarts.cn

JS:   [1, 2, 3].includes(x)
来源：http://zi.hahajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://va.hnjuh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ni.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hy.shtwfgs.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yo.colortex.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fp.hnjuh.cn

[B15] 布尔运算与取反
来源：http://jv.szsharing.cn

Py:   a and b or not c
来源：http://mh.szsharing.cn

PHP:  $a && $b || !$c
来源：http://ez.shxzukj.cn

JS:   a && b || !c
来源：http://go.jctech888.com.cn

TS:   a && b || !c
来源：http://dx.nicolike.cn

Java: a && b || !c
来源：http://lx.bookmarksfly.cn

Go:   a && b || !c
来源：http://df.shxzskj.cn

Ruby: a && b || !c
来源：http://sg.wgjwhj.cn

C#:   a && b || !c
来源：http://zs.521024.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ib.shxzukj.cn

Py:   if not data: return
来源：http://cy.haigaiapp.cn

PHP:  if (!$data) { return; }
来源：http://ch.nicolike.cn

JS:   if (!data) return;
来源：http://zi.chemitech.net.cn

TS:   if (!data) return;
来源：http://lr.hnjuh.cn

Java: if (data == null) return;
来源：http://eh.panjiajie.cn

Go:   if data == nil { return }
来源：http://kp.bjjhwx.cn

Ruby: return if data.nil?
来源：http://og.panjiajie.cn

C#:   if (data == null) return;
来源：http://pr.9csxet.cn

================================================================================
来源：http://wl.9csxet.cn

C. 函数与作用域
来源：http://tq.bookmarksfly.cn

================================================================================
来源：http://gd.lnxyls.cn

[C01] 定义函数
来源：http://mt.shxzskj.cn

Py:   def add(a, b): return a + b
来源：http://ft.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bx.asd995.cn

JS:   function add(a, b) { return a + b; }
来源：http://vy.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rw.colortex.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gf.521024.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ja.asd995.cn

Ruby: def add(a, b); a + b; end
来源：http://bj.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pg.wgjwhj.cn

[C02] 默认参数
来源：http://aj.521024.cn

Py:   def greet(name="World"): return name
来源：http://ct.yuntaijiaju.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tx.yuexingan06.cn

JS:   function greet(name = "World") { return name; }
来源：http://pj.521024.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://uc.huixinmuqiang.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hd.wgjwhj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://km.hnjuh.cn

Ruby: def greet(name = "World") = name
来源：http://ok.shxzukj.cn

C#:   string Greet(string name = "World") => name;
来源：http://aj.hahajie.cn

[C03] 可变参数
来源：http://ut.nicolike.cn

Py:   def total(*args): return sum(args)
来源：http://xe.huanxung.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ks.szxytkj.cn


<!-- 参考信息 -->