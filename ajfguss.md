代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://gb.yuexingan06.cn

[A03] 常量定义
来源：http://sf.yuntaijiaju.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yp.hahajie.cn

PHP:  const PI = 3.14159;
来源：http://cq.wgjwhj.cn

JS:   const PI = 3.14159;
来源：http://xu.lnxyls.cn

TS:   const PI: number = 3.14159;
来源：http://pf.huixiangedu.cn

Java: static final double PI = 3.14159;
来源：http://ol.shxzukj.cn

Go:   const PI = 3.14159
来源：http://uv.shxzukj.cn

Ruby: PI = 3.14159
来源：http://lk.panjiajie.cn

C#:   const double PI = 3.14159;
来源：http://fq.hahajie.cn

[A04] 判断变量类型
来源：http://dr.yuntaijiaju.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://sz.hahajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pk.muxihuayi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qy.jctech888.com.cn

TS:   typeof x; x instanceof Date
来源：http://fq.hnjuh.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kv.shtwfgs.cn

Go:   reflect.TypeOf(x).Name()
来源：http://tv.521024.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://mb.wgjwhj.cn

C#:   x.GetType().Name; x is int
来源：http://la.hnjuh.cn

[A05] 整数除法与取模
来源：http://od.shxzukj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yz.newstarts.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ta.shxzskj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jf.colortex.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vo.colortex.cn

Java: 7 / 2; 7 % 2
来源：http://dk.chemitech.net.cn

Go:   7 / 2; 7 % 2
来源：http://oo.nicolike.cn

Ruby: 7 / 2; 7 % 2
来源：http://pr.newstarts.cn

C#:   7 / 2; 7 % 2
来源：http://ji.szxytkj.cn

[A06] 字符串转数字
来源：http://tk.nszjky.cn

Py:   int("42"); float("3.14")
来源：http://vp.huixiangedu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ma.huanxung.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kd.gzmigu.cn

TS:   parseInt("42", 10); Number("42")
来源：http://rx.bookmarksfly.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pf.lnxyls.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ht.lnxyls.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fn.szsharing.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ic.521024.cn

[A07] 数字转字符串
来源：http://ma.colortex.cn

Py:   str(42)
来源：http://wv.9csxet.cn

PHP:  (string) 42; strval(42)
来源：http://nv.huixiangedu.cn

JS:   String(42); (42).toString()
来源：http://dk.bookmarksfly.cn

TS:   String(42)
来源：http://wl.chemitech.net.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://hh.wgjwhj.cn

Go:   strconv.Itoa(42)
来源：http://pe.panjiajie.cn

Ruby: 42.to_s
来源：http://ix.colortex.cn

C#:   42.ToString()
来源：http://bf.bjjhwx.cn

[A08] 取整与四舍五入
来源：http://sh.wgjwhj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xx.shtwfgs.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ve.newstarts.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fo.szsharing.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mj.wgjwhj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yr.yuexingan06.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rg.wgjwhj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://wr.huixiangedu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ga.asd995.cn

[A09] 绝对值与最大最小值
来源：http://ea.huixiangedu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dz.lnxyls.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tf.muxihuayi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xn.9csxet.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yu.huixiangedu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ka.shtwfgs.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tz.huanxung.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gk.jianghongdianzi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wp.shxzskj.cn

[A10] 生成随机数
来源：http://dg.shxzskj.cn

Py:   import random; random.randint(1, 100)
来源：http://ky.newstarts.cn

PHP:  random_int(1, 100);
来源：http://io.shtwfgs.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ma.haigaiapp.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://sr.shtwfgs.cn

Java: new Random().nextInt(100) + 1
来源：http://ga.yuntaijiaju.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://uk.colortex.cn

Ruby: rand(1..100)
来源：http://wr.chemitech.net.cn

C#:   new Random().Next(1, 101)
来源：http://by.chemitech.net.cn

[A11] 条件表达式（三元）
来源：http://tm.panjiajie.cn

Py:   "yes" if x > 0 else "no"
来源：http://uo.gzmigu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://pj.9csxet.cn

JS:   x > 0 ? "yes" : "no"
来源：http://fg.wgjwhj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://io.jctech888.com.cn

Java: x > 0 ? "yes" : "no"
来源：http://to.jctech888.com.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://eg.521024.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qc.asd995.cn

C#:   x > 0 ? "yes" : "no"
来源：http://py.jctech888.com.cn

[A12] 字符串插值 / 格式化
来源：http://pa.shxzskj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ve.bookmarksfly.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ya.lnxyls.cn

JS:   `Hello, ${name}!`
来源：http://zb.hnjuh.cn

TS:   `Hello, ${name}!`
来源：http://eh.jctech888.com.cn

Java: "Hello, %s!".formatted(name)
来源：http://ea.jianghongdianzi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://md.jctech888.com.cn

Ruby: "Hello, #{name}!"
来源：http://rr.szsharing.cn

C#:   $"Hello, {name}!"
来源：http://pt.gzmigu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://fs.yuntaijiaju.cn

Py:   "第一行\n第二行"
来源：http://yg.huixiangedu.cn

PHP:  "第一行\n第二行"
来源：http://tr.bookmarksfly.cn

JS:   "第一行\n第二行"
来源：http://we.yuntaijiaju.cn

TS:   "第一行\n第二行"
来源：http://la.lnxyls.cn

Java: "第一行\n第二行"
来源：http://aj.huixiangedu.cn

Go:   "第一行\n第二行"
来源：http://tv.colortex.cn

Ruby: "第一行\n第二行"
来源：http://jq.newstarts.cn

C#:   "第一行\n第二行"
来源：http://fq.chemitech.net.cn

[A14] 注释写法
来源：http://uo.muxihuayi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://qt.shxzukj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://vd.jianghongdianzi.cn

JS:   // 单行；/* 多行 */
来源：http://vp.newstarts.cn

TS:   // 单行；/* 多行 */
来源：http://jr.lnxyls.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://aq.huixiangedu.cn

Go:   // 单行；/* 多行 */
来源：http://xx.lnxyls.cn

Ruby: # 单行；=begin 多行 =end
来源：http://uk.hahajie.cn

C#:   // 单行；/* 多行 */
来源：http://gt.colortex.cn

[A15] 空值判断与默认值
来源：http://xe.huixinmuqiang.cn

Py:   value = data or "默认值"
来源：http://se.nszjky.cn

PHP:  $value = $data ?? "默认值";
来源：http://en.yuexingan06.cn

JS:   const value = data ?? "默认值";
来源：http://zy.asd995.cn

TS:   const value = data ?? "默认值";
来源：http://yi.huixiangedu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dz.shtwfgs.cn

Go:   if data == "" { data = "默认值" }
来源：http://db.hahajie.cn

Ruby: value = data || "默认值"
来源：http://kh.panjiajie.cn

C#:   var value = data ?? "默认值";
来源：http://uz.szsharing.cn

[A16] 真假值判断规则
来源：http://iu.shxzukj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cx.asd995.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vw.colortex.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hd.lnxyls.cn

TS:   if (!x) {}
来源：http://xn.chemitech.net.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://np.shxzskj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jx.huixinmuqiang.cn

Ruby: unless x            # nil 与 false 为假
来源：http://os.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://dm.asd995.cn

[A17] 位运算
来源：http://zt.jianghongdianzi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eq.shtwfgs.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ty.yuntaijiaju.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://od.newstarts.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qc.jianghongdianzi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ge.huixinmuqiang.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mq.nszjky.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hr.panjiajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hl.huixiangedu.cn

[A18] 字符与 ASCII 码互转
来源：http://xv.yuexingan06.cn

Py:   ord("A"); chr(65)
来源：http://ve.bjjhwx.cn

PHP:  ord("A"); chr(65)
来源：http://ts.gzmigu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sc.bookmarksfly.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ap.colortex.cn

Java: (int) 'A'; (char) 65
来源：http://pm.bookmarksfly.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kv.bjjhwx.cn

Ruby: "A".ord; 65.chr
来源：http://ae.521024.cn

C#:   (int)'A'; (char)65
来源：http://di.muxihuayi.cn

[A19] 交换两个变量
来源：http://pd.szxytkj.cn

Py:   a, b = b, a
来源：http://il.shtwfgs.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ha.nicolike.cn

JS:   [a, b] = [b, a];
来源：http://im.shtwfgs.cn

TS:   [a, b] = [b, a];
来源：http://pw.521024.cn

Java: int t = a; a = b; b = t;
来源：http://dc.huixinmuqiang.cn

Go:   a, b = b, a
来源：http://jw.jctech888.com.cn

Ruby: a, b = b, a
来源：http://lu.huanxung.cn

C#:   (a, b) = (b, a);
来源：http://sn.jianghongdianzi.cn

[A20] 读取标准输入
来源：http://ef.muxihuayi.cn

Py:   name = input("请输入：")
来源：http://yw.wgjwhj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://vc.hahajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nz.chemitech.net.cn

TS:   // Node.js：readline 模块
来源：http://jt.asd995.cn

Java: new Scanner(System.in).nextLine()
来源：http://vg.jianghongdianzi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nu.hahajie.cn

Ruby: gets.chomp
来源：http://xk.colortex.cn

C#:   Console.ReadLine();
来源：http://fh.hahajie.cn

[A21] 保留指定小数位输出
来源：http://ty.asd995.cn

Py:   f"{3.14159:.2f}"
来源：http://kh.shxzukj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ji.huixinmuqiang.cn

JS:   (3.14159).toFixed(2)
来源：http://pg.panjiajie.cn

TS:   (3.14159).toFixed(2)
来源：http://mo.asd995.cn

Java: String.format("%.2f", 3.14159)
来源：http://nh.shxzukj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pt.shxzukj.cn

Ruby: format("%.2f", 3.14159)
来源：http://il.colortex.cn

C#:   3.14159.ToString("F2")
来源：http://bh.jianghongdianzi.cn

[A22] 获取字符串长度
来源：http://ji.yuexingan06.cn

Py:   len(s)
来源：http://wn.lnxyls.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wr.shtwfgs.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pe.muxihuayi.cn

TS:   s.length
来源：http://zu.huanxung.cn

Java: s.length()
来源：http://rn.newstarts.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rq.521024.cn

Ruby: s.length
来源：http://jn.wgjwhj.cn

C#:   s.Length
来源：http://ce.nszjky.cn

[A23] 大小写转换
来源：http://lj.bookmarksfly.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://up.asd995.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ad.jctech888.com.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qj.yuexingan06.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jq.jctech888.com.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://uu.jctech888.com.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nx.huixinmuqiang.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mu.jianghongdianzi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://br.521024.cn

[A24] 去除首尾空白
来源：http://zu.jianghongdianzi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ds.shtwfgs.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qi.szsharing.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wt.shtwfgs.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tz.huanxung.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mu.yuntaijiaju.cn

Go:   strings.TrimSpace(s)
来源：http://jn.colortex.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ke.haigaiapp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tw.panjiajie.cn

[A25] 字符串比较
来源：http://qv.szxytkj.cn

Py:   s1 == s2; s1 != s2
来源：http://jw.jctech888.com.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lt.wgjwhj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cr.shxzukj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yd.bjjhwx.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xb.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wi.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yv.colortex.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sc.newstarts.cn

[A26] 类型转换总览
来源：http://nw.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ay.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wy.521024.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fp.nszjky.cn

TS:   Number() String() Boolean() x as number
来源：http://dn.bjjhwx.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yi.szxytkj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wz.nicolike.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ln.bjjhwx.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vg.521024.cn

================================================================================
来源：http://jv.jianghongdianzi.cn

B. 流程控制
来源：http://lv.nicolike.cn

================================================================================
来源：http://ch.chemitech.net.cn

[B01] 条件判断 if / else
来源：http://cw.asd995.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ur.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://on.jianghongdianzi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ba.gzmigu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://th.panjiajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cn.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wf.huanxung.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kb.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xp.nicolike.cn

[B02] 多分支 else if / elif
来源：http://na.asd995.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yq.shxzskj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uy.colortex.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pc.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zy.haigaiapp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gj.newstarts.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hj.gzmigu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://em.newstarts.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hm.huixiangedu.cn

[B03] switch / match / case
来源：http://kc.newstarts.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ud.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sd.szsharing.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rz.jianghongdianzi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rv.9csxet.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ut.jianghongdianzi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mn.shtwfgs.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gt.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tv.szxytkj.cn

[B04] for 计数循环
来源：http://gl.chemitech.net.cn

Py:   for i in range(10): print(i)
来源：http://ql.huixinmuqiang.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pm.bjjhwx.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oc.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://se.jianghongdianzi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://el.hahajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://og.521024.cn

Ruby: 10.times { |i| puts i }
来源：http://ze.shxzukj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ol.chemitech.net.cn

[B05] 遍历数组 / 列表
来源：http://lu.shtwfgs.cn

Py:   for item in arr: print(item)
来源：http://eq.shxzukj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yd.szxytkj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://po.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://md.lnxyls.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vx.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xq.yuexingan06.cn

Ruby: arr.each { |item| puts item }
来源：http://nr.huixiangedu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://us.huanxung.cn

[B06] 遍历字典 / 对象
来源：http://ot.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ti.yuexingan06.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kh.haigaiapp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ap.9csxet.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bt.yuexingan06.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dq.hahajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eo.9csxet.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wk.hnjuh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hm.bjjhwx.cn

[B07] while 循环
来源：http://dq.muxihuayi.cn

Py:   while i < 10: i += 1
来源：http://ul.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://eq.panjiajie.cn

JS:   while (i < 10) { i++; }
来源：http://qx.9csxet.cn

TS:   while (i < 10) { i++; }
来源：http://pg.huanxung.cn

Java: while (i < 10) { i++; }
来源：http://jg.nszjky.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ku.nszjky.cn

Ruby: while i < 10; i += 1; end
来源：http://vy.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://xk.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://le.bjjhwx.cn

Py:   # 无 do-while：用 while True + break
来源：http://kj.lnxyls.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kh.shxzukj.cn

JS:   do { i++; } while (i < 10);
来源：http://gz.huanxung.cn

TS:   do { i++; } while (i < 10);
来源：http://jv.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://vo.shtwfgs.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ue.chemitech.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://le.yuexingan06.cn

C#:   do { i++; } while (i < 10);
来源：http://gg.chemitech.net.cn

[B09] break 与 continue
来源：http://gx.chemitech.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dh.haigaiapp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jl.bjjhwx.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ab.chemitech.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zi.hnjuh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ny.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ic.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uk.yuntaijiaju.cn


<!-- 参考信息 -->