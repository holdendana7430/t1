代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lo.9csxet.cn

[A07] 数字转字符串
来源：http://wx.huanxung.cn

Py:   str(42)
来源：http://vw.colortex.cn

PHP:  (string) 42; strval(42)
来源：http://wu.lnxyls.cn

JS:   String(42); (42).toString()
来源：http://su.szsharing.cn

TS:   String(42)
来源：http://xw.yuntaijiaju.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://gg.yuntaijiaju.cn

Go:   strconv.Itoa(42)
来源：http://xw.yuntaijiaju.cn

Ruby: 42.to_s
来源：http://hf.huixinmuqiang.cn

C#:   42.ToString()
来源：http://fi.szxytkj.cn

[A08] 取整与四舍五入
来源：http://eb.lnxyls.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xc.shxzskj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ye.bjjhwx.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xe.panjiajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tw.hnjuh.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qu.muxihuayi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bp.jianghongdianzi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://gl.521024.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://em.szsharing.cn

[A09] 绝对值与最大最小值
来源：http://it.wgjwhj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ec.huanxung.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://sz.jianghongdianzi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gh.shtwfgs.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wg.lnxyls.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bc.shxzukj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://aq.chemitech.net.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vp.shxzukj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qk.shxzskj.cn

[A10] 生成随机数
来源：http://dm.huanxung.cn

Py:   import random; random.randint(1, 100)
来源：http://mb.gzmigu.cn

PHP:  random_int(1, 100);
来源：http://pv.lnxyls.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wd.haigaiapp.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cl.yuexingan06.cn

Java: new Random().nextInt(100) + 1
来源：http://ml.huixinmuqiang.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://so.hnjuh.cn

Ruby: rand(1..100)
来源：http://kd.szsharing.cn

C#:   new Random().Next(1, 101)
来源：http://jr.gzmigu.cn

[A11] 条件表达式（三元）
来源：http://ch.hnjuh.cn

Py:   "yes" if x > 0 else "no"
来源：http://rt.huixinmuqiang.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://fz.shxzukj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ds.hahajie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://en.wgjwhj.cn

Java: x > 0 ? "yes" : "no"
来源：http://zw.szsharing.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://dl.yuexingan06.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://pu.hnjuh.cn

C#:   x > 0 ? "yes" : "no"
来源：http://hs.yuntaijiaju.cn

[A12] 字符串插值 / 格式化
来源：http://hd.gzmigu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nw.szsharing.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ka.huanxung.cn

JS:   `Hello, ${name}!`
来源：http://cq.wgjwhj.cn

TS:   `Hello, ${name}!`
来源：http://jv.huixiangedu.cn

Java: "Hello, %s!".formatted(name)
来源：http://ib.colortex.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kb.newstarts.cn

Ruby: "Hello, #{name}!"
来源：http://ls.panjiajie.cn

C#:   $"Hello, {name}!"
来源：http://om.lnxyls.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://uz.shtwfgs.cn

Py:   "第一行\n第二行"
来源：http://ah.haigaiapp.cn

PHP:  "第一行\n第二行"
来源：http://un.newstarts.cn

JS:   "第一行\n第二行"
来源：http://lv.panjiajie.cn

TS:   "第一行\n第二行"
来源：http://jv.huixiangedu.cn

Java: "第一行\n第二行"
来源：http://hg.huanxung.cn

Go:   "第一行\n第二行"
来源：http://vp.jctech888.com.cn

Ruby: "第一行\n第二行"
来源：http://to.muxihuayi.cn

C#:   "第一行\n第二行"
来源：http://gs.wgjwhj.cn

[A14] 注释写法
来源：http://df.chemitech.net.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://lm.shxzukj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xu.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://hc.yuexingan06.cn

TS:   // 单行；/* 多行 */
来源：http://hv.bookmarksfly.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lc.asd995.cn

Go:   // 单行；/* 多行 */
来源：http://kr.521024.cn

Ruby: # 单行；=begin 多行 =end
来源：http://fi.shxzukj.cn

C#:   // 单行；/* 多行 */
来源：http://ov.jianghongdianzi.cn

[A15] 空值判断与默认值
来源：http://lr.shtwfgs.cn

Py:   value = data or "默认值"
来源：http://py.bjjhwx.cn

PHP:  $value = $data ?? "默认值";
来源：http://ri.wgjwhj.cn

JS:   const value = data ?? "默认值";
来源：http://wd.panjiajie.cn

TS:   const value = data ?? "默认值";
来源：http://dw.szsharing.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://se.shtwfgs.cn

Go:   if data == "" { data = "默认值" }
来源：http://ib.panjiajie.cn

Ruby: value = data || "默认值"
来源：http://mj.haigaiapp.cn

C#:   var value = data ?? "默认值";
来源：http://fa.shtwfgs.cn

[A16] 真假值判断规则
来源：http://ga.panjiajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ak.hnjuh.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bv.hnjuh.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sh.szsharing.cn

TS:   if (!x) {}
来源：http://vu.panjiajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rh.hahajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hh.newstarts.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ay.gzmigu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kn.hnjuh.cn

[A17] 位运算
来源：http://pn.colortex.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zo.nszjky.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qo.gzmigu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wb.hahajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zw.hahajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hv.szsharing.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wb.szsharing.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kr.nszjky.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://on.nicolike.cn

[A18] 字符与 ASCII 码互转
来源：http://jh.nszjky.cn

Py:   ord("A"); chr(65)
来源：http://sm.jctech888.com.cn

PHP:  ord("A"); chr(65)
来源：http://af.jctech888.com.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ah.huixinmuqiang.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://je.shtwfgs.cn

Java: (int) 'A'; (char) 65
来源：http://ye.muxihuayi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ok.gzmigu.cn

Ruby: "A".ord; 65.chr
来源：http://wt.nszjky.cn

C#:   (int)'A'; (char)65
来源：http://jt.nszjky.cn

[A19] 交换两个变量
来源：http://iy.asd995.cn

Py:   a, b = b, a
来源：http://my.wgjwhj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://dm.szxytkj.cn

JS:   [a, b] = [b, a];
来源：http://op.newstarts.cn

TS:   [a, b] = [b, a];
来源：http://rp.521024.cn

Java: int t = a; a = b; b = t;
来源：http://ks.lnxyls.cn

Go:   a, b = b, a
来源：http://vt.bookmarksfly.cn

Ruby: a, b = b, a
来源：http://yb.yuexingan06.cn

C#:   (a, b) = (b, a);
来源：http://om.colortex.cn

[A20] 读取标准输入
来源：http://rn.jctech888.com.cn

Py:   name = input("请输入：")
来源：http://vl.jctech888.com.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://dq.colortex.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yp.nicolike.cn

TS:   // Node.js：readline 模块
来源：http://tb.jctech888.com.cn

Java: new Scanner(System.in).nextLine()
来源：http://rg.521024.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kc.chemitech.net.cn

Ruby: gets.chomp
来源：http://xv.bjjhwx.cn

C#:   Console.ReadLine();
来源：http://mv.lnxyls.cn

[A21] 保留指定小数位输出
来源：http://ql.hnjuh.cn

Py:   f"{3.14159:.2f}"
来源：http://vq.haigaiapp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qt.wgjwhj.cn

JS:   (3.14159).toFixed(2)
来源：http://fg.nicolike.cn

TS:   (3.14159).toFixed(2)
来源：http://hq.chemitech.net.cn

Java: String.format("%.2f", 3.14159)
来源：http://ce.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://op.gzmigu.cn

Ruby: format("%.2f", 3.14159)
来源：http://lo.muxihuayi.cn

C#:   3.14159.ToString("F2")
来源：http://rq.huixinmuqiang.cn

[A22] 获取字符串长度
来源：http://es.shtwfgs.cn

Py:   len(s)
来源：http://og.wgjwhj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rx.shxzukj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://id.szsharing.cn

TS:   s.length
来源：http://rh.jianghongdianzi.cn

Java: s.length()
来源：http://xq.521024.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kr.nszjky.cn

Ruby: s.length
来源：http://jy.nszjky.cn

C#:   s.Length
来源：http://fq.shxzskj.cn

[A23] 大小写转换
来源：http://mx.hnjuh.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ny.chemitech.net.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://uk.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zq.szxytkj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xc.chemitech.net.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zj.bjjhwx.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hj.huixiangedu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wf.nszjky.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://yx.colortex.cn

[A24] 去除首尾空白
来源：http://vv.asd995.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://er.nszjky.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mu.jianghongdianzi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xb.jianghongdianzi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gi.shtwfgs.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pe.jianghongdianzi.cn

Go:   strings.TrimSpace(s)
来源：http://uo.yuntaijiaju.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ue.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ty.lnxyls.cn

[A25] 字符串比较
来源：http://iv.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://rn.chemitech.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qg.szxytkj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sq.shxzukj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gc.shtwfgs.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jw.521024.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kj.asd995.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mi.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://au.jianghongdianzi.cn

[A26] 类型转换总览
来源：http://nm.gzmigu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qq.yuexingan06.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jy.nicolike.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zd.huixiangedu.cn

TS:   Number() String() Boolean() x as number
来源：http://ag.9csxet.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://os.yuexingan06.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ur.lnxyls.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ha.panjiajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://er.gzmigu.cn

================================================================================
来源：http://bp.bookmarksfly.cn

B. 流程控制
来源：http://gm.shxzukj.cn

================================================================================
来源：http://ro.hahajie.cn

[B01] 条件判断 if / else
来源：http://pj.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vu.szxytkj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yf.szxytkj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://um.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kn.szsharing.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pw.hahajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yl.jianghongdianzi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nt.huixiangedu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jp.wgjwhj.cn

[B02] 多分支 else if / elif
来源：http://lv.chemitech.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lh.huixiangedu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xf.yuntaijiaju.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dt.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://si.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mt.9csxet.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ho.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://im.shxzukj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cw.jianghongdianzi.cn

[B03] switch / match / case
来源：http://fm.lnxyls.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bb.shxzukj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ro.haigaiapp.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kt.asd995.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gk.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ev.huixiangedu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jm.yuntaijiaju.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rx.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ro.bjjhwx.cn

[B04] for 计数循环
来源：http://an.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://ok.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://we.9csxet.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lo.gzmigu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kh.jianghongdianzi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zr.yuntaijiaju.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qp.521024.cn

Ruby: 10.times { |i| puts i }
来源：http://oc.yuntaijiaju.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rp.9csxet.cn

[B05] 遍历数组 / 列表
来源：http://ug.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://kx.bjjhwx.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gb.asd995.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ev.colortex.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jd.shxzskj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jm.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qh.chemitech.net.cn

Ruby: arr.each { |item| puts item }
来源：http://gn.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pg.lnxyls.cn

[B06] 遍历字典 / 对象
来源：http://yk.lnxyls.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ng.gzmigu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pi.haigaiapp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ev.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tj.hnjuh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sa.521024.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://am.muxihuayi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lv.szxytkj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ol.nicolike.cn

[B07] while 循环
来源：http://hz.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://pc.chemitech.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://sf.huixinmuqiang.cn

JS:   while (i < 10) { i++; }
来源：http://os.huixinmuqiang.cn

TS:   while (i < 10) { i++; }
来源：http://qa.yuexingan06.cn

Java: while (i < 10) { i++; }
来源：http://jv.shtwfgs.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oz.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://dw.shxzukj.cn

C#:   while (i < 10) { i++; }
来源：http://to.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://ch.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://jt.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zu.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://uz.bookmarksfly.cn

TS:   do { i++; } while (i < 10);
来源：http://dq.yuntaijiaju.cn

Java: do { i++; } while (i < 10);
来源：http://bq.hahajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xn.muxihuayi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vy.huixiangedu.cn

C#:   do { i++; } while (i < 10);
来源：http://gs.yuexingan06.cn

[B09] break 与 continue
来源：http://um.wgjwhj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gf.gzmigu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://it.szsharing.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jn.szsharing.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ob.9csxet.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ef.shxzskj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jl.newstarts.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rz.lnxyls.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aj.bookmarksfly.cn

[B10] 遍历同时拿索引
来源：http://ht.szsharing.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pz.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mm.yuntaijiaju.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ui.jctech888.com.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://by.panjiajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bn.chemitech.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gw.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ia.lnxyls.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://al.huixiangedu.cn

[B11] 生成数字序列 / 区间
来源：http://qb.shxzskj.cn

Py:   list(range(0, 10, 2))
来源：http://sp.lnxyls.cn

PHP:  range(0, 10, 2);
来源：http://qo.yuntaijiaju.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ym.hahajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sr.shxzskj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vg.huanxung.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zp.lnxyls.cn

Ruby: (0...10).step(2).to_a
来源：http://pm.asd995.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hd.asd995.cn

[B12] 跳出多层循环
来源：http://ck.521024.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gn.panjiajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hd.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://os.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://in.szxytkj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nk.hahajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cq.huixiangedu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sh.bookmarksfly.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nv.panjiajie.cn

[B13] 判断是否为数字
来源：http://yk.bjjhwx.cn

Py:   isinstance(x, (int, float))
来源：http://ee.huanxung.cn

PHP:  is_numeric($x)
来源：http://pc.gzmigu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jq.chemitech.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bt.colortex.cn

Java: x instanceof Number
来源：http://yi.panjiajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uj.huanxung.cn

Ruby: x.is_a?(Numeric)
来源：http://ad.yuexingan06.cn


<!-- 参考信息 -->