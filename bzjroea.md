代发 wailian999

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://km.lnxyls.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jt.9csxet.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ds.muxihuayi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kk.521024.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gp.huanxung.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://bn.nicolike.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ce.huanxung.cn

[A09] 绝对值与最大最小值
来源：http://hj.muxihuayi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ai.szsharing.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://st.huanxung.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qn.shxzukj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gs.9csxet.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://od.shxzskj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ys.9csxet.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mz.jianghongdianzi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vr.hnjuh.cn

[A10] 生成随机数
来源：http://uf.gzmigu.cn

Py:   import random; random.randint(1, 100)
来源：http://ab.muxihuayi.cn

PHP:  random_int(1, 100);
来源：http://ub.yuntaijiaju.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xa.szsharing.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wc.wgjwhj.cn

Java: new Random().nextInt(100) + 1
来源：http://us.haigaiapp.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://at.huanxung.cn

Ruby: rand(1..100)
来源：http://uw.nicolike.cn

C#:   new Random().Next(1, 101)
来源：http://st.gzmigu.cn

[A11] 条件表达式（三元）
来源：http://ep.muxihuayi.cn

Py:   "yes" if x > 0 else "no"
来源：http://uz.chemitech.net.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://mz.jianghongdianzi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://yc.hnjuh.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vu.shtwfgs.cn

Java: x > 0 ? "yes" : "no"
来源：http://rc.szsharing.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://om.hnjuh.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://da.nicolike.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ll.muxihuayi.cn

[A12] 字符串插值 / 格式化
来源：http://cd.szxytkj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cr.huanxung.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xm.huixiangedu.cn

JS:   `Hello, ${name}!`
来源：http://zc.asd995.cn

TS:   `Hello, ${name}!`
来源：http://nu.bjjhwx.cn

Java: "Hello, %s!".formatted(name)
来源：http://yg.szxytkj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jq.chemitech.net.cn

Ruby: "Hello, #{name}!"
来源：http://ce.shxzukj.cn

C#:   $"Hello, {name}!"
来源：http://hd.asd995.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://rz.shxzskj.cn

Py:   "第一行\n第二行"
来源：http://dy.nicolike.cn

PHP:  "第一行\n第二行"
来源：http://dp.asd995.cn

JS:   "第一行\n第二行"
来源：http://xi.szsharing.cn

TS:   "第一行\n第二行"
来源：http://ld.nicolike.cn

Java: "第一行\n第二行"
来源：http://yl.yuntaijiaju.cn

Go:   "第一行\n第二行"
来源：http://ib.muxihuayi.cn

Ruby: "第一行\n第二行"
来源：http://kt.hnjuh.cn

C#:   "第一行\n第二行"
来源：http://ch.lnxyls.cn

[A14] 注释写法
来源：http://zq.gzmigu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ej.huanxung.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://sh.9csxet.cn

JS:   // 单行；/* 多行 */
来源：http://cd.hnjuh.cn

TS:   // 单行；/* 多行 */
来源：http://wo.huanxung.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ga.shxzukj.cn

Go:   // 单行；/* 多行 */
来源：http://zx.gzmigu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://lq.szxytkj.cn

C#:   // 单行；/* 多行 */
来源：http://ri.lnxyls.cn

[A15] 空值判断与默认值
来源：http://fp.bookmarksfly.cn

Py:   value = data or "默认值"
来源：http://he.panjiajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://re.hnjuh.cn

JS:   const value = data ?? "默认值";
来源：http://ps.szxytkj.cn

TS:   const value = data ?? "默认值";
来源：http://gd.huixiangedu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gx.bjjhwx.cn

Go:   if data == "" { data = "默认值" }
来源：http://db.newstarts.cn

Ruby: value = data || "默认值"
来源：http://ep.jianghongdianzi.cn

C#:   var value = data ?? "默认值";
来源：http://cm.newstarts.cn

[A16] 真假值判断规则
来源：http://ee.shtwfgs.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gz.nszjky.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gp.yuexingan06.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yp.bjjhwx.cn

TS:   if (!x) {}
来源：http://gc.chemitech.net.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ig.wgjwhj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cf.huixiangedu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hc.9csxet.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cu.shxzukj.cn

[A17] 位运算
来源：http://jh.chemitech.net.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ol.panjiajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ss.shtwfgs.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sj.hnjuh.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://iw.muxihuayi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sj.szxytkj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ea.bjjhwx.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gu.nszjky.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sm.chemitech.net.cn

[A18] 字符与 ASCII 码互转
来源：http://fy.521024.cn

Py:   ord("A"); chr(65)
来源：http://tx.bjjhwx.cn

PHP:  ord("A"); chr(65)
来源：http://lx.haigaiapp.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pc.nszjky.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iz.yuexingan06.cn

Java: (int) 'A'; (char) 65
来源：http://cn.newstarts.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rt.panjiajie.cn

Ruby: "A".ord; 65.chr
来源：http://ic.shxzskj.cn

C#:   (int)'A'; (char)65
来源：http://zb.haigaiapp.cn

[A19] 交换两个变量
来源：http://yp.nicolike.cn

Py:   a, b = b, a
来源：http://ch.9csxet.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vg.hahajie.cn

JS:   [a, b] = [b, a];
来源：http://ii.nszjky.cn

TS:   [a, b] = [b, a];
来源：http://rd.yuntaijiaju.cn

Java: int t = a; a = b; b = t;
来源：http://xh.shtwfgs.cn

Go:   a, b = b, a
来源：http://ta.gzmigu.cn

Ruby: a, b = b, a
来源：http://ma.nszjky.cn

C#:   (a, b) = (b, a);
来源：http://ze.huanxung.cn

[A20] 读取标准输入
来源：http://fz.yuexingan06.cn

Py:   name = input("请输入：")
来源：http://ye.nszjky.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ji.panjiajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ab.jianghongdianzi.cn

TS:   // Node.js：readline 模块
来源：http://bt.bookmarksfly.cn

Java: new Scanner(System.in).nextLine()
来源：http://ko.bookmarksfly.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kn.gzmigu.cn

Ruby: gets.chomp
来源：http://ax.newstarts.cn

C#:   Console.ReadLine();
来源：http://ns.szsharing.cn

[A21] 保留指定小数位输出
来源：http://ic.nicolike.cn

Py:   f"{3.14159:.2f}"
来源：http://qo.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fy.bjjhwx.cn

JS:   (3.14159).toFixed(2)
来源：http://he.huanxung.cn

TS:   (3.14159).toFixed(2)
来源：http://jw.gzmigu.cn

Java: String.format("%.2f", 3.14159)
来源：http://dp.521024.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://na.chemitech.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://lv.bookmarksfly.cn

C#:   3.14159.ToString("F2")
来源：http://kd.panjiajie.cn

[A22] 获取字符串长度
来源：http://xb.nicolike.cn

Py:   len(s)
来源：http://cq.hahajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pp.bjjhwx.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jy.huixiangedu.cn

TS:   s.length
来源：http://tb.muxihuayi.cn

Java: s.length()
来源：http://cg.colortex.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ht.shxzskj.cn

Ruby: s.length
来源：http://ic.hahajie.cn

C#:   s.Length
来源：http://ht.jctech888.com.cn

[A23] 大小写转换
来源：http://ab.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zj.wgjwhj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pg.gzmigu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://io.9csxet.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pr.yuntaijiaju.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vr.nszjky.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ha.hahajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gg.huanxung.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ko.jctech888.com.cn

[A24] 去除首尾空白
来源：http://gb.yuntaijiaju.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sj.newstarts.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cf.lnxyls.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oi.lnxyls.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kv.lnxyls.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://th.huixiangedu.cn

Go:   strings.TrimSpace(s)
来源：http://mn.nicolike.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lf.haigaiapp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://us.521024.cn

[A25] 字符串比较
来源：http://gp.huixiangedu.cn

Py:   s1 == s2; s1 != s2
来源：http://uy.yuntaijiaju.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yc.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ze.huanxung.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lb.asd995.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ri.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mw.chemitech.net.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ff.jianghongdianzi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nb.shtwfgs.cn

[A26] 类型转换总览
来源：http://co.muxihuayi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ed.nszjky.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jn.jianghongdianzi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wa.wgjwhj.cn

TS:   Number() String() Boolean() x as number
来源：http://kp.chemitech.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mb.nicolike.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sj.jianghongdianzi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ng.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wf.asd995.cn

================================================================================
来源：http://kv.jianghongdianzi.cn

B. 流程控制
来源：http://yr.9csxet.cn

================================================================================
来源：http://ud.szsharing.cn

[B01] 条件判断 if / else
来源：http://su.yuexingan06.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bz.panjiajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ff.nicolike.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hk.huanxung.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fe.hahajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zv.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lx.9csxet.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hl.gzmigu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jt.wgjwhj.cn

[B02] 多分支 else if / elif
来源：http://tj.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://of.shxzukj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ym.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gf.haigaiapp.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pi.huixinmuqiang.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dm.nicolike.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cy.colortex.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cq.shxzukj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mk.szsharing.cn

[B03] switch / match / case
来源：http://ev.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bx.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gh.bookmarksfly.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qa.haigaiapp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fh.huixiangedu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xd.colortex.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yn.colortex.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ej.shxzukj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kr.panjiajie.cn

[B04] for 计数循环
来源：http://lm.yuntaijiaju.cn

Py:   for i in range(10): print(i)
来源：http://go.wgjwhj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ux.wgjwhj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xr.shtwfgs.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cw.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jh.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://si.yuexingan06.cn

Ruby: 10.times { |i| puts i }
来源：http://oh.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uk.haigaiapp.cn

[B05] 遍历数组 / 列表
来源：http://fw.hahajie.cn

Py:   for item in arr: print(item)
来源：http://ak.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ft.gzmigu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ue.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rp.shxzukj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bi.hnjuh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lu.bjjhwx.cn

Ruby: arr.each { |item| puts item }
来源：http://vm.szsharing.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ze.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://br.asd995.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bd.newstarts.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ss.wgjwhj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kj.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cj.yuexingan06.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jp.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dr.hnjuh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://km.shtwfgs.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ig.huixinmuqiang.cn

[B07] while 循环
来源：http://um.muxihuayi.cn

Py:   while i < 10: i += 1
来源：http://jd.jctech888.com.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gk.hahajie.cn

JS:   while (i < 10) { i++; }
来源：http://lo.lnxyls.cn

TS:   while (i < 10) { i++; }
来源：http://fr.yuntaijiaju.cn

Java: while (i < 10) { i++; }
来源：http://mw.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vm.hnjuh.cn

Ruby: while i < 10; i += 1; end
来源：http://td.colortex.cn

C#:   while (i < 10) { i++; }
来源：http://gf.nszjky.cn

[B08] do-while（至少执行一次）
来源：http://mt.huixiangedu.cn

Py:   # 无 do-while：用 while True + break
来源：http://iq.newstarts.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ck.huixinmuqiang.cn

JS:   do { i++; } while (i < 10);
来源：http://ug.bookmarksfly.cn

TS:   do { i++; } while (i < 10);
来源：http://bt.panjiajie.cn

Java: do { i++; } while (i < 10);
来源：http://ot.yuexingan06.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xp.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nc.yuntaijiaju.cn

C#:   do { i++; } while (i < 10);
来源：http://oc.gzmigu.cn

[B09] break 与 continue
来源：http://qp.yuexingan06.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mk.jctech888.com.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yq.nszjky.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mp.yuntaijiaju.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://it.gzmigu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ys.panjiajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mw.jctech888.com.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ij.nicolike.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ng.jianghongdianzi.cn

[B10] 遍历同时拿索引
来源：http://zq.huanxung.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://re.shtwfgs.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://eu.wgjwhj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ct.shxzskj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nb.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jw.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pj.wgjwhj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ij.gzmigu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rh.bjjhwx.cn

[B11] 生成数字序列 / 区间
来源：http://di.nszjky.cn

Py:   list(range(0, 10, 2))
来源：http://eu.newstarts.cn

PHP:  range(0, 10, 2);
来源：http://tl.wgjwhj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ue.yuntaijiaju.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jb.newstarts.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kl.jianghongdianzi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jt.yuexingan06.cn

Ruby: (0...10).step(2).to_a
来源：http://dc.huixiangedu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://po.szxytkj.cn

[B12] 跳出多层循环
来源：http://zv.nicolike.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zs.yuexingan06.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gw.yuntaijiaju.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ga.huixinmuqiang.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pl.nszjky.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ty.huixiangedu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tq.yuexingan06.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pq.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qq.jianghongdianzi.cn

[B13] 判断是否为数字
来源：http://yx.huanxung.cn

Py:   isinstance(x, (int, float))
来源：http://nf.521024.cn

PHP:  is_numeric($x)
来源：http://pt.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://me.szsharing.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qu.haigaiapp.cn

Java: x instanceof Number
来源：http://si.gzmigu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mm.panjiajie.cn

Ruby: x.is_a?(Numeric)
来源：http://lu.newstarts.cn

C#:   x is int or double or decimal
来源：http://vy.hahajie.cn

[B14] 判断值是否在集合内
来源：http://uu.hahajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://la.yuexingan06.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ch.asd995.cn

JS:   [1, 2, 3].includes(x)
来源：http://ed.9csxet.cn

TS:   [1, 2, 3].includes(x)
来源：http://eu.haigaiapp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hv.jctech888.com.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tb.panjiajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hc.panjiajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ms.huanxung.cn

[B15] 布尔运算与取反
来源：http://zu.bjjhwx.cn

Py:   a and b or not c
来源：http://th.521024.cn


<!-- 参考信息 -->