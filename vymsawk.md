代发 wailian999

[A06] 字符串转数字
来源：http://sf.521024.cn

Py:   int("42"); float("3.14")
来源：http://um.huanxung.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lv.nszjky.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lx.521024.cn

TS:   parseInt("42", 10); Number("42")
来源：http://zs.huixinmuqiang.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://so.shxzskj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ex.lnxyls.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://uq.szsharing.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://db.yuexingan06.cn

[A07] 数字转字符串
来源：http://zr.nszjky.cn

Py:   str(42)
来源：http://tg.shxzskj.cn

PHP:  (string) 42; strval(42)
来源：http://xy.shtwfgs.cn

JS:   String(42); (42).toString()
来源：http://jr.colortex.cn

TS:   String(42)
来源：http://gv.colortex.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://us.521024.cn

Go:   strconv.Itoa(42)
来源：http://xa.bjjhwx.cn

Ruby: 42.to_s
来源：http://ro.huixinmuqiang.cn

C#:   42.ToString()
来源：http://ao.yuntaijiaju.cn

[A08] 取整与四舍五入
来源：http://fe.colortex.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hy.haigaiapp.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xq.bookmarksfly.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://na.huixiangedu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ed.nszjky.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://by.muxihuayi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ic.nicolike.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://cs.shtwfgs.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vh.jianghongdianzi.cn

[A09] 绝对值与最大最小值
来源：http://pt.panjiajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yt.colortex.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qt.shxzskj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rb.szsharing.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ri.bookmarksfly.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bc.9csxet.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jm.wgjwhj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qb.muxihuayi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bt.huixiangedu.cn

[A10] 生成随机数
来源：http://fh.nicolike.cn

Py:   import random; random.randint(1, 100)
来源：http://ez.wgjwhj.cn

PHP:  random_int(1, 100);
来源：http://zk.huixiangedu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sa.wgjwhj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tj.shxzukj.cn

Java: new Random().nextInt(100) + 1
来源：http://os.jianghongdianzi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rr.huanxung.cn

Ruby: rand(1..100)
来源：http://en.yuntaijiaju.cn

C#:   new Random().Next(1, 101)
来源：http://pf.521024.cn

[A11] 条件表达式（三元）
来源：http://lx.lnxyls.cn

Py:   "yes" if x > 0 else "no"
来源：http://xf.521024.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ep.jianghongdianzi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pd.lnxyls.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ue.9csxet.cn

Java: x > 0 ? "yes" : "no"
来源：http://ue.huanxung.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://uv.nicolike.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://im.shxzskj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xg.shtwfgs.cn

[A12] 字符串插值 / 格式化
来源：http://ur.huixinmuqiang.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pk.huixinmuqiang.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tu.szsharing.cn

JS:   `Hello, ${name}!`
来源：http://qu.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://sj.shtwfgs.cn

Java: "Hello, %s!".formatted(name)
来源：http://jr.jctech888.com.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ww.hahajie.cn

Ruby: "Hello, #{name}!"
来源：http://kn.jianghongdianzi.cn

C#:   $"Hello, {name}!"
来源：http://tg.shxzskj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://yi.bjjhwx.cn

Py:   "第一行\n第二行"
来源：http://im.shxzskj.cn

PHP:  "第一行\n第二行"
来源：http://dd.shxzskj.cn

JS:   "第一行\n第二行"
来源：http://ot.nszjky.cn

TS:   "第一行\n第二行"
来源：http://ti.yuexingan06.cn

Java: "第一行\n第二行"
来源：http://ar.9csxet.cn

Go:   "第一行\n第二行"
来源：http://vh.haigaiapp.cn

Ruby: "第一行\n第二行"
来源：http://we.haigaiapp.cn

C#:   "第一行\n第二行"
来源：http://zb.jctech888.com.cn

[A14] 注释写法
来源：http://ry.shxzskj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://xg.9csxet.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://yd.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://hu.panjiajie.cn

TS:   // 单行；/* 多行 */
来源：http://uq.panjiajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xe.chemitech.net.cn

Go:   // 单行；/* 多行 */
来源：http://ia.shxzskj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xz.shxzukj.cn

C#:   // 单行；/* 多行 */
来源：http://uj.bjjhwx.cn

[A15] 空值判断与默认值
来源：http://wz.521024.cn

Py:   value = data or "默认值"
来源：http://do.gzmigu.cn

PHP:  $value = $data ?? "默认值";
来源：http://ku.newstarts.cn

JS:   const value = data ?? "默认值";
来源：http://qh.shtwfgs.cn

TS:   const value = data ?? "默认值";
来源：http://up.szxytkj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://el.lnxyls.cn

Go:   if data == "" { data = "默认值" }
来源：http://nj.hahajie.cn

Ruby: value = data || "默认值"
来源：http://lm.asd995.cn

C#:   var value = data ?? "默认值";
来源：http://vw.muxihuayi.cn

[A16] 真假值判断规则
来源：http://sd.nszjky.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vq.bjjhwx.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yz.gzmigu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pe.asd995.cn

TS:   if (!x) {}
来源：http://vo.jianghongdianzi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pe.asd995.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ri.asd995.cn

Ruby: unless x            # nil 与 false 为假
来源：http://qi.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rq.yuntaijiaju.cn

[A17] 位运算
来源：http://qw.wgjwhj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eu.huanxung.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ir.asd995.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bm.hnjuh.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://iu.chemitech.net.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qr.newstarts.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cc.huixiangedu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lc.newstarts.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jh.newstarts.cn

[A18] 字符与 ASCII 码互转
来源：http://at.yuntaijiaju.cn

Py:   ord("A"); chr(65)
来源：http://xa.haigaiapp.cn

PHP:  ord("A"); chr(65)
来源：http://pj.huanxung.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cz.haigaiapp.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bt.colortex.cn

Java: (int) 'A'; (char) 65
来源：http://ck.wgjwhj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ak.bjjhwx.cn

Ruby: "A".ord; 65.chr
来源：http://hr.9csxet.cn

C#:   (int)'A'; (char)65
来源：http://qv.jianghongdianzi.cn

[A19] 交换两个变量
来源：http://af.haigaiapp.cn

Py:   a, b = b, a
来源：http://dv.jctech888.com.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://uo.nicolike.cn

JS:   [a, b] = [b, a];
来源：http://vx.bookmarksfly.cn

TS:   [a, b] = [b, a];
来源：http://mo.szsharing.cn

Java: int t = a; a = b; b = t;
来源：http://ia.jctech888.com.cn

Go:   a, b = b, a
来源：http://eo.jctech888.com.cn

Ruby: a, b = b, a
来源：http://ko.hnjuh.cn

C#:   (a, b) = (b, a);
来源：http://wh.muxihuayi.cn

[A20] 读取标准输入
来源：http://wq.szxytkj.cn

Py:   name = input("请输入：")
来源：http://qh.nszjky.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rl.colortex.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lu.shxzskj.cn

TS:   // Node.js：readline 模块
来源：http://tr.nszjky.cn

Java: new Scanner(System.in).nextLine()
来源：http://bu.bookmarksfly.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qh.szsharing.cn

Ruby: gets.chomp
来源：http://kw.shxzukj.cn

C#:   Console.ReadLine();
来源：http://xw.hnjuh.cn

[A21] 保留指定小数位输出
来源：http://bs.asd995.cn

Py:   f"{3.14159:.2f}"
来源：http://dd.nszjky.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dn.newstarts.cn

JS:   (3.14159).toFixed(2)
来源：http://uo.9csxet.cn

TS:   (3.14159).toFixed(2)
来源：http://be.shtwfgs.cn

Java: String.format("%.2f", 3.14159)
来源：http://kh.jianghongdianzi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mm.panjiajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://zw.9csxet.cn

C#:   3.14159.ToString("F2")
来源：http://ix.huixiangedu.cn

[A22] 获取字符串长度
来源：http://ep.shtwfgs.cn

Py:   len(s)
来源：http://ds.colortex.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://at.hahajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xo.szsharing.cn

TS:   s.length
来源：http://hb.szxytkj.cn

Java: s.length()
来源：http://pj.muxihuayi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vy.newstarts.cn

Ruby: s.length
来源：http://cw.521024.cn

C#:   s.Length
来源：http://oj.gzmigu.cn

[A23] 大小写转换
来源：http://xq.hnjuh.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hc.nicolike.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zp.huixinmuqiang.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://td.yuntaijiaju.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vx.yuexingan06.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ib.huanxung.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ri.521024.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ej.lnxyls.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://co.shxzukj.cn

[A24] 去除首尾空白
来源：http://hh.yuntaijiaju.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://aa.bjjhwx.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://et.nszjky.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xj.jctech888.com.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tc.yuexingan06.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sj.hahajie.cn

Go:   strings.TrimSpace(s)
来源：http://ls.bjjhwx.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://js.yuexingan06.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zl.gzmigu.cn

[A25] 字符串比较
来源：http://tm.huixinmuqiang.cn

Py:   s1 == s2; s1 != s2
来源：http://gk.huanxung.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dm.panjiajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pz.yuexingan06.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lb.huixiangedu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pq.hahajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lp.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ec.lnxyls.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mz.panjiajie.cn

[A26] 类型转换总览
来源：http://lq.huanxung.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pq.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yd.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mt.9csxet.cn

TS:   Number() String() Boolean() x as number
来源：http://cd.yuntaijiaju.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ju.hahajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dx.colortex.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://or.yuexingan06.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wc.gzmigu.cn

================================================================================
来源：http://sn.chemitech.net.cn

B. 流程控制
来源：http://ml.panjiajie.cn

================================================================================
来源：http://as.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://hw.haigaiapp.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ld.szsharing.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pq.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vw.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ui.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xr.panjiajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://oo.szsharing.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ow.hahajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vj.521024.cn

[B02] 多分支 else if / elif
来源：http://cj.chemitech.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xa.szsharing.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bk.jctech888.com.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pg.lnxyls.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bs.haigaiapp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xz.jctech888.com.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kt.gzmigu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ua.lnxyls.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wr.jianghongdianzi.cn

[B03] switch / match / case
来源：http://ec.muxihuayi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://si.shxzukj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fe.jctech888.com.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xu.huanxung.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vf.shxzukj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uz.szxytkj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://br.yuexingan06.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lc.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cz.szxytkj.cn

[B04] for 计数循环
来源：http://yn.nicolike.cn

Py:   for i in range(10): print(i)
来源：http://lf.panjiajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ly.shxzukj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qc.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vr.9csxet.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ee.bjjhwx.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nq.nicolike.cn

Ruby: 10.times { |i| puts i }
来源：http://jd.gzmigu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uw.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://ld.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://rm.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sj.bookmarksfly.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://io.jctech888.com.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xn.chemitech.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ue.asd995.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zj.szxytkj.cn

Ruby: arr.each { |item| puts item }
来源：http://cv.nszjky.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nb.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://ba.9csxet.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bs.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xi.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sw.hahajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lo.521024.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mf.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://or.huixinmuqiang.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iw.szxytkj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sn.nicolike.cn

[B07] while 循环
来源：http://lf.bookmarksfly.cn

Py:   while i < 10: i += 1
来源：http://ug.muxihuayi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://iy.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://wf.jianghongdianzi.cn

TS:   while (i < 10) { i++; }
来源：http://ln.gzmigu.cn

Java: while (i < 10) { i++; }
来源：http://yr.szsharing.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xa.panjiajie.cn

Ruby: while i < 10; i += 1; end
来源：http://pz.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://al.nszjky.cn

[B08] do-while（至少执行一次）
来源：http://zy.shtwfgs.cn

Py:   # 无 do-while：用 while True + break
来源：http://js.nicolike.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vb.hnjuh.cn

JS:   do { i++; } while (i < 10);
来源：http://uf.nszjky.cn

TS:   do { i++; } while (i < 10);
来源：http://aa.jctech888.com.cn

Java: do { i++; } while (i < 10);
来源：http://on.yuexingan06.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fc.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pn.nicolike.cn

C#:   do { i++; } while (i < 10);
来源：http://qf.huanxung.cn

[B09] break 与 continue
来源：http://xq.jctech888.com.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wh.9csxet.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uf.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ee.muxihuayi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lw.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qc.nicolike.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sk.newstarts.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lt.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oc.521024.cn

[B10] 遍历同时拿索引
来源：http://qr.hnjuh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://eh.huanxung.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sd.muxihuayi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rg.lnxyls.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pm.newstarts.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fj.bookmarksfly.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://em.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tg.szxytkj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vc.colortex.cn

[B11] 生成数字序列 / 区间
来源：http://oo.jianghongdianzi.cn

Py:   list(range(0, 10, 2))
来源：http://ae.521024.cn

PHP:  range(0, 10, 2);
来源：http://dd.huanxung.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vy.szxytkj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://di.huanxung.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ts.szxytkj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hi.lnxyls.cn

Ruby: (0...10).step(2).to_a
来源：http://hl.colortex.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fy.panjiajie.cn

[B12] 跳出多层循环
来源：http://so.hahajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yb.shtwfgs.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kw.hnjuh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ms.jianghongdianzi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://le.521024.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ya.521024.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ze.521024.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ro.chemitech.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xl.gzmigu.cn


<!-- 参考信息 -->