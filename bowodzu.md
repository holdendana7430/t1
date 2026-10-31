代发 wailian999

Ruby: PI = 3.14159
来源：http://pr.nszjky.cn

C#:   const double PI = 3.14159;
来源：http://bt.lnxyls.cn

[A04] 判断变量类型
来源：http://cl.nicolike.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://sp.521024.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://or.newstarts.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cu.9csxet.cn

TS:   typeof x; x instanceof Date
来源：http://hl.jianghongdianzi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gu.lnxyls.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vj.szsharing.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://uu.huixiangedu.cn

C#:   x.GetType().Name; x is int
来源：http://nz.asd995.cn

[A05] 整数除法与取模
来源：http://sb.shtwfgs.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dn.panjiajie.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ox.lnxyls.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tj.huixiangedu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fj.newstarts.cn

Java: 7 / 2; 7 % 2
来源：http://it.lnxyls.cn

Go:   7 / 2; 7 % 2
来源：http://sy.asd995.cn

Ruby: 7 / 2; 7 % 2
来源：http://nv.jianghongdianzi.cn

C#:   7 / 2; 7 % 2
来源：http://pd.jianghongdianzi.cn

[A06] 字符串转数字
来源：http://dh.bookmarksfly.cn

Py:   int("42"); float("3.14")
来源：http://wh.chemitech.net.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://od.bjjhwx.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ya.521024.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ax.asd995.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://by.521024.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yh.wgjwhj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://gk.yuntaijiaju.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wv.nszjky.cn

[A07] 数字转字符串
来源：http://yk.nicolike.cn

Py:   str(42)
来源：http://ws.yuntaijiaju.cn

PHP:  (string) 42; strval(42)
来源：http://zl.wgjwhj.cn

JS:   String(42); (42).toString()
来源：http://zg.huanxung.cn

TS:   String(42)
来源：http://vb.521024.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://gv.wgjwhj.cn

Go:   strconv.Itoa(42)
来源：http://pe.shxzukj.cn

Ruby: 42.to_s
来源：http://vx.newstarts.cn

C#:   42.ToString()
来源：http://ox.gzmigu.cn

[A08] 取整与四舍五入
来源：http://nz.chemitech.net.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yu.gzmigu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mi.szsharing.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://on.asd995.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ou.newstarts.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sa.asd995.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ux.huixiangedu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://hc.nicolike.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gx.jianghongdianzi.cn

[A09] 绝对值与最大最小值
来源：http://gr.asd995.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ri.muxihuayi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jb.szsharing.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ul.lnxyls.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bf.lnxyls.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dt.muxihuayi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://st.newstarts.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qm.bjjhwx.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://by.huanxung.cn

[A10] 生成随机数
来源：http://mj.muxihuayi.cn

Py:   import random; random.randint(1, 100)
来源：http://sz.yuntaijiaju.cn

PHP:  random_int(1, 100);
来源：http://sd.jianghongdianzi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sy.shtwfgs.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://px.haigaiapp.cn

Java: new Random().nextInt(100) + 1
来源：http://po.shxzskj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ci.jianghongdianzi.cn

Ruby: rand(1..100)
来源：http://kk.muxihuayi.cn

C#:   new Random().Next(1, 101)
来源：http://pw.jctech888.com.cn

[A11] 条件表达式（三元）
来源：http://qd.shxzskj.cn

Py:   "yes" if x > 0 else "no"
来源：http://ox.hahajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cg.jctech888.com.cn

JS:   x > 0 ? "yes" : "no"
来源：http://oe.panjiajie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rz.szxytkj.cn

Java: x > 0 ? "yes" : "no"
来源：http://on.nszjky.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ep.9csxet.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qd.muxihuayi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://qk.jianghongdianzi.cn

[A12] 字符串插值 / 格式化
来源：http://dm.newstarts.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cb.shxzskj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://su.muxihuayi.cn

JS:   `Hello, ${name}!`
来源：http://po.shtwfgs.cn

TS:   `Hello, ${name}!`
来源：http://uf.521024.cn

Java: "Hello, %s!".formatted(name)
来源：http://nx.bjjhwx.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ct.yuntaijiaju.cn

Ruby: "Hello, #{name}!"
来源：http://li.nicolike.cn

C#:   $"Hello, {name}!"
来源：http://fg.newstarts.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://wr.gzmigu.cn

Py:   "第一行\n第二行"
来源：http://vg.muxihuayi.cn

PHP:  "第一行\n第二行"
来源：http://tf.nicolike.cn

JS:   "第一行\n第二行"
来源：http://or.szsharing.cn

TS:   "第一行\n第二行"
来源：http://un.shxzskj.cn

Java: "第一行\n第二行"
来源：http://ol.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://fq.chemitech.net.cn

Ruby: "第一行\n第二行"
来源：http://es.shtwfgs.cn

C#:   "第一行\n第二行"
来源：http://yl.nicolike.cn

[A14] 注释写法
来源：http://iw.newstarts.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://fy.muxihuayi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://gf.haigaiapp.cn

JS:   // 单行；/* 多行 */
来源：http://ky.9csxet.cn

TS:   // 单行；/* 多行 */
来源：http://js.jianghongdianzi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tx.panjiajie.cn

Go:   // 单行；/* 多行 */
来源：http://kj.panjiajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://yr.chemitech.net.cn

C#:   // 单行；/* 多行 */
来源：http://le.huixiangedu.cn

[A15] 空值判断与默认值
来源：http://ax.nszjky.cn

Py:   value = data or "默认值"
来源：http://lo.bookmarksfly.cn

PHP:  $value = $data ?? "默认值";
来源：http://kl.haigaiapp.cn

JS:   const value = data ?? "默认值";
来源：http://oy.colortex.cn

TS:   const value = data ?? "默认值";
来源：http://mx.jianghongdianzi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nu.jianghongdianzi.cn

Go:   if data == "" { data = "默认值" }
来源：http://nq.chemitech.net.cn

Ruby: value = data || "默认值"
来源：http://ov.521024.cn

C#:   var value = data ?? "默认值";
来源：http://ak.haigaiapp.cn

[A16] 真假值判断规则
来源：http://jc.huixinmuqiang.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ej.jianghongdianzi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dd.wgjwhj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://in.chemitech.net.cn

TS:   if (!x) {}
来源：http://hp.jctech888.com.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gu.nicolike.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bk.hnjuh.cn

Ruby: unless x            # nil 与 false 为假
来源：http://bd.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fs.huixiangedu.cn

[A17] 位运算
来源：http://jl.hahajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kt.wgjwhj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xu.hnjuh.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gn.huanxung.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rd.jianghongdianzi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rp.shxzukj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://by.colortex.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kt.jctech888.com.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rj.muxihuayi.cn

[A18] 字符与 ASCII 码互转
来源：http://ww.jctech888.com.cn

Py:   ord("A"); chr(65)
来源：http://sc.nicolike.cn

PHP:  ord("A"); chr(65)
来源：http://cj.haigaiapp.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ei.bookmarksfly.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gh.hnjuh.cn

Java: (int) 'A'; (char) 65
来源：http://yk.521024.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pz.shxzskj.cn

Ruby: "A".ord; 65.chr
来源：http://et.nszjky.cn

C#:   (int)'A'; (char)65
来源：http://zp.wgjwhj.cn

[A19] 交换两个变量
来源：http://js.gzmigu.cn

Py:   a, b = b, a
来源：http://fp.asd995.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qw.nicolike.cn

JS:   [a, b] = [b, a];
来源：http://li.bookmarksfly.cn

TS:   [a, b] = [b, a];
来源：http://sp.shxzukj.cn

Java: int t = a; a = b; b = t;
来源：http://gf.shtwfgs.cn

Go:   a, b = b, a
来源：http://sb.521024.cn

Ruby: a, b = b, a
来源：http://lc.huixiangedu.cn

C#:   (a, b) = (b, a);
来源：http://mw.wgjwhj.cn

[A20] 读取标准输入
来源：http://no.wgjwhj.cn

Py:   name = input("请输入：")
来源：http://el.jianghongdianzi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://fr.shxzukj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://io.colortex.cn

TS:   // Node.js：readline 模块
来源：http://ns.shxzskj.cn

Java: new Scanner(System.in).nextLine()
来源：http://rn.chemitech.net.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yp.jianghongdianzi.cn

Ruby: gets.chomp
来源：http://yf.shtwfgs.cn

C#:   Console.ReadLine();
来源：http://jx.hahajie.cn

[A21] 保留指定小数位输出
来源：http://ur.bookmarksfly.cn

Py:   f"{3.14159:.2f}"
来源：http://oz.colortex.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vd.panjiajie.cn

JS:   (3.14159).toFixed(2)
来源：http://op.asd995.cn

TS:   (3.14159).toFixed(2)
来源：http://kv.shtwfgs.cn

Java: String.format("%.2f", 3.14159)
来源：http://bx.nicolike.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cj.wgjwhj.cn

Ruby: format("%.2f", 3.14159)
来源：http://sk.hnjuh.cn

C#:   3.14159.ToString("F2")
来源：http://sj.9csxet.cn

[A22] 获取字符串长度
来源：http://uo.jctech888.com.cn

Py:   len(s)
来源：http://av.panjiajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rd.bjjhwx.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xh.newstarts.cn

TS:   s.length
来源：http://fn.bookmarksfly.cn

Java: s.length()
来源：http://cs.colortex.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pf.shtwfgs.cn

Ruby: s.length
来源：http://kk.gzmigu.cn

C#:   s.Length
来源：http://oy.shxzskj.cn

[A23] 大小写转换
来源：http://ct.haigaiapp.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://uo.jianghongdianzi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fn.jianghongdianzi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kb.colortex.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ii.nicolike.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nb.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gn.wgjwhj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nq.nicolike.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://bz.9csxet.cn

[A24] 去除首尾空白
来源：http://np.shtwfgs.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lf.9csxet.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bp.shxzskj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mv.hahajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hr.huixiangedu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://al.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://pa.jctech888.com.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gs.huixinmuqiang.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qv.lnxyls.cn

[A25] 字符串比较
来源：http://qk.lnxyls.cn

Py:   s1 == s2; s1 != s2
来源：http://qi.nszjky.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://db.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://eu.chemitech.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sz.shxzukj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ui.yuntaijiaju.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vz.shxzukj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xx.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vj.hahajie.cn

[A26] 类型转换总览
来源：http://te.yuexingan06.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://es.asd995.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://js.shtwfgs.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://el.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://gr.hahajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ln.szxytkj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oe.yuexingan06.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://um.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wr.bookmarksfly.cn

================================================================================
来源：http://zu.bookmarksfly.cn

B. 流程控制
来源：http://pr.colortex.cn

================================================================================
来源：http://tq.hnjuh.cn

[B01] 条件判断 if / else
来源：http://cw.jctech888.com.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zm.bookmarksfly.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xb.newstarts.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vi.shtwfgs.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://do.szxytkj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cw.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qf.nicolike.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hj.szxytkj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hu.wgjwhj.cn

[B02] 多分支 else if / elif
来源：http://km.haigaiapp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kw.shxzskj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ls.newstarts.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ff.shtwfgs.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ck.hahajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lj.wgjwhj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pz.nicolike.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ll.shxzskj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lv.jianghongdianzi.cn

[B03] switch / match / case
来源：http://ot.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cm.gzmigu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ym.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sv.lnxyls.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://le.huanxung.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gq.huixiangedu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qi.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ta.shxzukj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ba.haigaiapp.cn

[B04] for 计数循环
来源：http://ne.yuntaijiaju.cn

Py:   for i in range(10): print(i)
来源：http://vj.shxzskj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://da.hnjuh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cu.lnxyls.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aj.szsharing.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ko.haigaiapp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fc.bjjhwx.cn

Ruby: 10.times { |i| puts i }
来源：http://lu.huixiangedu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mw.wgjwhj.cn

[B05] 遍历数组 / 列表
来源：http://vn.hahajie.cn

Py:   for item in arr: print(item)
来源：http://tw.yuexingan06.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rf.huixiangedu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jv.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pg.hnjuh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fx.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ho.muxihuayi.cn

Ruby: arr.each { |item| puts item }
来源：http://pt.panjiajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bk.colortex.cn

[B06] 遍历字典 / 对象
来源：http://tj.gzmigu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ue.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nx.muxihuayi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://le.shtwfgs.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iu.bookmarksfly.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vt.shxzskj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yb.chemitech.net.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wm.jianghongdianzi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://st.jctech888.com.cn

[B07] while 循环
来源：http://hz.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://rm.lnxyls.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kb.szsharing.cn

JS:   while (i < 10) { i++; }
来源：http://mx.wgjwhj.cn

TS:   while (i < 10) { i++; }
来源：http://lh.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://ul.hahajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mm.shxzskj.cn

Ruby: while i < 10; i += 1; end
来源：http://yv.chemitech.net.cn

C#:   while (i < 10) { i++; }
来源：http://fk.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://dq.521024.cn

Py:   # 无 do-while：用 while True + break
来源：http://br.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yx.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://bb.jianghongdianzi.cn

TS:   do { i++; } while (i < 10);
来源：http://ej.shxzskj.cn

Java: do { i++; } while (i < 10);
来源：http://rl.szxytkj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://au.bjjhwx.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fr.huixiangedu.cn

C#:   do { i++; } while (i < 10);
来源：http://cn.nszjky.cn

[B09] break 与 continue
来源：http://tj.panjiajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nj.wgjwhj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eb.shtwfgs.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ha.hahajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kn.gzmigu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zp.bookmarksfly.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uh.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xs.panjiajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uc.szxytkj.cn

[B10] 遍历同时拿索引
来源：http://qg.shxzukj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rn.521024.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bm.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gb.huixiangedu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vm.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fj.nicolike.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vr.panjiajie.cn


<!-- 参考信息 -->