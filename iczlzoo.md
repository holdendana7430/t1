代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jn.colortex.cn

[A07] 数字转字符串
来源：http://eo.wgjwhj.cn

Py:   str(42)
来源：http://cd.bookmarksfly.cn

PHP:  (string) 42; strval(42)
来源：http://py.nszjky.cn

JS:   String(42); (42).toString()
来源：http://nj.panjiajie.cn

TS:   String(42)
来源：http://pt.521024.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xz.9csxet.cn

Go:   strconv.Itoa(42)
来源：http://hc.hnjuh.cn

Ruby: 42.to_s
来源：http://cv.yuexingan06.cn

C#:   42.ToString()
来源：http://gr.jctech888.com.cn

[A08] 取整与四舍五入
来源：http://mk.nicolike.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ku.yuntaijiaju.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zx.bookmarksfly.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zf.asd995.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gz.haigaiapp.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xz.szsharing.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bg.bookmarksfly.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ce.hahajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vc.panjiajie.cn

[A09] 绝对值与最大最小值
来源：http://tm.yuntaijiaju.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dq.szxytkj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://af.asd995.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qf.jctech888.com.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lp.lnxyls.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zo.9csxet.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://sd.shxzskj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yp.haigaiapp.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wh.9csxet.cn

[A10] 生成随机数
来源：http://yc.yuexingan06.cn

Py:   import random; random.randint(1, 100)
来源：http://ys.521024.cn

PHP:  random_int(1, 100);
来源：http://hq.muxihuayi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qa.yuexingan06.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xp.yuntaijiaju.cn

Java: new Random().nextInt(100) + 1
来源：http://tv.jctech888.com.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ci.hnjuh.cn

Ruby: rand(1..100)
来源：http://sw.bookmarksfly.cn

C#:   new Random().Next(1, 101)
来源：http://be.yuexingan06.cn

[A11] 条件表达式（三元）
来源：http://gn.gzmigu.cn

Py:   "yes" if x > 0 else "no"
来源：http://gh.lnxyls.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://pu.wgjwhj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ov.huixinmuqiang.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rm.wgjwhj.cn

Java: x > 0 ? "yes" : "no"
来源：http://nb.9csxet.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://bn.huanxung.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ms.bookmarksfly.cn

C#:   x > 0 ? "yes" : "no"
来源：http://kc.gzmigu.cn

[A12] 字符串插值 / 格式化
来源：http://rw.shxzskj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hk.shxzukj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yb.jianghongdianzi.cn

JS:   `Hello, ${name}!`
来源：http://xy.yuntaijiaju.cn

TS:   `Hello, ${name}!`
来源：http://am.szxytkj.cn

Java: "Hello, %s!".formatted(name)
来源：http://ij.gzmigu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yo.szxytkj.cn

Ruby: "Hello, #{name}!"
来源：http://wn.huanxung.cn

C#:   $"Hello, {name}!"
来源：http://xr.huixinmuqiang.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ps.jctech888.com.cn

Py:   "第一行\n第二行"
来源：http://rr.nszjky.cn

PHP:  "第一行\n第二行"
来源：http://tr.hnjuh.cn

JS:   "第一行\n第二行"
来源：http://iz.lnxyls.cn

TS:   "第一行\n第二行"
来源：http://ai.hnjuh.cn

Java: "第一行\n第二行"
来源：http://gm.colortex.cn

Go:   "第一行\n第二行"
来源：http://tw.nszjky.cn

Ruby: "第一行\n第二行"
来源：http://yl.haigaiapp.cn

C#:   "第一行\n第二行"
来源：http://tw.shxzukj.cn

[A14] 注释写法
来源：http://bq.newstarts.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ec.nszjky.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hb.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://lf.lnxyls.cn

TS:   // 单行；/* 多行 */
来源：http://oz.nicolike.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://af.wgjwhj.cn

Go:   // 单行；/* 多行 */
来源：http://bm.bookmarksfly.cn

Ruby: # 单行；=begin 多行 =end
来源：http://lb.wgjwhj.cn

C#:   // 单行；/* 多行 */
来源：http://mr.jctech888.com.cn

[A15] 空值判断与默认值
来源：http://or.panjiajie.cn

Py:   value = data or "默认值"
来源：http://hz.huixiangedu.cn

PHP:  $value = $data ?? "默认值";
来源：http://uz.bjjhwx.cn

JS:   const value = data ?? "默认值";
来源：http://wd.chemitech.net.cn

TS:   const value = data ?? "默认值";
来源：http://wb.huixiangedu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vc.nicolike.cn

Go:   if data == "" { data = "默认值" }
来源：http://dt.szsharing.cn

Ruby: value = data || "默认值"
来源：http://dr.jctech888.com.cn

C#:   var value = data ?? "默认值";
来源：http://ls.yuntaijiaju.cn

[A16] 真假值判断规则
来源：http://rk.huanxung.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pq.huixinmuqiang.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://od.9csxet.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sa.shxzskj.cn

TS:   if (!x) {}
来源：http://cd.shtwfgs.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gx.panjiajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rj.nszjky.cn

Ruby: unless x            # nil 与 false 为假
来源：http://qd.colortex.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vl.gzmigu.cn

[A17] 位运算
来源：http://yj.panjiajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bv.haigaiapp.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://so.colortex.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ll.huanxung.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qp.bjjhwx.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nk.jianghongdianzi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jf.nszjky.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kn.asd995.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gg.colortex.cn

[A18] 字符与 ASCII 码互转
来源：http://vo.shxzukj.cn

Py:   ord("A"); chr(65)
来源：http://ra.shxzskj.cn

PHP:  ord("A"); chr(65)
来源：http://md.huixinmuqiang.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hr.nszjky.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sz.colortex.cn

Java: (int) 'A'; (char) 65
来源：http://rw.yuexingan06.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ts.newstarts.cn

Ruby: "A".ord; 65.chr
来源：http://kh.hnjuh.cn

C#:   (int)'A'; (char)65
来源：http://ha.shtwfgs.cn

[A19] 交换两个变量
来源：http://wr.yuntaijiaju.cn

Py:   a, b = b, a
来源：http://dx.jctech888.com.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://em.shxzskj.cn

JS:   [a, b] = [b, a];
来源：http://ex.yuexingan06.cn

TS:   [a, b] = [b, a];
来源：http://yc.huixiangedu.cn

Java: int t = a; a = b; b = t;
来源：http://zo.szxytkj.cn

Go:   a, b = b, a
来源：http://ql.jctech888.com.cn

Ruby: a, b = b, a
来源：http://bb.hnjuh.cn

C#:   (a, b) = (b, a);
来源：http://nl.szxytkj.cn

[A20] 读取标准输入
来源：http://vc.lnxyls.cn

Py:   name = input("请输入：")
来源：http://of.szsharing.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ui.9csxet.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://av.huixinmuqiang.cn

TS:   // Node.js：readline 模块
来源：http://ee.haigaiapp.cn

Java: new Scanner(System.in).nextLine()
来源：http://av.nszjky.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nv.jianghongdianzi.cn

Ruby: gets.chomp
来源：http://ct.szsharing.cn

C#:   Console.ReadLine();
来源：http://rl.hnjuh.cn

[A21] 保留指定小数位输出
来源：http://bp.chemitech.net.cn

Py:   f"{3.14159:.2f}"
来源：http://uf.wgjwhj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gx.nszjky.cn

JS:   (3.14159).toFixed(2)
来源：http://uc.jianghongdianzi.cn

TS:   (3.14159).toFixed(2)
来源：http://il.panjiajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://tf.wgjwhj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rn.szxytkj.cn

Ruby: format("%.2f", 3.14159)
来源：http://tk.shxzukj.cn

C#:   3.14159.ToString("F2")
来源：http://gn.yuexingan06.cn

[A22] 获取字符串长度
来源：http://rh.asd995.cn

Py:   len(s)
来源：http://ly.szsharing.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rs.521024.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://az.shtwfgs.cn

TS:   s.length
来源：http://sq.yuntaijiaju.cn

Java: s.length()
来源：http://bo.asd995.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yj.bjjhwx.cn

Ruby: s.length
来源：http://nc.muxihuayi.cn

C#:   s.Length
来源：http://nd.asd995.cn

[A23] 大小写转换
来源：http://so.hnjuh.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fo.shtwfgs.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bq.shtwfgs.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ln.lnxyls.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nb.shxzskj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nb.lnxyls.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dp.9csxet.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ur.szxytkj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://yj.lnxyls.cn

[A24] 去除首尾空白
来源：http://tu.hnjuh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dq.asd995.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gr.chemitech.net.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nx.haigaiapp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ea.shxzukj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xo.hahajie.cn

Go:   strings.TrimSpace(s)
来源：http://xz.szsharing.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kx.nicolike.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zi.jianghongdianzi.cn

[A25] 字符串比较
来源：http://lw.newstarts.cn

Py:   s1 == s2; s1 != s2
来源：http://kt.yuntaijiaju.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uw.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wc.colortex.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sp.lnxyls.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kb.wgjwhj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gs.shxzukj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ez.chemitech.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jh.szxytkj.cn

[A26] 类型转换总览
来源：http://fk.szxytkj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yd.huanxung.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://op.huixinmuqiang.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zo.huixinmuqiang.cn

TS:   Number() String() Boolean() x as number
来源：http://gr.bjjhwx.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mm.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kn.hahajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nh.nicolike.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qw.nicolike.cn

================================================================================
来源：http://de.gzmigu.cn

B. 流程控制
来源：http://it.gzmigu.cn

================================================================================
来源：http://zd.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://ic.shxzukj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cc.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vq.nicolike.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ry.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ad.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bn.jianghongdianzi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://es.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lw.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dm.jctech888.com.cn

[B02] 多分支 else if / elif
来源：http://iw.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://be.huixinmuqiang.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://no.szxytkj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zs.nszjky.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hf.gzmigu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qq.shxzukj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ta.shxzukj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jz.asd995.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vv.hnjuh.cn

[B03] switch / match / case
来源：http://qa.haigaiapp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://id.muxihuayi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dz.szsharing.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jl.bookmarksfly.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jy.muxihuayi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yk.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://og.huixiangedu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gs.jianghongdianzi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sl.yuexingan06.cn

[B04] for 计数循环
来源：http://zv.hahajie.cn

Py:   for i in range(10): print(i)
来源：http://ky.jianghongdianzi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cy.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jn.hnjuh.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nz.nszjky.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ty.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jo.nszjky.cn

Ruby: 10.times { |i| puts i }
来源：http://sz.szsharing.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mc.szxytkj.cn

[B05] 遍历数组 / 列表
来源：http://od.shxzskj.cn

Py:   for item in arr: print(item)
来源：http://xd.haigaiapp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vm.lnxyls.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://cl.panjiajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://iv.bookmarksfly.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fk.jianghongdianzi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pm.lnxyls.cn

Ruby: arr.each { |item| puts item }
来源：http://ak.nszjky.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ri.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://qs.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dq.wgjwhj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uf.huanxung.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vb.yuntaijiaju.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fn.yuexingan06.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rx.huixinmuqiang.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gg.wgjwhj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rv.shxzukj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://df.521024.cn

[B07] while 循环
来源：http://om.asd995.cn

Py:   while i < 10: i += 1
来源：http://km.huixiangedu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ck.szxytkj.cn

JS:   while (i < 10) { i++; }
来源：http://ha.yuexingan06.cn

TS:   while (i < 10) { i++; }
来源：http://gg.panjiajie.cn

Java: while (i < 10) { i++; }
来源：http://bn.wgjwhj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ay.hahajie.cn

Ruby: while i < 10; i += 1; end
来源：http://wi.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://sv.shxzukj.cn

[B08] do-while（至少执行一次）
来源：http://fq.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://gs.panjiajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ha.jctech888.com.cn

JS:   do { i++; } while (i < 10);
来源：http://mv.gzmigu.cn

TS:   do { i++; } while (i < 10);
来源：http://gh.521024.cn

Java: do { i++; } while (i < 10);
来源：http://mu.bjjhwx.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ul.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bb.szsharing.cn

C#:   do { i++; } while (i < 10);
来源：http://qi.asd995.cn

[B09] break 与 continue
来源：http://hw.chemitech.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ll.huixinmuqiang.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qe.shxzukj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iz.yuexingan06.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wm.gzmigu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zu.hahajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jl.nszjky.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fm.hnjuh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ra.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://ou.hahajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xd.jianghongdianzi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sm.bjjhwx.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qo.wgjwhj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tv.nszjky.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jk.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://iq.yuexingan06.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://po.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mj.lnxyls.cn

[B11] 生成数字序列 / 区间
来源：http://bq.hnjuh.cn

Py:   list(range(0, 10, 2))
来源：http://wa.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://lv.yuntaijiaju.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kz.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tj.nszjky.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nn.hnjuh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://iy.szsharing.cn

Ruby: (0...10).step(2).to_a
来源：http://ac.9csxet.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vz.yuntaijiaju.cn

[B12] 跳出多层循环
来源：http://qa.wgjwhj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wj.huixiangedu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dz.gzmigu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vf.yuexingan06.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jf.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ev.9csxet.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pl.shxzskj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mx.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hy.newstarts.cn

[B13] 判断是否为数字
来源：http://cx.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://at.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://nd.panjiajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gl.chemitech.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dm.huanxung.cn

Java: x instanceof Number
来源：http://sf.bookmarksfly.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gy.colortex.cn

Ruby: x.is_a?(Numeric)
来源：http://uc.huixinmuqiang.cn


<!-- 参考信息 -->