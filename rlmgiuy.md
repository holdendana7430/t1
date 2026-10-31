代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nl.panjiajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kr.huixiangedu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ot.gzmigu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zl.panjiajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ao.hahajie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tl.szxytkj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rk.huixinmuqiang.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mk.hahajie.cn

[A10] 生成随机数
来源：http://wo.asd995.cn

Py:   import random; random.randint(1, 100)
来源：http://dg.newstarts.cn

PHP:  random_int(1, 100);
来源：http://hu.colortex.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://um.nszjky.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qn.colortex.cn

Java: new Random().nextInt(100) + 1
来源：http://qm.bjjhwx.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tk.jctech888.com.cn

Ruby: rand(1..100)
来源：http://tr.nicolike.cn

C#:   new Random().Next(1, 101)
来源：http://cf.wgjwhj.cn

[A11] 条件表达式（三元）
来源：http://sz.szsharing.cn

Py:   "yes" if x > 0 else "no"
来源：http://fv.521024.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://en.wgjwhj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://my.huanxung.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ea.bjjhwx.cn

Java: x > 0 ? "yes" : "no"
来源：http://sw.newstarts.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://uy.haigaiapp.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://gi.nicolike.cn

C#:   x > 0 ? "yes" : "no"
来源：http://yy.muxihuayi.cn

[A12] 字符串插值 / 格式化
来源：http://hx.bjjhwx.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ad.wgjwhj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pe.bjjhwx.cn

JS:   `Hello, ${name}!`
来源：http://vt.bjjhwx.cn

TS:   `Hello, ${name}!`
来源：http://go.colortex.cn

Java: "Hello, %s!".formatted(name)
来源：http://tz.hnjuh.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tv.panjiajie.cn

Ruby: "Hello, #{name}!"
来源：http://ze.yuntaijiaju.cn

C#:   $"Hello, {name}!"
来源：http://ry.hnjuh.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hq.521024.cn

Py:   "第一行\n第二行"
来源：http://vt.shxzskj.cn

PHP:  "第一行\n第二行"
来源：http://hy.nszjky.cn

JS:   "第一行\n第二行"
来源：http://tw.wgjwhj.cn

TS:   "第一行\n第二行"
来源：http://xi.huixinmuqiang.cn

Java: "第一行\n第二行"
来源：http://qm.huanxung.cn

Go:   "第一行\n第二行"
来源：http://jq.gzmigu.cn

Ruby: "第一行\n第二行"
来源：http://nz.nicolike.cn

C#:   "第一行\n第二行"
来源：http://vw.szsharing.cn

[A14] 注释写法
来源：http://gc.shxzukj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://cj.bookmarksfly.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hu.bjjhwx.cn

JS:   // 单行；/* 多行 */
来源：http://sb.bjjhwx.cn

TS:   // 单行；/* 多行 */
来源：http://lf.huixinmuqiang.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://az.521024.cn

Go:   // 单行；/* 多行 */
来源：http://gy.panjiajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qn.yuntaijiaju.cn

C#:   // 单行；/* 多行 */
来源：http://uj.huixiangedu.cn

[A15] 空值判断与默认值
来源：http://sg.szxytkj.cn

Py:   value = data or "默认值"
来源：http://va.asd995.cn

PHP:  $value = $data ?? "默认值";
来源：http://su.9csxet.cn

JS:   const value = data ?? "默认值";
来源：http://pe.yuntaijiaju.cn

TS:   const value = data ?? "默认值";
来源：http://ut.colortex.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ol.colortex.cn

Go:   if data == "" { data = "默认值" }
来源：http://cb.bookmarksfly.cn

Ruby: value = data || "默认值"
来源：http://ph.nicolike.cn

C#:   var value = data ?? "默认值";
来源：http://dt.panjiajie.cn

[A16] 真假值判断规则
来源：http://zg.muxihuayi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xt.panjiajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://te.szxytkj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pf.shtwfgs.cn

TS:   if (!x) {}
来源：http://gh.9csxet.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ym.huanxung.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wt.bjjhwx.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ex.lnxyls.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pb.hahajie.cn

[A17] 位运算
来源：http://yj.shxzukj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cx.huanxung.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ic.szxytkj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://im.9csxet.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ez.colortex.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hr.szxytkj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://uo.huanxung.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jq.jianghongdianzi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hh.shtwfgs.cn

[A18] 字符与 ASCII 码互转
来源：http://vl.szxytkj.cn

Py:   ord("A"); chr(65)
来源：http://xq.haigaiapp.cn

PHP:  ord("A"); chr(65)
来源：http://re.yuexingan06.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ft.muxihuayi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jz.bookmarksfly.cn

Java: (int) 'A'; (char) 65
来源：http://bh.colortex.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ma.yuntaijiaju.cn

Ruby: "A".ord; 65.chr
来源：http://jj.lnxyls.cn

C#:   (int)'A'; (char)65
来源：http://np.hnjuh.cn

[A19] 交换两个变量
来源：http://ji.hnjuh.cn

Py:   a, b = b, a
来源：http://re.wgjwhj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://bm.yuntaijiaju.cn

JS:   [a, b] = [b, a];
来源：http://hs.szsharing.cn

TS:   [a, b] = [b, a];
来源：http://bl.hnjuh.cn

Java: int t = a; a = b; b = t;
来源：http://ms.asd995.cn

Go:   a, b = b, a
来源：http://le.521024.cn

Ruby: a, b = b, a
来源：http://zi.nicolike.cn

C#:   (a, b) = (b, a);
来源：http://fu.wgjwhj.cn

[A20] 读取标准输入
来源：http://gc.jianghongdianzi.cn

Py:   name = input("请输入：")
来源：http://ge.bookmarksfly.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://jb.haigaiapp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mn.bjjhwx.cn

TS:   // Node.js：readline 模块
来源：http://pq.521024.cn

Java: new Scanner(System.in).nextLine()
来源：http://ze.gzmigu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sw.yuexingan06.cn

Ruby: gets.chomp
来源：http://hf.colortex.cn

C#:   Console.ReadLine();
来源：http://vd.9csxet.cn

[A21] 保留指定小数位输出
来源：http://ej.newstarts.cn

Py:   f"{3.14159:.2f}"
来源：http://yc.panjiajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://uf.hnjuh.cn

JS:   (3.14159).toFixed(2)
来源：http://ko.hahajie.cn

TS:   (3.14159).toFixed(2)
来源：http://if.bjjhwx.cn

Java: String.format("%.2f", 3.14159)
来源：http://pq.shtwfgs.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xo.yuexingan06.cn

Ruby: format("%.2f", 3.14159)
来源：http://is.jianghongdianzi.cn

C#:   3.14159.ToString("F2")
来源：http://vb.shxzskj.cn

[A22] 获取字符串长度
来源：http://lx.muxihuayi.cn

Py:   len(s)
来源：http://ue.yuntaijiaju.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ih.haigaiapp.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rb.shxzskj.cn

TS:   s.length
来源：http://kb.shxzskj.cn

Java: s.length()
来源：http://mp.szsharing.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mo.huanxung.cn

Ruby: s.length
来源：http://xj.lnxyls.cn

C#:   s.Length
来源：http://th.huixinmuqiang.cn

[A23] 大小写转换
来源：http://jy.shxzukj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ak.shtwfgs.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lh.shxzukj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wm.szsharing.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pe.newstarts.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sl.bjjhwx.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xi.shxzukj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jg.jianghongdianzi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://sx.yuexingan06.cn

[A24] 去除首尾空白
来源：http://xi.huixinmuqiang.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kj.szxytkj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xd.colortex.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wu.newstarts.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qw.gzmigu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.panjiajie.cn

Go:   strings.TrimSpace(s)
来源：http://st.9csxet.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nm.bjjhwx.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yr.chemitech.net.cn

[A25] 字符串比较
来源：http://jm.bjjhwx.cn

Py:   s1 == s2; s1 != s2
来源：http://sn.bjjhwx.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hh.lnxyls.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fc.shxzukj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bv.9csxet.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://or.wgjwhj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mw.chemitech.net.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://si.jianghongdianzi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pp.yuntaijiaju.cn

[A26] 类型转换总览
来源：http://zg.colortex.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ci.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://md.szsharing.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rv.yuexingan06.cn

TS:   Number() String() Boolean() x as number
来源：http://kf.newstarts.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wq.jianghongdianzi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zn.yuntaijiaju.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rx.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mw.hahajie.cn

================================================================================
来源：http://co.yuexingan06.cn

B. 流程控制
来源：http://el.hahajie.cn

================================================================================
来源：http://va.szsharing.cn

[B01] 条件判断 if / else
来源：http://in.shxzukj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xd.huixiangedu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fx.jctech888.com.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wk.shxzukj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oc.wgjwhj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pk.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gn.yuntaijiaju.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jz.nszjky.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ae.hnjuh.cn

[B02] 多分支 else if / elif
来源：http://yj.szxytkj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ei.shxzskj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rk.9csxet.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://at.szsharing.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ap.jianghongdianzi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pz.huanxung.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://op.muxihuayi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wr.asd995.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://if.muxihuayi.cn

[B03] switch / match / case
来源：http://dj.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://we.yuntaijiaju.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tm.nicolike.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xc.asd995.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hr.yuntaijiaju.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wy.shtwfgs.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xw.shxzskj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qq.huanxung.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ih.nszjky.cn

[B04] for 计数循环
来源：http://rr.lnxyls.cn

Py:   for i in range(10): print(i)
来源：http://wi.bookmarksfly.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://is.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://el.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zd.newstarts.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sk.shtwfgs.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bm.szsharing.cn

Ruby: 10.times { |i| puts i }
来源：http://vk.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bl.panjiajie.cn

[B05] 遍历数组 / 列表
来源：http://xz.shxzskj.cn

Py:   for item in arr: print(item)
来源：http://se.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://un.521024.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dq.jianghongdianzi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ba.521024.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sx.lnxyls.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vl.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://qi.jctech888.com.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uo.lnxyls.cn

[B06] 遍历字典 / 对象
来源：http://hl.bookmarksfly.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fu.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mv.asd995.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xm.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vz.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://en.muxihuayi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tn.gzmigu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ae.asd995.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://st.bjjhwx.cn

[B07] while 循环
来源：http://ig.szsharing.cn

Py:   while i < 10: i += 1
来源：http://it.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xh.colortex.cn

JS:   while (i < 10) { i++; }
来源：http://tq.szxytkj.cn

TS:   while (i < 10) { i++; }
来源：http://ns.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://dk.hahajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://na.chemitech.net.cn

Ruby: while i < 10; i += 1; end
来源：http://ph.muxihuayi.cn

C#:   while (i < 10) { i++; }
来源：http://uv.yuexingan06.cn

[B08] do-while（至少执行一次）
来源：http://pk.nicolike.cn

Py:   # 无 do-while：用 while True + break
来源：http://ta.bjjhwx.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://no.muxihuayi.cn

JS:   do { i++; } while (i < 10);
来源：http://sv.bjjhwx.cn

TS:   do { i++; } while (i < 10);
来源：http://kz.jctech888.com.cn

Java: do { i++; } while (i < 10);
来源：http://tq.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pw.newstarts.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nq.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://la.huixiangedu.cn

[B09] break 与 continue
来源：http://sf.521024.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bf.wgjwhj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kv.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://af.muxihuayi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vx.gzmigu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ev.shxzukj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wh.bjjhwx.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sr.chemitech.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ai.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://gn.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ia.huixiangedu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zh.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qf.muxihuayi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oy.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zk.asd995.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lk.bjjhwx.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tp.huanxung.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tn.yuntaijiaju.cn

[B11] 生成数字序列 / 区间
来源：http://ce.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://th.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://jm.colortex.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jw.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ao.muxihuayi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ps.szxytkj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uy.newstarts.cn

Ruby: (0...10).step(2).to_a
来源：http://pb.szxytkj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://it.lnxyls.cn

[B12] 跳出多层循环
来源：http://dj.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tv.jctech888.com.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kk.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rn.yuntaijiaju.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://il.szxytkj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jl.wgjwhj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wl.shtwfgs.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sw.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qw.bjjhwx.cn

[B13] 判断是否为数字
来源：http://vt.huixiangedu.cn

Py:   isinstance(x, (int, float))
来源：http://wa.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://jg.nicolike.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://un.bjjhwx.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hm.shxzukj.cn

Java: x instanceof Number
来源：http://qk.huixiangedu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rm.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://bx.wgjwhj.cn

C#:   x is int or double or decimal
来源：http://ek.shxzskj.cn

[B14] 判断值是否在集合内
来源：http://ln.bjjhwx.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kz.huixinmuqiang.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://du.521024.cn

JS:   [1, 2, 3].includes(x)
来源：http://xp.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://cp.shxzskj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sg.yuexingan06.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zm.nicolike.cn

Ruby: [1, 2, 3].include?(x)
来源：http://el.hahajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yq.bookmarksfly.cn

[B15] 布尔运算与取反
来源：http://yl.bjjhwx.cn

Py:   a and b or not c
来源：http://em.huixinmuqiang.cn

PHP:  $a && $b || !$c
来源：http://ss.yuntaijiaju.cn

JS:   a && b || !c
来源：http://we.panjiajie.cn

TS:   a && b || !c
来源：http://bx.gzmigu.cn

Java: a && b || !c
来源：http://ta.hnjuh.cn

Go:   a && b || !c
来源：http://ow.hahajie.cn

Ruby: a && b || !c
来源：http://fv.9csxet.cn

C#:   a && b || !c
来源：http://gh.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ug.hahajie.cn


<!-- 参考信息 -->