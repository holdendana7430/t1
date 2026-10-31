代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tk.lnxyls.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ok.shxzukj.cn

TS:   typeof x; x instanceof Date
来源：http://lf.huixinmuqiang.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rd.szxytkj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://zd.gzmigu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://pm.hnjuh.cn

C#:   x.GetType().Name; x is int
来源：http://nd.hahajie.cn

[A05] 整数除法与取模
来源：http://qs.huanxung.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://el.huanxung.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://cl.huanxung.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kw.jianghongdianzi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://iv.shtwfgs.cn

Java: 7 / 2; 7 % 2
来源：http://dg.lnxyls.cn

Go:   7 / 2; 7 % 2
来源：http://cv.shtwfgs.cn

Ruby: 7 / 2; 7 % 2
来源：http://jd.newstarts.cn

C#:   7 / 2; 7 % 2
来源：http://vo.lnxyls.cn

[A06] 字符串转数字
来源：http://zd.521024.cn

Py:   int("42"); float("3.14")
来源：http://jk.shtwfgs.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://sy.shxzskj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jg.bookmarksfly.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vl.hahajie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wi.szsharing.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cg.szxytkj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://di.huixinmuqiang.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gc.gzmigu.cn

[A07] 数字转字符串
来源：http://bs.jianghongdianzi.cn

Py:   str(42)
来源：http://di.shxzukj.cn

PHP:  (string) 42; strval(42)
来源：http://rn.shxzukj.cn

JS:   String(42); (42).toString()
来源：http://ue.bjjhwx.cn

TS:   String(42)
来源：http://eo.9csxet.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vd.yuntaijiaju.cn

Go:   strconv.Itoa(42)
来源：http://ey.wgjwhj.cn

Ruby: 42.to_s
来源：http://dw.wgjwhj.cn

C#:   42.ToString()
来源：http://wc.newstarts.cn

[A08] 取整与四舍五入
来源：http://wv.colortex.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ap.wgjwhj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://da.shtwfgs.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ne.bookmarksfly.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jg.hahajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dy.bjjhwx.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xg.521024.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://du.gzmigu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://el.asd995.cn

[A09] 绝对值与最大最小值
来源：http://ki.bookmarksfly.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ie.shxzskj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ii.gzmigu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ko.nicolike.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://oe.nszjky.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xn.asd995.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ov.szsharing.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ay.shtwfgs.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xw.gzmigu.cn

[A10] 生成随机数
来源：http://ra.hahajie.cn

Py:   import random; random.randint(1, 100)
来源：http://ar.huixiangedu.cn

PHP:  random_int(1, 100);
来源：http://kf.yuntaijiaju.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://if.newstarts.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kv.huanxung.cn

Java: new Random().nextInt(100) + 1
来源：http://tc.521024.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yt.chemitech.net.cn

Ruby: rand(1..100)
来源：http://ej.haigaiapp.cn

C#:   new Random().Next(1, 101)
来源：http://wg.9csxet.cn

[A11] 条件表达式（三元）
来源：http://jn.wgjwhj.cn

Py:   "yes" if x > 0 else "no"
来源：http://lt.chemitech.net.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://yy.asd995.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ot.szsharing.cn

TS:   x > 0 ? "yes" : "no"
来源：http://nr.asd995.cn

Java: x > 0 ? "yes" : "no"
来源：http://yi.haigaiapp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ps.shtwfgs.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://rd.lnxyls.cn

C#:   x > 0 ? "yes" : "no"
来源：http://df.szxytkj.cn

[A12] 字符串插值 / 格式化
来源：http://tr.gzmigu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wo.chemitech.net.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hm.nszjky.cn

JS:   `Hello, ${name}!`
来源：http://bp.asd995.cn

TS:   `Hello, ${name}!`
来源：http://ym.newstarts.cn

Java: "Hello, %s!".formatted(name)
来源：http://ku.yuntaijiaju.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zn.newstarts.cn

Ruby: "Hello, #{name}!"
来源：http://xw.wgjwhj.cn

C#:   $"Hello, {name}!"
来源：http://af.asd995.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://zu.yuntaijiaju.cn

Py:   "第一行\n第二行"
来源：http://hj.hnjuh.cn

PHP:  "第一行\n第二行"
来源：http://nl.yuexingan06.cn

JS:   "第一行\n第二行"
来源：http://qz.huixiangedu.cn

TS:   "第一行\n第二行"
来源：http://ga.newstarts.cn

Java: "第一行\n第二行"
来源：http://ue.yuntaijiaju.cn

Go:   "第一行\n第二行"
来源：http://ko.yuexingan06.cn

Ruby: "第一行\n第二行"
来源：http://ur.nszjky.cn

C#:   "第一行\n第二行"
来源：http://fe.colortex.cn

[A14] 注释写法
来源：http://my.gzmigu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://fq.chemitech.net.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://az.muxihuayi.cn

JS:   // 单行；/* 多行 */
来源：http://rj.nszjky.cn

TS:   // 单行；/* 多行 */
来源：http://yw.huanxung.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ip.nicolike.cn

Go:   // 单行；/* 多行 */
来源：http://qw.chemitech.net.cn

Ruby: # 单行；=begin 多行 =end
来源：http://yh.szsharing.cn

C#:   // 单行；/* 多行 */
来源：http://po.hahajie.cn

[A15] 空值判断与默认值
来源：http://jw.jctech888.com.cn

Py:   value = data or "默认值"
来源：http://gm.huixiangedu.cn

PHP:  $value = $data ?? "默认值";
来源：http://lr.jctech888.com.cn

JS:   const value = data ?? "默认值";
来源：http://bt.chemitech.net.cn

TS:   const value = data ?? "默认值";
来源：http://rq.nicolike.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cw.muxihuayi.cn

Go:   if data == "" { data = "默认值" }
来源：http://qc.huixiangedu.cn

Ruby: value = data || "默认值"
来源：http://lv.shxzukj.cn

C#:   var value = data ?? "默认值";
来源：http://eo.panjiajie.cn

[A16] 真假值判断规则
来源：http://uf.bjjhwx.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fo.szsharing.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://to.shxzukj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zr.jctech888.com.cn

TS:   if (!x) {}
来源：http://xp.szxytkj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ir.shxzukj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sn.hahajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://qp.shxzukj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ox.huixiangedu.cn

[A17] 位运算
来源：http://cx.shxzskj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pa.asd995.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nx.shxzskj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sm.nicolike.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hq.huixinmuqiang.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vh.nszjky.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yz.chemitech.net.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tn.chemitech.net.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://no.gzmigu.cn

[A18] 字符与 ASCII 码互转
来源：http://xk.newstarts.cn

Py:   ord("A"); chr(65)
来源：http://be.jianghongdianzi.cn

PHP:  ord("A"); chr(65)
来源：http://jn.newstarts.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yz.bookmarksfly.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sq.nicolike.cn

Java: (int) 'A'; (char) 65
来源：http://ad.huixinmuqiang.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://en.panjiajie.cn

Ruby: "A".ord; 65.chr
来源：http://bj.shxzskj.cn

C#:   (int)'A'; (char)65
来源：http://xb.gzmigu.cn

[A19] 交换两个变量
来源：http://co.panjiajie.cn

Py:   a, b = b, a
来源：http://kn.muxihuayi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yu.shtwfgs.cn

JS:   [a, b] = [b, a];
来源：http://tw.gzmigu.cn

TS:   [a, b] = [b, a];
来源：http://bk.jianghongdianzi.cn

Java: int t = a; a = b; b = t;
来源：http://se.bookmarksfly.cn

Go:   a, b = b, a
来源：http://ch.colortex.cn

Ruby: a, b = b, a
来源：http://ok.9csxet.cn

C#:   (a, b) = (b, a);
来源：http://yo.lnxyls.cn

[A20] 读取标准输入
来源：http://hc.hnjuh.cn

Py:   name = input("请输入：")
来源：http://cp.haigaiapp.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://mh.chemitech.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fo.hnjuh.cn

TS:   // Node.js：readline 模块
来源：http://ax.shtwfgs.cn

Java: new Scanner(System.in).nextLine()
来源：http://ap.nszjky.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rs.lnxyls.cn

Ruby: gets.chomp
来源：http://no.jctech888.com.cn

C#:   Console.ReadLine();
来源：http://hw.jctech888.com.cn

[A21] 保留指定小数位输出
来源：http://rr.shxzukj.cn

Py:   f"{3.14159:.2f}"
来源：http://do.nicolike.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hb.yuexingan06.cn

JS:   (3.14159).toFixed(2)
来源：http://sz.chemitech.net.cn

TS:   (3.14159).toFixed(2)
来源：http://wx.jianghongdianzi.cn

Java: String.format("%.2f", 3.14159)
来源：http://xv.panjiajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://of.shxzskj.cn

Ruby: format("%.2f", 3.14159)
来源：http://ih.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://cg.shxzskj.cn

[A22] 获取字符串长度
来源：http://nk.haigaiapp.cn

Py:   len(s)
来源：http://el.nicolike.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rt.huixiangedu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qq.newstarts.cn

TS:   s.length
来源：http://om.shxzskj.cn

Java: s.length()
来源：http://ep.panjiajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mq.muxihuayi.cn

Ruby: s.length
来源：http://zr.hahajie.cn

C#:   s.Length
来源：http://hh.yuntaijiaju.cn

[A23] 大小写转换
来源：http://dr.jctech888.com.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://go.newstarts.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bh.nicolike.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zv.szsharing.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nw.wgjwhj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cs.jctech888.com.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://iv.hnjuh.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ic.bookmarksfly.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zo.hahajie.cn

[A24] 去除首尾空白
来源：http://bo.lnxyls.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zf.jctech888.com.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ki.colortex.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zv.huixiangedu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cy.wgjwhj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ki.huanxung.cn

Go:   strings.TrimSpace(s)
来源：http://ds.huixiangedu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gy.wgjwhj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://if.huixinmuqiang.cn

[A25] 字符串比较
来源：http://sr.hahajie.cn

Py:   s1 == s2; s1 != s2
来源：http://sx.huanxung.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ep.gzmigu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fx.bookmarksfly.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ut.szsharing.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bh.newstarts.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yh.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ro.yuntaijiaju.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gh.shxzukj.cn

[A26] 类型转换总览
来源：http://on.huixinmuqiang.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sq.muxihuayi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ob.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://px.colortex.cn

TS:   Number() String() Boolean() x as number
来源：http://dm.shtwfgs.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ar.shtwfgs.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ws.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kv.huixinmuqiang.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://no.huanxung.cn

================================================================================
来源：http://om.haigaiapp.cn

B. 流程控制
来源：http://ck.bookmarksfly.cn

================================================================================
来源：http://yu.bookmarksfly.cn

[B01] 条件判断 if / else
来源：http://zd.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ml.521024.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zx.shtwfgs.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mr.muxihuayi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fl.wgjwhj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jh.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cf.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://oc.huanxung.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ig.gzmigu.cn

[B02] 多分支 else if / elif
来源：http://ze.yuntaijiaju.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tn.521024.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fl.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gu.huixinmuqiang.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qo.shtwfgs.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ze.jianghongdianzi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jw.jianghongdianzi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ev.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bk.shxzukj.cn

[B03] switch / match / case
来源：http://tu.chemitech.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sg.huixinmuqiang.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://un.bookmarksfly.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zk.chemitech.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dm.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uo.huixinmuqiang.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nz.asd995.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ad.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jn.hnjuh.cn

[B04] for 计数循环
来源：http://xt.bookmarksfly.cn

Py:   for i in range(10): print(i)
来源：http://ya.szxytkj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ue.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vl.jctech888.com.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://od.jianghongdianzi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://aq.nszjky.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gr.nszjky.cn

Ruby: 10.times { |i| puts i }
来源：http://lu.lnxyls.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ui.bookmarksfly.cn

[B05] 遍历数组 / 列表
来源：http://ly.newstarts.cn

Py:   for item in arr: print(item)
来源：http://sp.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kr.muxihuayi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gp.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vt.jianghongdianzi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rg.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jw.asd995.cn

Ruby: arr.each { |item| puts item }
来源：http://pn.panjiajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uh.lnxyls.cn

[B06] 遍历字典 / 对象
来源：http://ca.lnxyls.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tv.colortex.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mn.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dl.shxzskj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vu.huanxung.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://om.huixiangedu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ck.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://la.asd995.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nr.wgjwhj.cn

[B07] while 循环
来源：http://tg.lnxyls.cn

Py:   while i < 10: i += 1
来源：http://no.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pf.shxzskj.cn

JS:   while (i < 10) { i++; }
来源：http://dx.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://py.haigaiapp.cn

Java: while (i < 10) { i++; }
来源：http://jh.yuexingan06.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dw.chemitech.net.cn

Ruby: while i < 10; i += 1; end
来源：http://mz.shxzukj.cn

C#:   while (i < 10) { i++; }
来源：http://fm.521024.cn

[B08] do-while（至少执行一次）
来源：http://vj.bookmarksfly.cn

Py:   # 无 do-while：用 while True + break
来源：http://nx.szsharing.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ko.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://qj.chemitech.net.cn

TS:   do { i++; } while (i < 10);
来源：http://uh.jctech888.com.cn

Java: do { i++; } while (i < 10);
来源：http://ug.jctech888.com.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hu.lnxyls.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jb.huixinmuqiang.cn

C#:   do { i++; } while (i < 10);
来源：http://rj.szsharing.cn

[B09] break 与 continue
来源：http://ga.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fm.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tq.yuexingan06.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ts.chemitech.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://os.yuexingan06.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rf.chemitech.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ea.shtwfgs.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://la.gzmigu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pu.wgjwhj.cn

[B10] 遍历同时拿索引
来源：http://cf.haigaiapp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vz.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mj.nszjky.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zs.muxihuayi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://aw.huanxung.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uv.nszjky.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mo.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bd.newstarts.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ia.muxihuayi.cn

[B11] 生成数字序列 / 区间
来源：http://nm.newstarts.cn

Py:   list(range(0, 10, 2))
来源：http://gv.nicolike.cn


<!-- 参考信息 -->