代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wy.shtwfgs.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ly.shxzukj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://sz.bjjhwx.cn

[A09] 绝对值与最大最小值
来源：http://of.hahajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hy.521024.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yn.521024.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ez.9csxet.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ua.chemitech.net.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pb.asd995.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rv.9csxet.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://uw.wgjwhj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://yr.yuntaijiaju.cn

[A10] 生成随机数
来源：http://to.yuexingan06.cn

Py:   import random; random.randint(1, 100)
来源：http://nx.huanxung.cn

PHP:  random_int(1, 100);
来源：http://nt.huixiangedu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://eq.hahajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ep.bjjhwx.cn

Java: new Random().nextInt(100) + 1
来源：http://lx.nicolike.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ux.colortex.cn

Ruby: rand(1..100)
来源：http://xb.asd995.cn

C#:   new Random().Next(1, 101)
来源：http://zm.huixiangedu.cn

[A11] 条件表达式（三元）
来源：http://kc.shxzukj.cn

Py:   "yes" if x > 0 else "no"
来源：http://fb.jianghongdianzi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xv.bjjhwx.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rf.jianghongdianzi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://fq.jctech888.com.cn

Java: x > 0 ? "yes" : "no"
来源：http://qe.huixinmuqiang.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ej.chemitech.net.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://tm.yuexingan06.cn

C#:   x > 0 ? "yes" : "no"
来源：http://pl.nicolike.cn

[A12] 字符串插值 / 格式化
来源：http://jy.bjjhwx.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lr.colortex.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xu.szxytkj.cn

JS:   `Hello, ${name}!`
来源：http://lg.chemitech.net.cn

TS:   `Hello, ${name}!`
来源：http://ni.huixiangedu.cn

Java: "Hello, %s!".formatted(name)
来源：http://oa.hnjuh.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qs.szsharing.cn

Ruby: "Hello, #{name}!"
来源：http://mz.huanxung.cn

C#:   $"Hello, {name}!"
来源：http://wc.lnxyls.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://bf.hahajie.cn

Py:   "第一行\n第二行"
来源：http://gl.hnjuh.cn

PHP:  "第一行\n第二行"
来源：http://yu.shtwfgs.cn

JS:   "第一行\n第二行"
来源：http://td.yuntaijiaju.cn

TS:   "第一行\n第二行"
来源：http://bd.yuexingan06.cn

Java: "第一行\n第二行"
来源：http://jt.haigaiapp.cn

Go:   "第一行\n第二行"
来源：http://ua.szsharing.cn

Ruby: "第一行\n第二行"
来源：http://vv.nicolike.cn

C#:   "第一行\n第二行"
来源：http://yb.yuexingan06.cn

[A14] 注释写法
来源：http://ur.yuntaijiaju.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ez.bjjhwx.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://vo.wgjwhj.cn

JS:   // 单行；/* 多行 */
来源：http://yq.muxihuayi.cn

TS:   // 单行；/* 多行 */
来源：http://kk.chemitech.net.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bw.colortex.cn

Go:   // 单行；/* 多行 */
来源：http://yw.wgjwhj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vh.huanxung.cn

C#:   // 单行；/* 多行 */
来源：http://nk.newstarts.cn

[A15] 空值判断与默认值
来源：http://fi.shxzskj.cn

Py:   value = data or "默认值"
来源：http://gk.haigaiapp.cn

PHP:  $value = $data ?? "默认值";
来源：http://hf.nicolike.cn

JS:   const value = data ?? "默认值";
来源：http://ee.shxzskj.cn

TS:   const value = data ?? "默认值";
来源：http://he.huanxung.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wz.shxzukj.cn

Go:   if data == "" { data = "默认值" }
来源：http://vy.shxzukj.cn

Ruby: value = data || "默认值"
来源：http://xy.chemitech.net.cn

C#:   var value = data ?? "默认值";
来源：http://nc.9csxet.cn

[A16] 真假值判断规则
来源：http://py.chemitech.net.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fl.shxzskj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ec.huixiangedu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pb.9csxet.cn

TS:   if (!x) {}
来源：http://jt.521024.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wn.newstarts.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jr.huixiangedu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vg.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://eq.muxihuayi.cn

[A17] 位运算
来源：http://bx.521024.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jd.9csxet.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dq.nszjky.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ft.asd995.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kr.panjiajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ug.gzmigu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://uw.jctech888.com.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://us.panjiajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yk.chemitech.net.cn

[A18] 字符与 ASCII 码互转
来源：http://jg.bjjhwx.cn

Py:   ord("A"); chr(65)
来源：http://py.nicolike.cn

PHP:  ord("A"); chr(65)
来源：http://jf.shtwfgs.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yn.muxihuayi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lr.asd995.cn

Java: (int) 'A'; (char) 65
来源：http://yz.asd995.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gl.nszjky.cn

Ruby: "A".ord; 65.chr
来源：http://hh.huixiangedu.cn

C#:   (int)'A'; (char)65
来源：http://vy.huixiangedu.cn

[A19] 交换两个变量
来源：http://lx.panjiajie.cn

Py:   a, b = b, a
来源：http://av.huixinmuqiang.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://bw.muxihuayi.cn

JS:   [a, b] = [b, a];
来源：http://ea.huanxung.cn

TS:   [a, b] = [b, a];
来源：http://jv.chemitech.net.cn

Java: int t = a; a = b; b = t;
来源：http://ol.shtwfgs.cn

Go:   a, b = b, a
来源：http://mf.wgjwhj.cn

Ruby: a, b = b, a
来源：http://kt.szxytkj.cn

C#:   (a, b) = (b, a);
来源：http://lx.asd995.cn

[A20] 读取标准输入
来源：http://ar.szsharing.cn

Py:   name = input("请输入：")
来源：http://st.huixiangedu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://nw.hahajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://er.newstarts.cn

TS:   // Node.js：readline 模块
来源：http://ju.jctech888.com.cn

Java: new Scanner(System.in).nextLine()
来源：http://yf.nicolike.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vg.jianghongdianzi.cn

Ruby: gets.chomp
来源：http://jc.haigaiapp.cn

C#:   Console.ReadLine();
来源：http://nt.asd995.cn

[A21] 保留指定小数位输出
来源：http://tm.jianghongdianzi.cn

Py:   f"{3.14159:.2f}"
来源：http://ny.gzmigu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zh.muxihuayi.cn

JS:   (3.14159).toFixed(2)
来源：http://oh.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://bz.yuntaijiaju.cn

Java: String.format("%.2f", 3.14159)
来源：http://te.shxzukj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zz.bookmarksfly.cn

Ruby: format("%.2f", 3.14159)
来源：http://ti.chemitech.net.cn

C#:   3.14159.ToString("F2")
来源：http://xj.panjiajie.cn

[A22] 获取字符串长度
来源：http://nm.yuexingan06.cn

Py:   len(s)
来源：http://gf.wgjwhj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://im.hnjuh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qf.9csxet.cn

TS:   s.length
来源：http://vn.lnxyls.cn

Java: s.length()
来源：http://rs.hahajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://as.gzmigu.cn

Ruby: s.length
来源：http://qg.shxzukj.cn

C#:   s.Length
来源：http://va.wgjwhj.cn

[A23] 大小写转换
来源：http://fz.nszjky.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://cf.newstarts.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://od.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vh.huixinmuqiang.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gq.shxzukj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ht.shxzukj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lv.szsharing.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nl.jctech888.com.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://te.huanxung.cn

[A24] 去除首尾空白
来源：http://gf.nicolike.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://eh.521024.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pk.huanxung.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ow.colortex.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://in.521024.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wy.huixiangedu.cn

Go:   strings.TrimSpace(s)
来源：http://ll.newstarts.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ux.nszjky.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fy.yuexingan06.cn

[A25] 字符串比较
来源：http://cd.asd995.cn

Py:   s1 == s2; s1 != s2
来源：http://ou.huanxung.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hk.colortex.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://oi.huixinmuqiang.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rj.szsharing.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rr.chemitech.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://um.shxzukj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://kl.szxytkj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dj.bookmarksfly.cn

[A26] 类型转换总览
来源：http://jj.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fc.shxzskj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rc.yuntaijiaju.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wr.asd995.cn

TS:   Number() String() Boolean() x as number
来源：http://og.hahajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bn.jianghongdianzi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://do.huanxung.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rf.panjiajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sb.huanxung.cn

================================================================================
来源：http://qd.yuntaijiaju.cn

B. 流程控制
来源：http://vr.9csxet.cn

================================================================================
来源：http://wd.shxzskj.cn

[B01] 条件判断 if / else
来源：http://iy.huixinmuqiang.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://eh.521024.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bq.bjjhwx.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ve.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qn.gzmigu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gt.bjjhwx.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hn.huixinmuqiang.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sy.chemitech.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ll.wgjwhj.cn

[B02] 多分支 else if / elif
来源：http://yo.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ki.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ca.9csxet.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pn.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ex.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yk.shxzskj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vq.haigaiapp.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tl.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tk.yuexingan06.cn

[B03] switch / match / case
来源：http://pt.yuexingan06.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ia.nicolike.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zr.asd995.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ii.lnxyls.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rx.bookmarksfly.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gp.haigaiapp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rc.asd995.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wd.hnjuh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://oj.yuntaijiaju.cn

[B04] for 计数循环
来源：http://zg.haigaiapp.cn

Py:   for i in range(10): print(i)
来源：http://wu.521024.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ow.panjiajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://id.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zl.chemitech.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xp.wgjwhj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ib.hnjuh.cn

Ruby: 10.times { |i| puts i }
来源：http://rt.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hi.szxytkj.cn

[B05] 遍历数组 / 列表
来源：http://fr.wgjwhj.cn

Py:   for item in arr: print(item)
来源：http://la.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://se.huixinmuqiang.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tv.hahajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dt.jctech888.com.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gm.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sh.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://sj.szsharing.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gs.bjjhwx.cn

[B06] 遍历字典 / 对象
来源：http://ee.nszjky.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ev.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kd.szsharing.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://be.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fg.panjiajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nw.wgjwhj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gm.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xk.huanxung.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cy.nicolike.cn

[B07] while 循环
来源：http://dp.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://fg.yuntaijiaju.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pq.szsharing.cn

JS:   while (i < 10) { i++; }
来源：http://nm.bookmarksfly.cn

TS:   while (i < 10) { i++; }
来源：http://ag.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://cs.shtwfgs.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mm.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://bd.bookmarksfly.cn

C#:   while (i < 10) { i++; }
来源：http://cy.colortex.cn

[B08] do-while（至少执行一次）
来源：http://hg.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://ko.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ek.huanxung.cn

JS:   do { i++; } while (i < 10);
来源：http://wy.521024.cn

TS:   do { i++; } while (i < 10);
来源：http://ke.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://jy.hahajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vy.shtwfgs.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ur.yuntaijiaju.cn

C#:   do { i++; } while (i < 10);
来源：http://nd.shxzskj.cn

[B09] break 与 continue
来源：http://kb.shtwfgs.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rb.szsharing.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zd.huanxung.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qp.shxzskj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hi.nicolike.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jz.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gv.bjjhwx.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wz.jctech888.com.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zo.jctech888.com.cn

[B10] 遍历同时拿索引
来源：http://du.huanxung.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kv.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ip.szxytkj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://md.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qp.huixinmuqiang.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ne.chemitech.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wn.bookmarksfly.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bn.shxzukj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ey.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://pk.yuntaijiaju.cn

Py:   list(range(0, 10, 2))
来源：http://oy.lnxyls.cn

PHP:  range(0, 10, 2);
来源：http://dy.nicolike.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://et.huixiangedu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tr.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vi.bjjhwx.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gh.asd995.cn

Ruby: (0...10).step(2).to_a
来源：http://nq.newstarts.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://az.jctech888.com.cn

[B12] 跳出多层循环
来源：http://ss.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xa.muxihuayi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kk.asd995.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ww.asd995.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uk.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pv.nicolike.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jk.muxihuayi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pj.huanxung.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ou.521024.cn

[B13] 判断是否为数字
来源：http://bh.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://he.yuntaijiaju.cn

PHP:  is_numeric($x)
来源：http://co.bjjhwx.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gx.bookmarksfly.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://em.panjiajie.cn

Java: x instanceof Number
来源：http://yd.huixiangedu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zj.9csxet.cn

Ruby: x.is_a?(Numeric)
来源：http://zu.hnjuh.cn

C#:   x is int or double or decimal
来源：http://gf.lnxyls.cn

[B14] 判断值是否在集合内
来源：http://nh.huixinmuqiang.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ph.shxzukj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tg.nszjky.cn

JS:   [1, 2, 3].includes(x)
来源：http://bp.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://rj.shtwfgs.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vn.szsharing.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://du.jianghongdianzi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qb.newstarts.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gh.panjiajie.cn

[B15] 布尔运算与取反
来源：http://gg.521024.cn

Py:   a and b or not c
来源：http://la.chemitech.net.cn

PHP:  $a && $b || !$c
来源：http://op.colortex.cn

JS:   a && b || !c
来源：http://vz.jctech888.com.cn

TS:   a && b || !c
来源：http://ef.nszjky.cn

Java: a && b || !c
来源：http://rp.asd995.cn


<!-- 参考信息 -->