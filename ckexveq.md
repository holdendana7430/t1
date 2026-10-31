代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lm.chemitech.net.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ze.szxytkj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ol.nszjky.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://am.lnxyls.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ul.bookmarksfly.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xf.gzmigu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mt.jctech888.com.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://uf.bjjhwx.cn

[A10] 生成随机数
来源：http://rr.asd995.cn

Py:   import random; random.randint(1, 100)
来源：http://vv.yuexingan06.cn

PHP:  random_int(1, 100);
来源：http://mj.bookmarksfly.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://tq.jctech888.com.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wn.nszjky.cn

Java: new Random().nextInt(100) + 1
来源：http://uf.asd995.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vo.nicolike.cn

Ruby: rand(1..100)
来源：http://td.haigaiapp.cn

C#:   new Random().Next(1, 101)
来源：http://po.jctech888.com.cn

[A11] 条件表达式（三元）
来源：http://hb.gzmigu.cn

Py:   "yes" if x > 0 else "no"
来源：http://lc.wgjwhj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://zh.newstarts.cn

JS:   x > 0 ? "yes" : "no"
来源：http://jo.nicolike.cn

TS:   x > 0 ? "yes" : "no"
来源：http://nn.muxihuayi.cn

Java: x > 0 ? "yes" : "no"
来源：http://rx.chemitech.net.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ju.szxytkj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://hw.shtwfgs.cn

C#:   x > 0 ? "yes" : "no"
来源：http://wk.panjiajie.cn

[A12] 字符串插值 / 格式化
来源：http://ir.bookmarksfly.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gq.newstarts.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://en.szxytkj.cn

JS:   `Hello, ${name}!`
来源：http://qt.colortex.cn

TS:   `Hello, ${name}!`
来源：http://rv.huanxung.cn

Java: "Hello, %s!".formatted(name)
来源：http://mt.jctech888.com.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dp.panjiajie.cn

Ruby: "Hello, #{name}!"
来源：http://xn.hnjuh.cn

C#:   $"Hello, {name}!"
来源：http://sb.huanxung.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://gk.wgjwhj.cn

Py:   "第一行\n第二行"
来源：http://mn.haigaiapp.cn

PHP:  "第一行\n第二行"
来源：http://wb.shxzskj.cn

JS:   "第一行\n第二行"
来源：http://vf.bjjhwx.cn

TS:   "第一行\n第二行"
来源：http://ps.hnjuh.cn

Java: "第一行\n第二行"
来源：http://ml.shxzskj.cn

Go:   "第一行\n第二行"
来源：http://en.asd995.cn

Ruby: "第一行\n第二行"
来源：http://bq.huixinmuqiang.cn

C#:   "第一行\n第二行"
来源：http://lc.huanxung.cn

[A14] 注释写法
来源：http://np.szxytkj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gh.nicolike.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://cs.yuntaijiaju.cn

JS:   // 单行；/* 多行 */
来源：http://oa.colortex.cn

TS:   // 单行；/* 多行 */
来源：http://lx.wgjwhj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://oa.szsharing.cn

Go:   // 单行；/* 多行 */
来源：http://pc.gzmigu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xk.huanxung.cn

C#:   // 单行；/* 多行 */
来源：http://bb.panjiajie.cn

[A15] 空值判断与默认值
来源：http://wt.shxzukj.cn

Py:   value = data or "默认值"
来源：http://qr.muxihuayi.cn

PHP:  $value = $data ?? "默认值";
来源：http://ad.yuntaijiaju.cn

JS:   const value = data ?? "默认值";
来源：http://yx.bookmarksfly.cn

TS:   const value = data ?? "默认值";
来源：http://lt.hahajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yt.bookmarksfly.cn

Go:   if data == "" { data = "默认值" }
来源：http://bw.jianghongdianzi.cn

Ruby: value = data || "默认值"
来源：http://js.colortex.cn

C#:   var value = data ?? "默认值";
来源：http://el.gzmigu.cn

[A16] 真假值判断规则
来源：http://nb.nicolike.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dp.muxihuayi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qp.bookmarksfly.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://po.lnxyls.cn

TS:   if (!x) {}
来源：http://do.muxihuayi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nd.jctech888.com.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rw.nszjky.cn

Ruby: unless x            # nil 与 false 为假
来源：http://pl.szsharing.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://oy.yuntaijiaju.cn

[A17] 位运算
来源：http://vv.szsharing.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dv.nicolike.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jr.gzmigu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tf.jctech888.com.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://sb.nicolike.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xo.bookmarksfly.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fq.hnjuh.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yr.bjjhwx.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rx.chemitech.net.cn

[A18] 字符与 ASCII 码互转
来源：http://ox.szsharing.cn

Py:   ord("A"); chr(65)
来源：http://xo.szxytkj.cn

PHP:  ord("A"); chr(65)
来源：http://si.9csxet.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vj.9csxet.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://an.asd995.cn

Java: (int) 'A'; (char) 65
来源：http://en.hahajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://si.colortex.cn

Ruby: "A".ord; 65.chr
来源：http://fv.bjjhwx.cn

C#:   (int)'A'; (char)65
来源：http://fg.jctech888.com.cn

[A19] 交换两个变量
来源：http://im.nicolike.cn

Py:   a, b = b, a
来源：http://xd.jctech888.com.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://xe.bjjhwx.cn

JS:   [a, b] = [b, a];
来源：http://fj.asd995.cn

TS:   [a, b] = [b, a];
来源：http://xe.huanxung.cn

Java: int t = a; a = b; b = t;
来源：http://br.muxihuayi.cn

Go:   a, b = b, a
来源：http://ju.panjiajie.cn

Ruby: a, b = b, a
来源：http://fv.haigaiapp.cn

C#:   (a, b) = (b, a);
来源：http://su.panjiajie.cn

[A20] 读取标准输入
来源：http://cb.muxihuayi.cn

Py:   name = input("请输入：")
来源：http://te.szsharing.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gi.yuntaijiaju.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hc.shxzskj.cn

TS:   // Node.js：readline 模块
来源：http://hi.shtwfgs.cn

Java: new Scanner(System.in).nextLine()
来源：http://fu.colortex.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fe.yuexingan06.cn

Ruby: gets.chomp
来源：http://fu.hahajie.cn

C#:   Console.ReadLine();
来源：http://fx.9csxet.cn

[A21] 保留指定小数位输出
来源：http://sn.wgjwhj.cn

Py:   f"{3.14159:.2f}"
来源：http://sp.shxzukj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rh.muxihuayi.cn

JS:   (3.14159).toFixed(2)
来源：http://uf.jctech888.com.cn

TS:   (3.14159).toFixed(2)
来源：http://la.szsharing.cn

Java: String.format("%.2f", 3.14159)
来源：http://ql.chemitech.net.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ip.huixinmuqiang.cn

Ruby: format("%.2f", 3.14159)
来源：http://zs.huixiangedu.cn

C#:   3.14159.ToString("F2")
来源：http://ys.nszjky.cn

[A22] 获取字符串长度
来源：http://pp.yuntaijiaju.cn

Py:   len(s)
来源：http://my.huixiangedu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sm.muxihuayi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wo.muxihuayi.cn

TS:   s.length
来源：http://fw.bookmarksfly.cn

Java: s.length()
来源：http://qf.asd995.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ma.huanxung.cn

Ruby: s.length
来源：http://qe.jctech888.com.cn

C#:   s.Length
来源：http://eq.shxzukj.cn

[A23] 大小写转换
来源：http://kd.huanxung.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gb.shxzukj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wo.huanxung.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://md.yuexingan06.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tf.wgjwhj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rx.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fs.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gd.bjjhwx.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hl.yuntaijiaju.cn

[A24] 去除首尾空白
来源：http://au.shxzskj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fy.shxzukj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pb.yuexingan06.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://an.shtwfgs.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ck.newstarts.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wf.jianghongdianzi.cn

Go:   strings.TrimSpace(s)
来源：http://ea.haigaiapp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xn.nicolike.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qj.szxytkj.cn

[A25] 字符串比较
来源：http://mp.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://gr.gzmigu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gn.muxihuayi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sh.szsharing.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hr.gzmigu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nc.gzmigu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zv.bjjhwx.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ub.shxzukj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dy.chemitech.net.cn

[A26] 类型转换总览
来源：http://ar.gzmigu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bu.shxzskj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kv.gzmigu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ow.shxzskj.cn

TS:   Number() String() Boolean() x as number
来源：http://nl.huanxung.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ql.hahajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://it.shxzukj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ft.wgjwhj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cn.521024.cn

================================================================================
来源：http://st.hahajie.cn

B. 流程控制
来源：http://yn.9csxet.cn

================================================================================
来源：http://il.muxihuayi.cn

[B01] 条件判断 if / else
来源：http://iu.yuexingan06.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ue.panjiajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://se.huanxung.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bc.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ry.muxihuayi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zf.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://aa.jianghongdianzi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rf.szxytkj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pp.nszjky.cn

[B02] 多分支 else if / elif
来源：http://lh.asd995.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wk.521024.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mf.9csxet.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://un.szxytkj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bs.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dz.shtwfgs.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qg.colortex.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hc.nszjky.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vy.bjjhwx.cn

[B03] switch / match / case
来源：http://es.chemitech.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ml.jctech888.com.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ns.nszjky.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qe.9csxet.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ag.jianghongdianzi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sb.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mb.jctech888.com.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uu.yuntaijiaju.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gj.shxzukj.cn

[B04] for 计数循环
来源：http://sd.9csxet.cn

Py:   for i in range(10): print(i)
来源：http://jb.shtwfgs.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wi.yuntaijiaju.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ea.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xt.gzmigu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ts.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hl.newstarts.cn

Ruby: 10.times { |i| puts i }
来源：http://jp.haigaiapp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ev.wgjwhj.cn

[B05] 遍历数组 / 列表
来源：http://qn.szxytkj.cn

Py:   for item in arr: print(item)
来源：http://vb.lnxyls.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ac.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://go.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fc.521024.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kb.nszjky.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gu.gzmigu.cn

Ruby: arr.each { |item| puts item }
来源：http://sx.yuexingan06.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ui.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://tc.yuexingan06.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://iu.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://we.panjiajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wa.szsharing.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://se.asd995.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yx.huanxung.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jy.panjiajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://om.hnjuh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://do.colortex.cn

[B07] while 循环
来源：http://uk.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://nb.yuexingan06.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zk.hnjuh.cn

JS:   while (i < 10) { i++; }
来源：http://yz.nicolike.cn

TS:   while (i < 10) { i++; }
来源：http://iw.chemitech.net.cn

Java: while (i < 10) { i++; }
来源：http://np.muxihuayi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fm.jianghongdianzi.cn

Ruby: while i < 10; i += 1; end
来源：http://uo.wgjwhj.cn

C#:   while (i < 10) { i++; }
来源：http://bv.colortex.cn

[B08] do-while（至少执行一次）
来源：http://qk.521024.cn

Py:   # 无 do-while：用 while True + break
来源：http://lh.gzmigu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://un.lnxyls.cn

JS:   do { i++; } while (i < 10);
来源：http://lj.jianghongdianzi.cn

TS:   do { i++; } while (i < 10);
来源：http://zj.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://br.521024.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tx.521024.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rh.nicolike.cn

C#:   do { i++; } while (i < 10);
来源：http://yk.yuntaijiaju.cn

[B09] break 与 continue
来源：http://hh.jianghongdianzi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uf.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rw.shxzukj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qx.muxihuayi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iy.newstarts.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hn.yuntaijiaju.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ba.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lj.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bx.shxzukj.cn

[B10] 遍历同时拿索引
来源：http://lf.jianghongdianzi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://it.yuexingan06.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tv.muxihuayi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ib.9csxet.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ve.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wi.9csxet.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bd.haigaiapp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uv.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dn.hnjuh.cn

[B11] 生成数字序列 / 区间
来源：http://vl.haigaiapp.cn

Py:   list(range(0, 10, 2))
来源：http://cz.huanxung.cn

PHP:  range(0, 10, 2);
来源：http://pn.huixinmuqiang.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://te.bookmarksfly.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ap.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lq.bjjhwx.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wg.shtwfgs.cn

Ruby: (0...10).step(2).to_a
来源：http://yh.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sv.hnjuh.cn

[B12] 跳出多层循环
来源：http://je.yuntaijiaju.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sq.shxzukj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://le.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ox.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sc.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ep.521024.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ru.nszjky.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qb.shxzukj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rl.huixiangedu.cn

[B13] 判断是否为数字
来源：http://ju.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://na.huixiangedu.cn

PHP:  is_numeric($x)
来源：http://ox.haigaiapp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ni.jctech888.com.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vt.bookmarksfly.cn

Java: x instanceof Number
来源：http://fe.jctech888.com.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bx.lnxyls.cn

Ruby: x.is_a?(Numeric)
来源：http://kd.jianghongdianzi.cn

C#:   x is int or double or decimal
来源：http://lr.nicolike.cn

[B14] 判断值是否在集合内
来源：http://hc.panjiajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gz.521024.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ys.nszjky.cn

JS:   [1, 2, 3].includes(x)
来源：http://wo.9csxet.cn

TS:   [1, 2, 3].includes(x)
来源：http://df.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bj.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yp.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ah.nszjky.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ly.bookmarksfly.cn

[B15] 布尔运算与取反
来源：http://gu.gzmigu.cn

Py:   a and b or not c
来源：http://nt.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://pv.muxihuayi.cn

JS:   a && b || !c
来源：http://tn.lnxyls.cn

TS:   a && b || !c
来源：http://so.nicolike.cn

Java: a && b || !c
来源：http://te.jctech888.com.cn

Go:   a && b || !c
来源：http://lp.bookmarksfly.cn

Ruby: a && b || !c
来源：http://yg.colortex.cn

C#:   a && b || !c
来源：http://vc.jctech888.com.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bt.nicolike.cn


<!-- 参考信息 -->