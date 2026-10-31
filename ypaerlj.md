代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qv.lnxyls.cn

Java: String name = "Alex"; int age = 20;
来源：http://vm.shxzskj.cn

Go:   name := "Alex"; age := 20
来源：http://cp.panjiajie.cn

Ruby: name = "Alex"; age = 20
来源：http://bp.huixiangedu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://td.haigaiapp.cn

[A03] 常量定义
来源：http://au.hnjuh.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qv.jctech888.com.cn

PHP:  const PI = 3.14159;
来源：http://kq.bookmarksfly.cn

JS:   const PI = 3.14159;
来源：http://kh.huixinmuqiang.cn

TS:   const PI: number = 3.14159;
来源：http://yf.jctech888.com.cn

Java: static final double PI = 3.14159;
来源：http://ic.asd995.cn

Go:   const PI = 3.14159
来源：http://vy.wgjwhj.cn

Ruby: PI = 3.14159
来源：http://yf.shxzukj.cn

C#:   const double PI = 3.14159;
来源：http://xk.lnxyls.cn

[A04] 判断变量类型
来源：http://is.9csxet.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hw.huanxung.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vv.521024.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://uu.shtwfgs.cn

TS:   typeof x; x instanceof Date
来源：http://oh.shtwfgs.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hr.szxytkj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://wh.shtwfgs.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://xb.muxihuayi.cn

C#:   x.GetType().Name; x is int
来源：http://ki.lnxyls.cn

[A05] 整数除法与取模
来源：http://jc.muxihuayi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fv.colortex.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://jh.shxzukj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xi.haigaiapp.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qz.hahajie.cn

Java: 7 / 2; 7 % 2
来源：http://bw.yuexingan06.cn

Go:   7 / 2; 7 % 2
来源：http://sw.jianghongdianzi.cn

Ruby: 7 / 2; 7 % 2
来源：http://ke.huixinmuqiang.cn

C#:   7 / 2; 7 % 2
来源：http://mo.yuntaijiaju.cn

[A06] 字符串转数字
来源：http://ta.asd995.cn

Py:   int("42"); float("3.14")
来源：http://vs.shxzukj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ty.huanxung.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tl.hnjuh.cn

TS:   parseInt("42", 10); Number("42")
来源：http://id.shxzukj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xp.huixinmuqiang.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wo.haigaiapp.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://jv.huixiangedu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xm.gzmigu.cn

[A07] 数字转字符串
来源：http://qw.shxzukj.cn

Py:   str(42)
来源：http://ow.shxzskj.cn

PHP:  (string) 42; strval(42)
来源：http://gj.haigaiapp.cn

JS:   String(42); (42).toString()
来源：http://gu.bjjhwx.cn

TS:   String(42)
来源：http://za.wgjwhj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ld.wgjwhj.cn

Go:   strconv.Itoa(42)
来源：http://lp.huixinmuqiang.cn

Ruby: 42.to_s
来源：http://gr.szxytkj.cn

C#:   42.ToString()
来源：http://ip.haigaiapp.cn

[A08] 取整与四舍五入
来源：http://ih.shtwfgs.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://af.nicolike.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dn.szxytkj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://cs.lnxyls.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wv.shxzskj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dh.panjiajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dk.muxihuayi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://yk.nszjky.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://at.nicolike.cn

[A09] 绝对值与最大最小值
来源：http://ag.nicolike.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ra.newstarts.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://am.hnjuh.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bs.gzmigu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gj.szsharing.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zq.huixinmuqiang.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ev.shxzukj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qd.bjjhwx.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://li.jctech888.com.cn

[A10] 生成随机数
来源：http://kp.lnxyls.cn

Py:   import random; random.randint(1, 100)
来源：http://td.gzmigu.cn

PHP:  random_int(1, 100);
来源：http://dx.shxzskj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sk.hnjuh.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hx.jctech888.com.cn

Java: new Random().nextInt(100) + 1
来源：http://it.gzmigu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://md.newstarts.cn

Ruby: rand(1..100)
来源：http://ht.colortex.cn

C#:   new Random().Next(1, 101)
来源：http://oh.colortex.cn

[A11] 条件表达式（三元）
来源：http://ri.szsharing.cn

Py:   "yes" if x > 0 else "no"
来源：http://mg.asd995.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://gy.shxzskj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://yq.wgjwhj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://yt.yuexingan06.cn

Java: x > 0 ? "yes" : "no"
来源：http://lc.9csxet.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://gb.521024.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://yi.panjiajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ma.jctech888.com.cn

[A12] 字符串插值 / 格式化
来源：http://ru.newstarts.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qz.huixinmuqiang.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zd.jctech888.com.cn

JS:   `Hello, ${name}!`
来源：http://jb.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://ku.newstarts.cn

Java: "Hello, %s!".formatted(name)
来源：http://dk.chemitech.net.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://lm.shxzskj.cn

Ruby: "Hello, #{name}!"
来源：http://jl.yuexingan06.cn

C#:   $"Hello, {name}!"
来源：http://nv.muxihuayi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://nm.bookmarksfly.cn

Py:   "第一行\n第二行"
来源：http://vu.jctech888.com.cn

PHP:  "第一行\n第二行"
来源：http://vc.lnxyls.cn

JS:   "第一行\n第二行"
来源：http://rv.lnxyls.cn

TS:   "第一行\n第二行"
来源：http://qo.wgjwhj.cn

Java: "第一行\n第二行"
来源：http://ns.huixinmuqiang.cn

Go:   "第一行\n第二行"
来源：http://ar.jianghongdianzi.cn

Ruby: "第一行\n第二行"
来源：http://iu.yuexingan06.cn

C#:   "第一行\n第二行"
来源：http://nm.muxihuayi.cn

[A14] 注释写法
来源：http://bn.asd995.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pd.bookmarksfly.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://rb.jianghongdianzi.cn

JS:   // 单行；/* 多行 */
来源：http://gj.wgjwhj.cn

TS:   // 单行；/* 多行 */
来源：http://sq.wgjwhj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tr.colortex.cn

Go:   // 单行；/* 多行 */
来源：http://ak.shxzukj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://rr.muxihuayi.cn

C#:   // 单行；/* 多行 */
来源：http://zt.9csxet.cn

[A15] 空值判断与默认值
来源：http://mw.hahajie.cn

Py:   value = data or "默认值"
来源：http://ni.newstarts.cn

PHP:  $value = $data ?? "默认值";
来源：http://zb.jianghongdianzi.cn

JS:   const value = data ?? "默认值";
来源：http://ny.nszjky.cn

TS:   const value = data ?? "默认值";
来源：http://hx.haigaiapp.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zx.huixiangedu.cn

Go:   if data == "" { data = "默认值" }
来源：http://rq.shxzskj.cn

Ruby: value = data || "默认值"
来源：http://xi.muxihuayi.cn

C#:   var value = data ?? "默认值";
来源：http://bv.jctech888.com.cn

[A16] 真假值判断规则
来源：http://hl.haigaiapp.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://oj.huixiangedu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://li.yuexingan06.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://di.asd995.cn

TS:   if (!x) {}
来源：http://vi.huixinmuqiang.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rf.chemitech.net.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ln.hahajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://fo.lnxyls.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pt.newstarts.cn

[A17] 位运算
来源：http://lw.gzmigu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uk.szsharing.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bo.colortex.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fc.shtwfgs.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ow.lnxyls.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xb.hnjuh.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://od.shtwfgs.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xj.szsharing.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cb.gzmigu.cn

[A18] 字符与 ASCII 码互转
来源：http://iy.lnxyls.cn

Py:   ord("A"); chr(65)
来源：http://dq.521024.cn

PHP:  ord("A"); chr(65)
来源：http://hs.asd995.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dw.wgjwhj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ep.jianghongdianzi.cn

Java: (int) 'A'; (char) 65
来源：http://cu.hnjuh.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yb.wgjwhj.cn

Ruby: "A".ord; 65.chr
来源：http://yo.hahajie.cn

C#:   (int)'A'; (char)65
来源：http://uo.521024.cn

[A19] 交换两个变量
来源：http://cd.bjjhwx.cn

Py:   a, b = b, a
来源：http://gl.shtwfgs.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://eu.szsharing.cn

JS:   [a, b] = [b, a];
来源：http://ea.shxzukj.cn

TS:   [a, b] = [b, a];
来源：http://oo.nicolike.cn

Java: int t = a; a = b; b = t;
来源：http://pb.newstarts.cn

Go:   a, b = b, a
来源：http://hd.haigaiapp.cn

Ruby: a, b = b, a
来源：http://qq.jctech888.com.cn

C#:   (a, b) = (b, a);
来源：http://pi.shxzskj.cn

[A20] 读取标准输入
来源：http://gq.bookmarksfly.cn

Py:   name = input("请输入：")
来源：http://qg.muxihuayi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://nf.bjjhwx.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://em.521024.cn

TS:   // Node.js：readline 模块
来源：http://gf.szxytkj.cn

Java: new Scanner(System.in).nextLine()
来源：http://mc.shxzskj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jb.hnjuh.cn

Ruby: gets.chomp
来源：http://my.yuexingan06.cn

C#:   Console.ReadLine();
来源：http://gg.hnjuh.cn

[A21] 保留指定小数位输出
来源：http://xu.hahajie.cn

Py:   f"{3.14159:.2f}"
来源：http://mv.shxzukj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kw.nicolike.cn

JS:   (3.14159).toFixed(2)
来源：http://sl.521024.cn

TS:   (3.14159).toFixed(2)
来源：http://fm.gzmigu.cn

Java: String.format("%.2f", 3.14159)
来源：http://zu.9csxet.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rc.wgjwhj.cn

Ruby: format("%.2f", 3.14159)
来源：http://fu.huixiangedu.cn

C#:   3.14159.ToString("F2")
来源：http://ns.shxzskj.cn

[A22] 获取字符串长度
来源：http://gy.colortex.cn

Py:   len(s)
来源：http://uv.shxzukj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ef.shtwfgs.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xa.shtwfgs.cn

TS:   s.length
来源：http://tq.521024.cn

Java: s.length()
来源：http://pe.hahajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ae.shtwfgs.cn

Ruby: s.length
来源：http://bl.colortex.cn

C#:   s.Length
来源：http://rk.colortex.cn

[A23] 大小写转换
来源：http://ki.szsharing.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://lz.jctech888.com.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ii.muxihuayi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tk.szsharing.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sx.9csxet.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ct.muxihuayi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tv.huixinmuqiang.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rd.shxzukj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://db.colortex.cn

[A24] 去除首尾空白
来源：http://fs.nszjky.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xw.muxihuayi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ly.wgjwhj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zq.wgjwhj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ex.gzmigu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bb.muxihuayi.cn

Go:   strings.TrimSpace(s)
来源：http://wx.hnjuh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://de.nszjky.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rw.hahajie.cn

[A25] 字符串比较
来源：http://yh.shtwfgs.cn

Py:   s1 == s2; s1 != s2
来源：http://yo.shxzukj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ns.colortex.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rl.bookmarksfly.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://br.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vk.haigaiapp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zb.yuexingan06.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://sp.chemitech.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tv.yuexingan06.cn

[A26] 类型转换总览
来源：http://xq.shtwfgs.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xv.nicolike.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ie.huixinmuqiang.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://go.asd995.cn

TS:   Number() String() Boolean() x as number
来源：http://gj.bookmarksfly.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ux.shtwfgs.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ta.hnjuh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://tm.gzmigu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://al.szsharing.cn

================================================================================
来源：http://qf.huanxung.cn

B. 流程控制
来源：http://fl.shtwfgs.cn

================================================================================
来源：http://qs.shxzukj.cn

[B01] 条件判断 if / else
来源：http://go.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xo.nszjky.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ka.hahajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ch.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fx.gzmigu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ft.bookmarksfly.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gz.yuexingan06.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ux.asd995.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yy.huanxung.cn

[B02] 多分支 else if / elif
来源：http://oe.panjiajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tr.colortex.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bl.yuntaijiaju.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fp.hahajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fu.asd995.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ck.hnjuh.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dm.nszjky.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yb.bjjhwx.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rp.muxihuayi.cn

[B03] switch / match / case
来源：http://px.huanxung.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ck.hnjuh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ny.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qq.jianghongdianzi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://so.bjjhwx.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uf.huixiangedu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ib.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dz.muxihuayi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vv.shxzukj.cn

[B04] for 计数循环
来源：http://zg.bjjhwx.cn

Py:   for i in range(10): print(i)
来源：http://af.wgjwhj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rt.shtwfgs.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sz.jctech888.com.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hj.bookmarksfly.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ty.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wa.wgjwhj.cn

Ruby: 10.times { |i| puts i }
来源：http://sg.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fx.colortex.cn

[B05] 遍历数组 / 列表
来源：http://yn.shtwfgs.cn

Py:   for item in arr: print(item)
来源：http://wb.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://md.shxzukj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://oh.bjjhwx.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jt.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://iy.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://st.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://bz.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gy.huixinmuqiang.cn

[B06] 遍历字典 / 对象
来源：http://fe.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hu.wgjwhj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ed.muxihuayi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wh.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rj.muxihuayi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qt.huanxung.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ip.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ul.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://go.521024.cn

[B07] while 循环
来源：http://kp.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://cy.shxzukj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://sf.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://dc.lnxyls.cn

TS:   while (i < 10) { i++; }
来源：http://oh.hahajie.cn

Java: while (i < 10) { i++; }
来源：http://te.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ix.hahajie.cn

Ruby: while i < 10; i += 1; end
来源：http://ba.panjiajie.cn

C#:   while (i < 10) { i++; }
来源：http://br.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://wh.bookmarksfly.cn

Py:   # 无 do-while：用 while True + break
来源：http://cz.shxzukj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ni.newstarts.cn

JS:   do { i++; } while (i < 10);
来源：http://wu.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://sl.hahajie.cn

Java: do { i++; } while (i < 10);
来源：http://ar.jianghongdianzi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nd.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mm.wgjwhj.cn

C#:   do { i++; } while (i < 10);
来源：http://kb.newstarts.cn

[B09] break 与 continue
来源：http://dk.muxihuayi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wt.huanxung.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qz.wgjwhj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pw.huixinmuqiang.cn


<!-- 参考信息 -->