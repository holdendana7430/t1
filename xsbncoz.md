代发 wailian999

[A06] 字符串转数字
来源：http://kb.haigaiapp.cn

Py:   int("42"); float("3.14")
来源：http://my.haigaiapp.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ag.bookmarksfly.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qk.nszjky.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xl.szxytkj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://px.gzmigu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ag.shxzukj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://rv.bjjhwx.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tc.huixinmuqiang.cn

[A07] 数字转字符串
来源：http://jz.huanxung.cn

Py:   str(42)
来源：http://lq.jctech888.com.cn

PHP:  (string) 42; strval(42)
来源：http://uf.jianghongdianzi.cn

JS:   String(42); (42).toString()
来源：http://hc.521024.cn

TS:   String(42)
来源：http://on.szxytkj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://cz.szsharing.cn

Go:   strconv.Itoa(42)
来源：http://uh.nicolike.cn

Ruby: 42.to_s
来源：http://jj.yuntaijiaju.cn

C#:   42.ToString()
来源：http://gc.colortex.cn

[A08] 取整与四舍五入
来源：http://sg.521024.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bi.jianghongdianzi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cd.hnjuh.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qx.bookmarksfly.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gg.huixinmuqiang.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tt.colortex.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qd.shxzukj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://lw.yuntaijiaju.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ad.jctech888.com.cn

[A09] 绝对值与最大最小值
来源：http://hx.szsharing.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xv.haigaiapp.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vm.yuntaijiaju.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bd.huixiangedu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hm.muxihuayi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xz.chemitech.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xe.colortex.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://em.wgjwhj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://es.nszjky.cn

[A10] 生成随机数
来源：http://ha.nicolike.cn

Py:   import random; random.randint(1, 100)
来源：http://mp.huanxung.cn

PHP:  random_int(1, 100);
来源：http://rs.hnjuh.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://px.shxzukj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ra.gzmigu.cn

Java: new Random().nextInt(100) + 1
来源：http://yn.yuexingan06.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qj.hahajie.cn

Ruby: rand(1..100)
来源：http://fr.521024.cn

C#:   new Random().Next(1, 101)
来源：http://uf.521024.cn

[A11] 条件表达式（三元）
来源：http://fn.newstarts.cn

Py:   "yes" if x > 0 else "no"
来源：http://rw.yuexingan06.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://th.haigaiapp.cn

JS:   x > 0 ? "yes" : "no"
来源：http://lz.muxihuayi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://en.lnxyls.cn

Java: x > 0 ? "yes" : "no"
来源：http://ev.huanxung.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ir.asd995.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ma.haigaiapp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://hq.wgjwhj.cn

[A12] 字符串插值 / 格式化
来源：http://wp.lnxyls.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://yz.panjiajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pn.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://cj.jctech888.com.cn

TS:   `Hello, ${name}!`
来源：http://tv.chemitech.net.cn

Java: "Hello, %s!".formatted(name)
来源：http://lm.colortex.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hk.huixiangedu.cn

Ruby: "Hello, #{name}!"
来源：http://sp.newstarts.cn

C#:   $"Hello, {name}!"
来源：http://pb.hnjuh.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ye.asd995.cn

Py:   "第一行\n第二行"
来源：http://it.haigaiapp.cn

PHP:  "第一行\n第二行"
来源：http://wv.huixiangedu.cn

JS:   "第一行\n第二行"
来源：http://id.huixiangedu.cn

TS:   "第一行\n第二行"
来源：http://oj.szsharing.cn

Java: "第一行\n第二行"
来源：http://pm.gzmigu.cn

Go:   "第一行\n第二行"
来源：http://og.9csxet.cn

Ruby: "第一行\n第二行"
来源：http://rr.yuexingan06.cn

C#:   "第一行\n第二行"
来源：http://xp.huixiangedu.cn

[A14] 注释写法
来源：http://dj.muxihuayi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://lr.shxzskj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://um.huixinmuqiang.cn

JS:   // 单行；/* 多行 */
来源：http://oo.wgjwhj.cn

TS:   // 单行；/* 多行 */
来源：http://zq.szxytkj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fu.lnxyls.cn

Go:   // 单行；/* 多行 */
来源：http://py.huanxung.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hn.panjiajie.cn

C#:   // 单行；/* 多行 */
来源：http://gf.lnxyls.cn

[A15] 空值判断与默认值
来源：http://dx.bookmarksfly.cn

Py:   value = data or "默认值"
来源：http://wz.yuexingan06.cn

PHP:  $value = $data ?? "默认值";
来源：http://ns.haigaiapp.cn

JS:   const value = data ?? "默认值";
来源：http://sf.huixiangedu.cn

TS:   const value = data ?? "默认值";
来源：http://jp.haigaiapp.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qd.colortex.cn

Go:   if data == "" { data = "默认值" }
来源：http://ey.haigaiapp.cn

Ruby: value = data || "默认值"
来源：http://af.521024.cn

C#:   var value = data ?? "默认值";
来源：http://nv.bookmarksfly.cn

[A16] 真假值判断规则
来源：http://oi.huixinmuqiang.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gv.asd995.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://kn.muxihuayi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xx.asd995.cn

TS:   if (!x) {}
来源：http://ug.hnjuh.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kv.shtwfgs.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ev.gzmigu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xn.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qg.muxihuayi.cn

[A17] 位运算
来源：http://wl.lnxyls.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://it.jctech888.com.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://al.szsharing.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qo.huixiangedu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tc.9csxet.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://et.yuntaijiaju.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zk.asd995.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://as.chemitech.net.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://td.lnxyls.cn

[A18] 字符与 ASCII 码互转
来源：http://xa.szxytkj.cn

Py:   ord("A"); chr(65)
来源：http://ax.muxihuayi.cn

PHP:  ord("A"); chr(65)
来源：http://rq.huixiangedu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zp.yuntaijiaju.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ld.newstarts.cn

Java: (int) 'A'; (char) 65
来源：http://af.521024.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jn.wgjwhj.cn

Ruby: "A".ord; 65.chr
来源：http://xd.bjjhwx.cn

C#:   (int)'A'; (char)65
来源：http://do.hahajie.cn

[A19] 交换两个变量
来源：http://kd.gzmigu.cn

Py:   a, b = b, a
来源：http://zd.lnxyls.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tk.wgjwhj.cn

JS:   [a, b] = [b, a];
来源：http://rd.shxzukj.cn

TS:   [a, b] = [b, a];
来源：http://uf.hahajie.cn

Java: int t = a; a = b; b = t;
来源：http://wt.wgjwhj.cn

Go:   a, b = b, a
来源：http://na.huixinmuqiang.cn

Ruby: a, b = b, a
来源：http://me.huanxung.cn

C#:   (a, b) = (b, a);
来源：http://hi.9csxet.cn

[A20] 读取标准输入
来源：http://at.huixinmuqiang.cn

Py:   name = input("请输入：")
来源：http://jp.shxzskj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://lu.hnjuh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wi.yuntaijiaju.cn

TS:   // Node.js：readline 模块
来源：http://gc.huanxung.cn

Java: new Scanner(System.in).nextLine()
来源：http://ks.shxzskj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rs.jianghongdianzi.cn

Ruby: gets.chomp
来源：http://gn.wgjwhj.cn

C#:   Console.ReadLine();
来源：http://kn.nicolike.cn

[A21] 保留指定小数位输出
来源：http://cz.colortex.cn

Py:   f"{3.14159:.2f}"
来源：http://po.szxytkj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://iz.wgjwhj.cn

JS:   (3.14159).toFixed(2)
来源：http://ho.yuntaijiaju.cn

TS:   (3.14159).toFixed(2)
来源：http://qe.shxzukj.cn

Java: String.format("%.2f", 3.14159)
来源：http://ge.jctech888.com.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ju.wgjwhj.cn

Ruby: format("%.2f", 3.14159)
来源：http://eu.9csxet.cn

C#:   3.14159.ToString("F2")
来源：http://nc.lnxyls.cn

[A22] 获取字符串长度
来源：http://fx.yuexingan06.cn

Py:   len(s)
来源：http://mw.shxzukj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xq.jctech888.com.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pc.huixiangedu.cn

TS:   s.length
来源：http://jw.hnjuh.cn

Java: s.length()
来源：http://hk.muxihuayi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yb.hnjuh.cn

Ruby: s.length
来源：http://dj.colortex.cn

C#:   s.Length
来源：http://ro.yuntaijiaju.cn

[A23] 大小写转换
来源：http://jd.szxytkj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ak.jctech888.com.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://an.newstarts.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rn.huanxung.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qv.shtwfgs.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xs.yuexingan06.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qh.huixiangedu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fr.bjjhwx.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ho.lnxyls.cn

[A24] 去除首尾空白
来源：http://br.huanxung.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rt.panjiajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://aj.wgjwhj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://th.jctech888.com.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jg.haigaiapp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://oy.newstarts.cn

Go:   strings.TrimSpace(s)
来源：http://hp.shxzukj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ha.huixinmuqiang.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pz.bookmarksfly.cn

[A25] 字符串比较
来源：http://yc.huixinmuqiang.cn

Py:   s1 == s2; s1 != s2
来源：http://cx.jianghongdianzi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nj.bookmarksfly.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://aj.szxytkj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zf.newstarts.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sb.yuntaijiaju.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cw.nszjky.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://iq.shxzukj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ow.wgjwhj.cn

[A26] 类型转换总览
来源：http://sa.panjiajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ws.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wa.nszjky.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sz.wgjwhj.cn

TS:   Number() String() Boolean() x as number
来源：http://aq.huixinmuqiang.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://oc.hnjuh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vj.huixinmuqiang.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zw.nszjky.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uv.jctech888.com.cn

================================================================================
来源：http://ex.yuexingan06.cn

B. 流程控制
来源：http://yc.9csxet.cn

================================================================================
来源：http://oo.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://um.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://kt.9csxet.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cs.newstarts.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zd.szsharing.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mx.yuntaijiaju.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wu.colortex.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lz.gzmigu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gn.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jp.muxihuayi.cn

[B02] 多分支 else if / elif
来源：http://vo.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ci.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jx.huanxung.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ea.huixiangedu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://og.bjjhwx.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kz.shxzskj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kb.chemitech.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cp.nszjky.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nm.nszjky.cn

[B03] switch / match / case
来源：http://ae.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xw.panjiajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uo.521024.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pi.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gt.muxihuayi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cl.nszjky.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cz.asd995.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wf.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gy.muxihuayi.cn

[B04] for 计数循环
来源：http://wh.lnxyls.cn

Py:   for i in range(10): print(i)
来源：http://qs.huixinmuqiang.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sy.haigaiapp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kt.nicolike.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qw.szxytkj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pw.szxytkj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lj.lnxyls.cn

Ruby: 10.times { |i| puts i }
来源：http://et.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://se.hahajie.cn

[B05] 遍历数组 / 列表
来源：http://tw.shxzukj.cn

Py:   for item in arr: print(item)
来源：http://fu.wgjwhj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gj.shtwfgs.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yq.newstarts.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mu.jctech888.com.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vl.szsharing.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ij.jctech888.com.cn

Ruby: arr.each { |item| puts item }
来源：http://wl.szxytkj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://np.chemitech.net.cn

[B06] 遍历字典 / 对象
来源：http://fa.hahajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://em.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nj.panjiajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qz.nszjky.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qe.wgjwhj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gs.asd995.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://er.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xh.shxzskj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xi.jianghongdianzi.cn

[B07] while 循环
来源：http://jt.jianghongdianzi.cn

Py:   while i < 10: i += 1
来源：http://sx.panjiajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://po.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://de.521024.cn

TS:   while (i < 10) { i++; }
来源：http://wo.521024.cn

Java: while (i < 10) { i++; }
来源：http://yq.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jf.lnxyls.cn

Ruby: while i < 10; i += 1; end
来源：http://rm.lnxyls.cn

C#:   while (i < 10) { i++; }
来源：http://zj.yuntaijiaju.cn

[B08] do-while（至少执行一次）
来源：http://jz.shxzukj.cn

Py:   # 无 do-while：用 while True + break
来源：http://yl.colortex.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rm.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://qp.yuexingan06.cn

TS:   do { i++; } while (i < 10);
来源：http://qi.muxihuayi.cn

Java: do { i++; } while (i < 10);
来源：http://vr.szsharing.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ay.hahajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hh.haigaiapp.cn

C#:   do { i++; } while (i < 10);
来源：http://gs.panjiajie.cn

[B09] break 与 continue
来源：http://ek.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ap.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ci.gzmigu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nl.shxzskj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sz.hnjuh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gc.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yi.asd995.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ac.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lo.szxytkj.cn

[B10] 遍历同时拿索引
来源：http://jj.yuntaijiaju.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wp.huixinmuqiang.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vu.bookmarksfly.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ip.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cs.szsharing.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sn.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bi.haigaiapp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rf.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qp.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://tb.newstarts.cn

Py:   list(range(0, 10, 2))
来源：http://ft.bookmarksfly.cn

PHP:  range(0, 10, 2);
来源：http://gx.jianghongdianzi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jy.shxzskj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hm.yuntaijiaju.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lf.bjjhwx.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ws.nicolike.cn

Ruby: (0...10).step(2).to_a
来源：http://lr.jianghongdianzi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tw.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://is.colortex.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qx.asd995.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vv.szsharing.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hv.huixinmuqiang.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gx.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://no.haigaiapp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nh.nicolike.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kr.9csxet.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xy.shxzskj.cn


<!-- 参考信息 -->