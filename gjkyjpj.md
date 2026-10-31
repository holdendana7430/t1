代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://dt.hahajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://ks.huixiangedu.cn

Ruby: puts "Hello, World!"
来源：http://bn.nicolike.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://yt.panjiajie.cn

[A02] 变量声明与赋值
来源：http://ge.521024.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lg.yuexingan06.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://of.huixinmuqiang.cn

JS:   let name = "Alex"; const age = 20;
来源：http://bs.gzmigu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lb.nszjky.cn

Java: String name = "Alex"; int age = 20;
来源：http://vk.huixiangedu.cn

Go:   name := "Alex"; age := 20
来源：http://hb.haigaiapp.cn

Ruby: name = "Alex"; age = 20
来源：http://pa.asd995.cn

C#:   string name = "Alex"; int age = 20;
来源：http://tu.huanxung.cn

[A03] 常量定义
来源：http://lo.shxzskj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tq.huanxung.cn

PHP:  const PI = 3.14159;
来源：http://uo.shxzskj.cn

JS:   const PI = 3.14159;
来源：http://yr.jctech888.com.cn

TS:   const PI: number = 3.14159;
来源：http://uq.lnxyls.cn

Java: static final double PI = 3.14159;
来源：http://bc.bookmarksfly.cn

Go:   const PI = 3.14159
来源：http://hf.asd995.cn

Ruby: PI = 3.14159
来源：http://vr.shtwfgs.cn

C#:   const double PI = 3.14159;
来源：http://sr.yuexingan06.cn

[A04] 判断变量类型
来源：http://jv.colortex.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://aj.521024.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hx.yuexingan06.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jz.yuntaijiaju.cn

TS:   typeof x; x instanceof Date
来源：http://td.hahajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://sl.nicolike.cn

Go:   reflect.TypeOf(x).Name()
来源：http://mq.chemitech.net.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gy.huanxung.cn

C#:   x.GetType().Name; x is int
来源：http://ie.lnxyls.cn

[A05] 整数除法与取模
来源：http://zf.9csxet.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ge.haigaiapp.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ys.hahajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://me.bjjhwx.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kw.nicolike.cn

Java: 7 / 2; 7 % 2
来源：http://th.huixiangedu.cn

Go:   7 / 2; 7 % 2
来源：http://xn.shxzskj.cn

Ruby: 7 / 2; 7 % 2
来源：http://dl.9csxet.cn

C#:   7 / 2; 7 % 2
来源：http://jj.nicolike.cn

[A06] 字符串转数字
来源：http://cc.chemitech.net.cn

Py:   int("42"); float("3.14")
来源：http://pm.colortex.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://px.muxihuayi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://it.bookmarksfly.cn

TS:   parseInt("42", 10); Number("42")
来源：http://oh.shtwfgs.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://aj.hahajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ia.jctech888.com.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zt.shxzukj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://si.panjiajie.cn

[A07] 数字转字符串
来源：http://sd.muxihuayi.cn

Py:   str(42)
来源：http://da.chemitech.net.cn

PHP:  (string) 42; strval(42)
来源：http://eh.huixiangedu.cn

JS:   String(42); (42).toString()
来源：http://qa.wgjwhj.cn

TS:   String(42)
来源：http://ej.bookmarksfly.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://eu.huanxung.cn

Go:   strconv.Itoa(42)
来源：http://dk.hahajie.cn

Ruby: 42.to_s
来源：http://rl.haigaiapp.cn

C#:   42.ToString()
来源：http://uz.gzmigu.cn

[A08] 取整与四舍五入
来源：http://mh.yuntaijiaju.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tu.huanxung.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ue.bjjhwx.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xq.521024.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cd.9csxet.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rp.szsharing.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lz.yuntaijiaju.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://bo.lnxyls.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ku.haigaiapp.cn

[A09] 绝对值与最大最小值
来源：http://cn.muxihuayi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pt.muxihuayi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ck.szxytkj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zw.panjiajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kx.jctech888.com.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qz.shxzukj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://li.asd995.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lq.huixiangedu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jy.lnxyls.cn

[A10] 生成随机数
来源：http://kj.yuntaijiaju.cn

Py:   import random; random.randint(1, 100)
来源：http://ut.nicolike.cn

PHP:  random_int(1, 100);
来源：http://hq.szsharing.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rz.gzmigu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://pj.jctech888.com.cn

Java: new Random().nextInt(100) + 1
来源：http://xd.bookmarksfly.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dc.yuntaijiaju.cn

Ruby: rand(1..100)
来源：http://ac.shtwfgs.cn

C#:   new Random().Next(1, 101)
来源：http://es.chemitech.net.cn

[A11] 条件表达式（三元）
来源：http://ld.colortex.cn

Py:   "yes" if x > 0 else "no"
来源：http://dl.colortex.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ko.wgjwhj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pm.wgjwhj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://pp.shxzukj.cn

Java: x > 0 ? "yes" : "no"
来源：http://wz.colortex.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://sl.bookmarksfly.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://nq.nszjky.cn

C#:   x > 0 ? "yes" : "no"
来源：http://sx.huanxung.cn

[A12] 字符串插值 / 格式化
来源：http://er.jianghongdianzi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wm.wgjwhj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ik.szsharing.cn

JS:   `Hello, ${name}!`
来源：http://nj.shxzukj.cn

TS:   `Hello, ${name}!`
来源：http://xs.shxzskj.cn

Java: "Hello, %s!".formatted(name)
来源：http://iv.huixiangedu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sp.newstarts.cn

Ruby: "Hello, #{name}!"
来源：http://vl.asd995.cn

C#:   $"Hello, {name}!"
来源：http://dk.huixinmuqiang.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hr.huanxung.cn

Py:   "第一行\n第二行"
来源：http://xd.huanxung.cn

PHP:  "第一行\n第二行"
来源：http://yk.huanxung.cn

JS:   "第一行\n第二行"
来源：http://oa.shxzskj.cn

TS:   "第一行\n第二行"
来源：http://fz.colortex.cn

Java: "第一行\n第二行"
来源：http://ez.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://ye.shtwfgs.cn

Ruby: "第一行\n第二行"
来源：http://pm.wgjwhj.cn

C#:   "第一行\n第二行"
来源：http://kb.nszjky.cn

[A14] 注释写法
来源：http://rc.yuexingan06.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://df.chemitech.net.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ko.wgjwhj.cn

JS:   // 单行；/* 多行 */
来源：http://sz.asd995.cn

TS:   // 单行；/* 多行 */
来源：http://kv.jianghongdianzi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mt.jctech888.com.cn

Go:   // 单行；/* 多行 */
来源：http://vm.bookmarksfly.cn

Ruby: # 单行；=begin 多行 =end
来源：http://bi.shtwfgs.cn

C#:   // 单行；/* 多行 */
来源：http://ip.shxzskj.cn

[A15] 空值判断与默认值
来源：http://yc.shtwfgs.cn

Py:   value = data or "默认值"
来源：http://zg.newstarts.cn

PHP:  $value = $data ?? "默认值";
来源：http://vz.huanxung.cn

JS:   const value = data ?? "默认值";
来源：http://cd.521024.cn

TS:   const value = data ?? "默认值";
来源：http://go.bjjhwx.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bj.huixiangedu.cn

Go:   if data == "" { data = "默认值" }
来源：http://av.lnxyls.cn

Ruby: value = data || "默认值"
来源：http://oh.huanxung.cn

C#:   var value = data ?? "默认值";
来源：http://om.jianghongdianzi.cn

[A16] 真假值判断规则
来源：http://rw.yuntaijiaju.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yw.huixinmuqiang.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nc.szxytkj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vm.yuexingan06.cn

TS:   if (!x) {}
来源：http://vs.muxihuayi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yb.shtwfgs.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mu.huixiangedu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://nw.panjiajie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gt.shtwfgs.cn

[A17] 位运算
来源：http://ct.shxzukj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jv.bjjhwx.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uh.panjiajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mw.bookmarksfly.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wd.chemitech.net.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://me.lnxyls.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dn.szsharing.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kn.lnxyls.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ok.colortex.cn

[A18] 字符与 ASCII 码互转
来源：http://nz.haigaiapp.cn

Py:   ord("A"); chr(65)
来源：http://vd.shxzskj.cn

PHP:  ord("A"); chr(65)
来源：http://ub.bookmarksfly.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gi.huixiangedu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qb.bookmarksfly.cn

Java: (int) 'A'; (char) 65
来源：http://hk.huixinmuqiang.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://az.gzmigu.cn

Ruby: "A".ord; 65.chr
来源：http://tc.jianghongdianzi.cn

C#:   (int)'A'; (char)65
来源：http://xz.bookmarksfly.cn

[A19] 交换两个变量
来源：http://ux.colortex.cn

Py:   a, b = b, a
来源：http://al.shxzskj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fr.nicolike.cn

JS:   [a, b] = [b, a];
来源：http://oa.muxihuayi.cn

TS:   [a, b] = [b, a];
来源：http://kg.szxytkj.cn

Java: int t = a; a = b; b = t;
来源：http://ra.huixiangedu.cn

Go:   a, b = b, a
来源：http://ei.panjiajie.cn

Ruby: a, b = b, a
来源：http://lh.hnjuh.cn

C#:   (a, b) = (b, a);
来源：http://gs.huixinmuqiang.cn

[A20] 读取标准输入
来源：http://ym.hnjuh.cn

Py:   name = input("请输入：")
来源：http://gp.colortex.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://nh.chemitech.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ck.yuexingan06.cn

TS:   // Node.js：readline 模块
来源：http://fm.shxzukj.cn

Java: new Scanner(System.in).nextLine()
来源：http://ca.wgjwhj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ie.panjiajie.cn

Ruby: gets.chomp
来源：http://lu.chemitech.net.cn

C#:   Console.ReadLine();
来源：http://fm.muxihuayi.cn

[A21] 保留指定小数位输出
来源：http://ke.shxzskj.cn

Py:   f"{3.14159:.2f}"
来源：http://gl.muxihuayi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://is.jctech888.com.cn

JS:   (3.14159).toFixed(2)
来源：http://go.asd995.cn

TS:   (3.14159).toFixed(2)
来源：http://pd.9csxet.cn

Java: String.format("%.2f", 3.14159)
来源：http://nr.jianghongdianzi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vc.shxzukj.cn

Ruby: format("%.2f", 3.14159)
来源：http://xo.huanxung.cn

C#:   3.14159.ToString("F2")
来源：http://tb.hahajie.cn

[A22] 获取字符串长度
来源：http://sh.yuntaijiaju.cn

Py:   len(s)
来源：http://zp.9csxet.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lf.yuexingan06.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zk.shxzukj.cn

TS:   s.length
来源：http://oy.colortex.cn

Java: s.length()
来源：http://vt.gzmigu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sx.haigaiapp.cn

Ruby: s.length
来源：http://cd.muxihuayi.cn

C#:   s.Length
来源：http://ki.huixiangedu.cn

[A23] 大小写转换
来源：http://bh.asd995.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fl.nszjky.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://le.huixiangedu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jf.nszjky.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lr.hnjuh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nn.shxzskj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ia.panjiajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uc.huixiangedu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ic.chemitech.net.cn

[A24] 去除首尾空白
来源：http://mq.yuexingan06.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://at.yuexingan06.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xf.lnxyls.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xq.chemitech.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rg.colortex.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yc.newstarts.cn

Go:   strings.TrimSpace(s)
来源：http://mw.asd995.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vi.colortex.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rh.asd995.cn

[A25] 字符串比较
来源：http://ul.szxytkj.cn

Py:   s1 == s2; s1 != s2
来源：http://nm.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cu.gzmigu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wh.hahajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yr.hnjuh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rk.shxzskj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://oj.wgjwhj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yc.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xm.newstarts.cn

[A26] 类型转换总览
来源：http://uz.nicolike.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jj.huanxung.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ao.yuntaijiaju.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tz.bjjhwx.cn

TS:   Number() String() Boolean() x as number
来源：http://cx.jianghongdianzi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yi.szsharing.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xg.lnxyls.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://sq.colortex.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yu.panjiajie.cn

================================================================================
来源：http://fv.chemitech.net.cn

B. 流程控制
来源：http://vf.haigaiapp.cn

================================================================================
来源：http://cp.yuexingan06.cn

[B01] 条件判断 if / else
来源：http://en.muxihuayi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gt.nicolike.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rt.colortex.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ul.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ol.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bo.szsharing.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://my.yuntaijiaju.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fy.shxzskj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rh.newstarts.cn

[B02] 多分支 else if / elif
来源：http://yt.hnjuh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://so.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nd.huanxung.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://al.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wb.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tu.nszjky.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gf.shxzukj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gz.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lv.shxzukj.cn

[B03] switch / match / case
来源：http://ev.yuexingan06.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rb.wgjwhj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jp.szsharing.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tv.jctech888.com.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oj.hnjuh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ia.asd995.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://io.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rk.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ne.bookmarksfly.cn

[B04] for 计数循环
来源：http://km.jctech888.com.cn

Py:   for i in range(10): print(i)
来源：http://fq.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lp.lnxyls.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vb.nicolike.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://le.chemitech.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zs.shxzskj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://so.newstarts.cn

Ruby: 10.times { |i| puts i }
来源：http://nt.wgjwhj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sv.szsharing.cn

[B05] 遍历数组 / 列表
来源：http://pl.asd995.cn

Py:   for item in arr: print(item)
来源：http://ee.yuntaijiaju.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ab.huanxung.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://um.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bg.shtwfgs.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yo.colortex.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cm.huanxung.cn

Ruby: arr.each { |item| puts item }
来源：http://tp.muxihuayi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fs.shxzskj.cn

[B06] 遍历字典 / 对象
来源：http://pe.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jh.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wt.bjjhwx.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kh.haigaiapp.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cc.bjjhwx.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://im.nszjky.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kx.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nw.szsharing.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yb.wgjwhj.cn

[B07] while 循环
来源：http://uc.nszjky.cn

Py:   while i < 10: i += 1
来源：http://cd.yuntaijiaju.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zr.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://xr.chemitech.net.cn

TS:   while (i < 10) { i++; }
来源：http://ta.haigaiapp.cn

Java: while (i < 10) { i++; }
来源：http://vy.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kx.9csxet.cn

Ruby: while i < 10; i += 1; end
来源：http://gi.szxytkj.cn

C#:   while (i < 10) { i++; }
来源：http://mo.bookmarksfly.cn

[B08] do-while（至少执行一次）
来源：http://ub.huixinmuqiang.cn

Py:   # 无 do-while：用 while True + break
来源：http://jp.huixinmuqiang.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xu.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://aq.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://bo.521024.cn


<!-- 参考信息 -->