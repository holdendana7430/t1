代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gq.asd995.cn

[A07] 数字转字符串
来源：http://ul.shxzukj.cn

Py:   str(42)
来源：http://ai.huixiangedu.cn

PHP:  (string) 42; strval(42)
来源：http://er.hnjuh.cn

JS:   String(42); (42).toString()
来源：http://ga.gzmigu.cn

TS:   String(42)
来源：http://ic.colortex.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://bg.9csxet.cn

Go:   strconv.Itoa(42)
来源：http://gs.hahajie.cn

Ruby: 42.to_s
来源：http://ua.hahajie.cn

C#:   42.ToString()
来源：http://me.521024.cn

[A08] 取整与四舍五入
来源：http://xi.shxzukj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bu.shxzskj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bo.huixinmuqiang.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://po.panjiajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vt.bookmarksfly.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nz.lnxyls.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ps.hnjuh.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ru.shxzskj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://le.yuntaijiaju.cn

[A09] 绝对值与最大最小值
来源：http://yu.asd995.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rv.szsharing.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qp.521024.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://iq.yuntaijiaju.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wo.shxzukj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hi.jctech888.com.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wa.lnxyls.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wj.huixinmuqiang.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://os.hahajie.cn

[A10] 生成随机数
来源：http://mt.chemitech.net.cn

Py:   import random; random.randint(1, 100)
来源：http://mr.shtwfgs.cn

PHP:  random_int(1, 100);
来源：http://do.asd995.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://uc.jctech888.com.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ev.szsharing.cn

Java: new Random().nextInt(100) + 1
来源：http://yq.huixinmuqiang.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://di.shtwfgs.cn

Ruby: rand(1..100)
来源：http://qy.muxihuayi.cn

C#:   new Random().Next(1, 101)
来源：http://rt.bjjhwx.cn

[A11] 条件表达式（三元）
来源：http://ud.yuntaijiaju.cn

Py:   "yes" if x > 0 else "no"
来源：http://ve.bookmarksfly.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://if.wgjwhj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://or.jctech888.com.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rt.shxzukj.cn

Java: x > 0 ? "yes" : "no"
来源：http://gh.521024.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xn.chemitech.net.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://mr.nicolike.cn

C#:   x > 0 ? "yes" : "no"
来源：http://to.shxzukj.cn

[A12] 字符串插值 / 格式化
来源：http://pe.jianghongdianzi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zv.lnxyls.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ot.jianghongdianzi.cn

JS:   `Hello, ${name}!`
来源：http://sf.szxytkj.cn

TS:   `Hello, ${name}!`
来源：http://gc.huixinmuqiang.cn

Java: "Hello, %s!".formatted(name)
来源：http://gv.muxihuayi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dj.huixiangedu.cn

Ruby: "Hello, #{name}!"
来源：http://jo.shtwfgs.cn

C#:   $"Hello, {name}!"
来源：http://to.nicolike.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://mi.huixinmuqiang.cn

Py:   "第一行\n第二行"
来源：http://jo.jctech888.com.cn

PHP:  "第一行\n第二行"
来源：http://ab.yuntaijiaju.cn

JS:   "第一行\n第二行"
来源：http://qs.jctech888.com.cn

TS:   "第一行\n第二行"
来源：http://wo.panjiajie.cn

Java: "第一行\n第二行"
来源：http://bz.bjjhwx.cn

Go:   "第一行\n第二行"
来源：http://ep.newstarts.cn

Ruby: "第一行\n第二行"
来源：http://lu.huixinmuqiang.cn

C#:   "第一行\n第二行"
来源：http://be.huixinmuqiang.cn

[A14] 注释写法
来源：http://qw.colortex.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://my.shxzukj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://kb.jctech888.com.cn

JS:   // 单行；/* 多行 */
来源：http://hb.yuexingan06.cn

TS:   // 单行；/* 多行 */
来源：http://pv.shxzskj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zp.szxytkj.cn

Go:   // 单行；/* 多行 */
来源：http://hh.szxytkj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xi.szxytkj.cn

C#:   // 单行；/* 多行 */
来源：http://pk.nicolike.cn

[A15] 空值判断与默认值
来源：http://za.huanxung.cn

Py:   value = data or "默认值"
来源：http://zj.shtwfgs.cn

PHP:  $value = $data ?? "默认值";
来源：http://ji.huanxung.cn

JS:   const value = data ?? "默认值";
来源：http://wx.hahajie.cn

TS:   const value = data ?? "默认值";
来源：http://jx.panjiajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zt.muxihuayi.cn

Go:   if data == "" { data = "默认值" }
来源：http://dc.szxytkj.cn

Ruby: value = data || "默认值"
来源：http://ij.lnxyls.cn

C#:   var value = data ?? "默认值";
来源：http://oq.521024.cn

[A16] 真假值判断规则
来源：http://pr.muxihuayi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ny.9csxet.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yk.yuntaijiaju.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uj.huanxung.cn

TS:   if (!x) {}
来源：http://xu.hahajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ea.muxihuayi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fe.jianghongdianzi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://yb.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bg.bjjhwx.cn

[A17] 位运算
来源：http://ef.newstarts.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ux.521024.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bu.shtwfgs.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hv.szxytkj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pg.huanxung.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gk.shxzskj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://om.shtwfgs.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ck.wgjwhj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qj.newstarts.cn

[A18] 字符与 ASCII 码互转
来源：http://sc.szxytkj.cn

Py:   ord("A"); chr(65)
来源：http://iu.nicolike.cn

PHP:  ord("A"); chr(65)
来源：http://ye.wgjwhj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ev.szsharing.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nk.haigaiapp.cn

Java: (int) 'A'; (char) 65
来源：http://bm.muxihuayi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qe.521024.cn

Ruby: "A".ord; 65.chr
来源：http://ng.shxzukj.cn

C#:   (int)'A'; (char)65
来源：http://yw.lnxyls.cn

[A19] 交换两个变量
来源：http://hm.9csxet.cn

Py:   a, b = b, a
来源：http://kt.shxzskj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ii.nicolike.cn

JS:   [a, b] = [b, a];
来源：http://ki.shxzukj.cn

TS:   [a, b] = [b, a];
来源：http://ox.wgjwhj.cn

Java: int t = a; a = b; b = t;
来源：http://cy.haigaiapp.cn

Go:   a, b = b, a
来源：http://ug.yuntaijiaju.cn

Ruby: a, b = b, a
来源：http://vd.shxzukj.cn

C#:   (a, b) = (b, a);
来源：http://zr.jctech888.com.cn

[A20] 读取标准输入
来源：http://xh.nicolike.cn

Py:   name = input("请输入：")
来源：http://lf.nszjky.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qc.chemitech.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bz.nicolike.cn

TS:   // Node.js：readline 模块
来源：http://ai.colortex.cn

Java: new Scanner(System.in).nextLine()
来源：http://vo.panjiajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wq.muxihuayi.cn

Ruby: gets.chomp
来源：http://lv.shtwfgs.cn

C#:   Console.ReadLine();
来源：http://ze.bookmarksfly.cn

[A21] 保留指定小数位输出
来源：http://rr.panjiajie.cn

Py:   f"{3.14159:.2f}"
来源：http://im.newstarts.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zh.huanxung.cn

JS:   (3.14159).toFixed(2)
来源：http://qj.shtwfgs.cn

TS:   (3.14159).toFixed(2)
来源：http://vj.shtwfgs.cn

Java: String.format("%.2f", 3.14159)
来源：http://qh.huanxung.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qu.9csxet.cn

Ruby: format("%.2f", 3.14159)
来源：http://dh.lnxyls.cn

C#:   3.14159.ToString("F2")
来源：http://wn.jianghongdianzi.cn

[A22] 获取字符串长度
来源：http://gd.jianghongdianzi.cn

Py:   len(s)
来源：http://rc.hnjuh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pv.asd995.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ud.newstarts.cn

TS:   s.length
来源：http://ux.huixiangedu.cn

Java: s.length()
来源：http://ko.bookmarksfly.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ou.yuntaijiaju.cn

Ruby: s.length
来源：http://tw.gzmigu.cn

C#:   s.Length
来源：http://fs.9csxet.cn

[A23] 大小写转换
来源：http://ty.chemitech.net.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kk.shxzukj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hk.jianghongdianzi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yd.newstarts.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://oa.jctech888.com.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://uc.chemitech.net.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jd.wgjwhj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://as.lnxyls.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://tr.szsharing.cn

[A24] 去除首尾空白
来源：http://nz.szsharing.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nd.szxytkj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dk.521024.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dq.nszjky.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://li.asd995.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dq.yuexingan06.cn

Go:   strings.TrimSpace(s)
来源：http://nw.colortex.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uj.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tg.asd995.cn

[A25] 字符串比较
来源：http://vu.newstarts.cn

Py:   s1 == s2; s1 != s2
来源：http://cj.bjjhwx.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.szxytkj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uu.jctech888.com.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gw.yuntaijiaju.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fn.shxzukj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ck.chemitech.net.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://kv.shtwfgs.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://up.hahajie.cn

[A26] 类型转换总览
来源：http://jp.9csxet.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qn.gzmigu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zk.shtwfgs.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yg.9csxet.cn

TS:   Number() String() Boolean() x as number
来源：http://go.yuntaijiaju.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://az.nszjky.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xa.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://xd.chemitech.net.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bs.yuexingan06.cn

================================================================================
来源：http://fk.9csxet.cn

B. 流程控制
来源：http://xb.haigaiapp.cn

================================================================================
来源：http://zf.colortex.cn

[B01] 条件判断 if / else
来源：http://nd.yuexingan06.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zu.yuexingan06.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qb.szsharing.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gc.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yy.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vt.huixinmuqiang.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qi.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lr.yuexingan06.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fn.haigaiapp.cn

[B02] 多分支 else if / elif
来源：http://rk.huanxung.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ox.jctech888.com.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://el.huixiangedu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://da.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qq.yuntaijiaju.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kl.wgjwhj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://be.lnxyls.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pf.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nl.lnxyls.cn

[B03] switch / match / case
来源：http://me.haigaiapp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ru.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ss.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sl.lnxyls.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fk.9csxet.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zg.bookmarksfly.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pl.jctech888.com.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://za.hnjuh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ys.jctech888.com.cn

[B04] for 计数循环
来源：http://fq.chemitech.net.cn

Py:   for i in range(10): print(i)
来源：http://vv.huanxung.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://de.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jq.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://up.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ob.wgjwhj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://df.521024.cn

Ruby: 10.times { |i| puts i }
来源：http://vz.shtwfgs.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nl.muxihuayi.cn

[B05] 遍历数组 / 列表
来源：http://gb.shtwfgs.cn

Py:   for item in arr: print(item)
来源：http://tt.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://el.haigaiapp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yx.wgjwhj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qw.szsharing.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://in.9csxet.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lu.haigaiapp.cn

Ruby: arr.each { |item| puts item }
来源：http://xk.asd995.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nb.yuexingan06.cn

[B06] 遍历字典 / 对象
来源：http://wj.shxzukj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ru.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hm.jianghongdianzi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cj.hnjuh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dw.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://io.yuntaijiaju.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jg.panjiajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ec.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://oo.haigaiapp.cn

[B07] while 循环
来源：http://xr.shxzukj.cn

Py:   while i < 10: i += 1
来源：http://cp.szxytkj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yi.chemitech.net.cn

JS:   while (i < 10) { i++; }
来源：http://jg.szxytkj.cn

TS:   while (i < 10) { i++; }
来源：http://dc.hahajie.cn

Java: while (i < 10) { i++; }
来源：http://pb.panjiajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vd.yuntaijiaju.cn

Ruby: while i < 10; i += 1; end
来源：http://lx.huixinmuqiang.cn

C#:   while (i < 10) { i++; }
来源：http://vk.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://to.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://av.hnjuh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://aa.szsharing.cn

JS:   do { i++; } while (i < 10);
来源：http://ow.colortex.cn

TS:   do { i++; } while (i < 10);
来源：http://ds.szsharing.cn

Java: do { i++; } while (i < 10);
来源：http://kw.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://uy.newstarts.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pm.jianghongdianzi.cn

C#:   do { i++; } while (i < 10);
来源：http://qn.jianghongdianzi.cn

[B09] break 与 continue
来源：http://oe.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://px.newstarts.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ny.szxytkj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://er.521024.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://go.gzmigu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://io.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://au.huanxung.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cd.jianghongdianzi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kw.hnjuh.cn

[B10] 遍历同时拿索引
来源：http://oc.wgjwhj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cl.shtwfgs.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xm.asd995.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fp.huixiangedu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pi.chemitech.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sx.shxzskj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pp.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ih.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zd.szsharing.cn

[B11] 生成数字序列 / 区间
来源：http://mb.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://av.chemitech.net.cn

PHP:  range(0, 10, 2);
来源：http://em.colortex.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cw.huixiangedu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yw.szsharing.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rp.shtwfgs.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sr.panjiajie.cn

Ruby: (0...10).step(2).to_a
来源：http://pg.521024.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jf.yuntaijiaju.cn

[B12] 跳出多层循环
来源：http://qz.panjiajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hq.hahajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ve.hnjuh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ar.yuntaijiaju.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jp.asd995.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ef.bookmarksfly.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ek.yuexingan06.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ai.bookmarksfly.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cf.panjiajie.cn

[B13] 判断是否为数字
来源：http://lx.huixinmuqiang.cn

Py:   isinstance(x, (int, float))
来源：http://ov.shxzskj.cn

PHP:  is_numeric($x)
来源：http://vd.jianghongdianzi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ov.szxytkj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vk.yuexingan06.cn

Java: x instanceof Number
来源：http://sv.haigaiapp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sg.newstarts.cn

Ruby: x.is_a?(Numeric)
来源：http://hj.shtwfgs.cn


<!-- 参考信息 -->