代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ji.nszjky.cn

JS:   `Hello, ${name}!`
来源：http://cf.wgjwhj.cn

TS:   `Hello, ${name}!`
来源：http://in.9csxet.cn

Java: "Hello, %s!".formatted(name)
来源：http://lf.gzmigu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yy.nicolike.cn

Ruby: "Hello, #{name}!"
来源：http://lb.newstarts.cn

C#:   $"Hello, {name}!"
来源：http://ej.huixinmuqiang.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://xa.jctech888.com.cn

Py:   "第一行\n第二行"
来源：http://ug.bookmarksfly.cn

PHP:  "第一行\n第二行"
来源：http://tt.yuexingan06.cn

JS:   "第一行\n第二行"
来源：http://ic.wgjwhj.cn

TS:   "第一行\n第二行"
来源：http://yy.nszjky.cn

Java: "第一行\n第二行"
来源：http://hi.huixiangedu.cn

Go:   "第一行\n第二行"
来源：http://zk.9csxet.cn

Ruby: "第一行\n第二行"
来源：http://ow.lnxyls.cn

C#:   "第一行\n第二行"
来源：http://zi.colortex.cn

[A14] 注释写法
来源：http://ak.bjjhwx.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://mb.521024.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://yb.hahajie.cn

JS:   // 单行；/* 多行 */
来源：http://og.asd995.cn

TS:   // 单行；/* 多行 */
来源：http://vk.hahajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ez.colortex.cn

Go:   // 单行；/* 多行 */
来源：http://qg.bookmarksfly.cn

Ruby: # 单行；=begin 多行 =end
来源：http://nb.gzmigu.cn

C#:   // 单行；/* 多行 */
来源：http://ud.jctech888.com.cn

[A15] 空值判断与默认值
来源：http://di.shxzskj.cn

Py:   value = data or "默认值"
来源：http://lq.shtwfgs.cn

PHP:  $value = $data ?? "默认值";
来源：http://ew.gzmigu.cn

JS:   const value = data ?? "默认值";
来源：http://yl.nszjky.cn

TS:   const value = data ?? "默认值";
来源：http://bh.nszjky.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vs.huanxung.cn

Go:   if data == "" { data = "默认值" }
来源：http://gd.huixinmuqiang.cn

Ruby: value = data || "默认值"
来源：http://bj.wgjwhj.cn

C#:   var value = data ?? "默认值";
来源：http://jk.haigaiapp.cn

[A16] 真假值判断规则
来源：http://ij.huixinmuqiang.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://us.shtwfgs.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vu.huanxung.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://de.521024.cn

TS:   if (!x) {}
来源：http://hf.huixinmuqiang.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://oc.szxytkj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ui.huixiangedu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://kx.9csxet.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://en.haigaiapp.cn

[A17] 位运算
来源：http://nb.hahajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yl.yuexingan06.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vm.huixiangedu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lm.hnjuh.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uj.shxzskj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vb.bjjhwx.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ev.nszjky.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xq.shxzskj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pk.szsharing.cn

[A18] 字符与 ASCII 码互转
来源：http://lx.yuntaijiaju.cn

Py:   ord("A"); chr(65)
来源：http://zq.nszjky.cn

PHP:  ord("A"); chr(65)
来源：http://ql.nszjky.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fi.asd995.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://so.muxihuayi.cn

Java: (int) 'A'; (char) 65
来源：http://ni.colortex.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dw.jctech888.com.cn

Ruby: "A".ord; 65.chr
来源：http://vz.newstarts.cn

C#:   (int)'A'; (char)65
来源：http://oh.huixiangedu.cn

[A19] 交换两个变量
来源：http://or.muxihuayi.cn

Py:   a, b = b, a
来源：http://we.colortex.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ft.bjjhwx.cn

JS:   [a, b] = [b, a];
来源：http://al.huanxung.cn

TS:   [a, b] = [b, a];
来源：http://ha.huixinmuqiang.cn

Java: int t = a; a = b; b = t;
来源：http://yc.521024.cn

Go:   a, b = b, a
来源：http://iu.colortex.cn

Ruby: a, b = b, a
来源：http://pt.nszjky.cn

C#:   (a, b) = (b, a);
来源：http://pn.lnxyls.cn

[A20] 读取标准输入
来源：http://po.nszjky.cn

Py:   name = input("请输入：")
来源：http://rt.yuexingan06.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://iw.asd995.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://li.colortex.cn

TS:   // Node.js：readline 模块
来源：http://jl.panjiajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://pl.nicolike.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ba.shxzskj.cn

Ruby: gets.chomp
来源：http://aq.hahajie.cn

C#:   Console.ReadLine();
来源：http://rt.hahajie.cn

[A21] 保留指定小数位输出
来源：http://nx.yuntaijiaju.cn

Py:   f"{3.14159:.2f}"
来源：http://lv.szsharing.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vn.9csxet.cn

JS:   (3.14159).toFixed(2)
来源：http://we.521024.cn

TS:   (3.14159).toFixed(2)
来源：http://lk.huixiangedu.cn

Java: String.format("%.2f", 3.14159)
来源：http://ze.521024.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ix.nicolike.cn

Ruby: format("%.2f", 3.14159)
来源：http://pv.521024.cn

C#:   3.14159.ToString("F2")
来源：http://zt.hahajie.cn

[A22] 获取字符串长度
来源：http://iy.bjjhwx.cn

Py:   len(s)
来源：http://eq.gzmigu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fb.shxzskj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ny.haigaiapp.cn

TS:   s.length
来源：http://xw.panjiajie.cn

Java: s.length()
来源：http://fi.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kv.colortex.cn

Ruby: s.length
来源：http://ju.huixiangedu.cn

C#:   s.Length
来源：http://io.huixiangedu.cn

[A23] 大小写转换
来源：http://ww.yuntaijiaju.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qe.521024.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://we.huixinmuqiang.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ic.gzmigu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ym.9csxet.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ah.shtwfgs.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qx.hnjuh.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gy.colortex.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fp.hnjuh.cn

[A24] 去除首尾空白
来源：http://vu.huanxung.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wt.panjiajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ex.521024.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://js.hnjuh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tc.muxihuayi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qn.lnxyls.cn

Go:   strings.TrimSpace(s)
来源：http://yx.nicolike.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tl.yuntaijiaju.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nz.haigaiapp.cn

[A25] 字符串比较
来源：http://hz.bjjhwx.cn

Py:   s1 == s2; s1 != s2
来源：http://ml.nszjky.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qm.nicolike.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qj.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nx.panjiajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cd.muxihuayi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xp.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zm.521024.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://me.jianghongdianzi.cn

[A26] 类型转换总览
来源：http://jy.huanxung.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mj.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://by.shxzskj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cz.chemitech.net.cn

TS:   Number() String() Boolean() x as number
来源：http://pn.huixiangedu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vt.huixinmuqiang.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ao.521024.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jf.wgjwhj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nd.bjjhwx.cn

================================================================================
来源：http://hl.lnxyls.cn

B. 流程控制
来源：http://gu.szsharing.cn

================================================================================
来源：http://oy.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://ch.jianghongdianzi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ff.szsharing.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://aq.bookmarksfly.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xc.huixinmuqiang.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ou.szxytkj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ua.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://li.haigaiapp.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ie.nszjky.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xb.szsharing.cn

[B02] 多分支 else if / elif
来源：http://wq.szsharing.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fm.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ou.jctech888.com.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rv.yuntaijiaju.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://er.jctech888.com.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xd.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ta.gzmigu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://az.bjjhwx.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xb.bookmarksfly.cn

[B03] switch / match / case
来源：http://fp.panjiajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jo.521024.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nu.gzmigu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dx.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mj.yuexingan06.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pv.szxytkj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dy.jctech888.com.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lg.wgjwhj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mp.bookmarksfly.cn

[B04] for 计数循环
来源：http://gl.bookmarksfly.cn

Py:   for i in range(10): print(i)
来源：http://qg.szxytkj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://om.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dd.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sy.521024.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oo.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lo.muxihuayi.cn

Ruby: 10.times { |i| puts i }
来源：http://fp.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rz.haigaiapp.cn

[B05] 遍历数组 / 列表
来源：http://yl.chemitech.net.cn

Py:   for item in arr: print(item)
来源：http://gw.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ps.newstarts.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yk.panjiajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zm.9csxet.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pc.lnxyls.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cy.shxzskj.cn

Ruby: arr.each { |item| puts item }
来源：http://nk.haigaiapp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rv.bjjhwx.cn

[B06] 遍历字典 / 对象
来源：http://be.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dn.521024.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cm.huixinmuqiang.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ph.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xz.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qq.shtwfgs.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zp.szxytkj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ef.hahajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ku.huanxung.cn

[B07] while 循环
来源：http://nk.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://se.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wu.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://rk.muxihuayi.cn

TS:   while (i < 10) { i++; }
来源：http://qy.jctech888.com.cn

Java: while (i < 10) { i++; }
来源：http://zz.521024.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mo.szsharing.cn

Ruby: while i < 10; i += 1; end
来源：http://fb.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://nu.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://hb.shxzukj.cn

Py:   # 无 do-while：用 while True + break
来源：http://fb.wgjwhj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://lu.asd995.cn

JS:   do { i++; } while (i < 10);
来源：http://ee.szsharing.cn

TS:   do { i++; } while (i < 10);
来源：http://kz.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://ot.haigaiapp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://de.yuntaijiaju.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jl.huanxung.cn

C#:   do { i++; } while (i < 10);
来源：http://wb.yuntaijiaju.cn

[B09] break 与 continue
来源：http://ac.jctech888.com.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uc.hnjuh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hx.chemitech.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iy.haigaiapp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ge.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mf.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bc.9csxet.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xs.szsharing.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jc.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://ze.chemitech.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qd.hahajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zr.newstarts.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dl.shxzskj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ow.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ei.bookmarksfly.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ks.chemitech.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tt.colortex.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yu.jianghongdianzi.cn

[B11] 生成数字序列 / 区间
来源：http://sy.nicolike.cn

Py:   list(range(0, 10, 2))
来源：http://uq.bookmarksfly.cn

PHP:  range(0, 10, 2);
来源：http://mk.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bc.9csxet.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dr.nszjky.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ns.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ms.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://sk.9csxet.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://el.bookmarksfly.cn

[B12] 跳出多层循环
来源：http://wv.newstarts.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fk.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fb.wgjwhj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fa.panjiajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://in.shxzukj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ws.nicolike.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zj.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zd.yuntaijiaju.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kv.521024.cn

[B13] 判断是否为数字
来源：http://hr.colortex.cn

Py:   isinstance(x, (int, float))
来源：http://un.shtwfgs.cn

PHP:  is_numeric($x)
来源：http://er.nicolike.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tr.hahajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://so.huanxung.cn

Java: x instanceof Number
来源：http://mg.muxihuayi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vw.bookmarksfly.cn

Ruby: x.is_a?(Numeric)
来源：http://ws.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://vh.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://vp.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ic.521024.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kt.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://pw.szxytkj.cn

TS:   [1, 2, 3].includes(x)
来源：http://gg.shxzukj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rb.shxzukj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nn.yuexingan06.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xv.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bf.yuexingan06.cn

[B15] 布尔运算与取反
来源：http://pr.yuexingan06.cn

Py:   a and b or not c
来源：http://pc.chemitech.net.cn

PHP:  $a && $b || !$c
来源：http://hm.yuntaijiaju.cn

JS:   a && b || !c
来源：http://js.nszjky.cn

TS:   a && b || !c
来源：http://pe.asd995.cn

Java: a && b || !c
来源：http://nu.shxzskj.cn

Go:   a && b || !c
来源：http://xz.yuexingan06.cn

Ruby: a && b || !c
来源：http://ay.huixinmuqiang.cn

C#:   a && b || !c
来源：http://rw.szxytkj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gc.hahajie.cn

Py:   if not data: return
来源：http://qk.chemitech.net.cn

PHP:  if (!$data) { return; }
来源：http://ux.nszjky.cn

JS:   if (!data) return;
来源：http://sq.panjiajie.cn

TS:   if (!data) return;
来源：http://kl.yuexingan06.cn

Java: if (data == null) return;
来源：http://xk.hahajie.cn

Go:   if data == nil { return }
来源：http://rf.chemitech.net.cn

Ruby: return if data.nil?
来源：http://ld.hahajie.cn

C#:   if (data == null) return;
来源：http://nh.shxzukj.cn

================================================================================
来源：http://ti.jianghongdianzi.cn

C. 函数与作用域
来源：http://oe.szsharing.cn

================================================================================
来源：http://it.521024.cn

[C01] 定义函数
来源：http://vv.newstarts.cn

Py:   def add(a, b): return a + b
来源：http://zp.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ls.jctech888.com.cn

JS:   function add(a, b) { return a + b; }
来源：http://ka.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kt.yuntaijiaju.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://as.huixiangedu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zw.shtwfgs.cn

Ruby: def add(a, b); a + b; end
来源：http://sj.jianghongdianzi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ig.lnxyls.cn

[C02] 默认参数
来源：http://cm.yuntaijiaju.cn

Py:   def greet(name="World"): return name
来源：http://mq.521024.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rx.lnxyls.cn

JS:   function greet(name = "World") { return name; }
来源：http://pn.nszjky.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xm.shxzukj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kk.asd995.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zv.521024.cn

Ruby: def greet(name = "World") = name
来源：http://wu.huixiangedu.cn


<!-- 参考信息 -->