代发 wailian999

[A06] 字符串转数字
来源：http://dh.gzmigu.cn

Py:   int("42"); float("3.14")
来源：http://cu.huixiangedu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lr.panjiajie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hj.jianghongdianzi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://zx.hnjuh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vd.asd995.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cn.lnxyls.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://lw.newstarts.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bh.jctech888.com.cn

[A07] 数字转字符串
来源：http://rl.huanxung.cn

Py:   str(42)
来源：http://ra.shtwfgs.cn

PHP:  (string) 42; strval(42)
来源：http://dh.521024.cn

JS:   String(42); (42).toString()
来源：http://ns.huixinmuqiang.cn

TS:   String(42)
来源：http://us.9csxet.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://fl.wgjwhj.cn

Go:   strconv.Itoa(42)
来源：http://zj.asd995.cn

Ruby: 42.to_s
来源：http://dj.chemitech.net.cn

C#:   42.ToString()
来源：http://lk.9csxet.cn

[A08] 取整与四舍五入
来源：http://jo.newstarts.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dd.huixinmuqiang.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://di.panjiajie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hi.huixinmuqiang.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wk.haigaiapp.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ue.szsharing.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kh.chemitech.net.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://yi.yuexingan06.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://uf.huixiangedu.cn

[A09] 绝对值与最大最小值
来源：http://uc.hahajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lx.bookmarksfly.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pg.bjjhwx.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tg.jianghongdianzi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xy.shxzskj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yu.shxzukj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ai.panjiajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ng.jianghongdianzi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bc.szsharing.cn

[A10] 生成随机数
来源：http://zj.nszjky.cn

Py:   import random; random.randint(1, 100)
来源：http://gc.newstarts.cn

PHP:  random_int(1, 100);
来源：http://yi.newstarts.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ja.nicolike.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://up.colortex.cn

Java: new Random().nextInt(100) + 1
来源：http://yr.panjiajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kj.bjjhwx.cn

Ruby: rand(1..100)
来源：http://kj.gzmigu.cn

C#:   new Random().Next(1, 101)
来源：http://qq.asd995.cn

[A11] 条件表达式（三元）
来源：http://nk.jctech888.com.cn

Py:   "yes" if x > 0 else "no"
来源：http://di.huixiangedu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ha.shtwfgs.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xp.asd995.cn

TS:   x > 0 ? "yes" : "no"
来源：http://pq.szsharing.cn

Java: x > 0 ? "yes" : "no"
来源：http://yb.shtwfgs.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://pw.gzmigu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://dh.shtwfgs.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xa.nicolike.cn

[A12] 字符串插值 / 格式化
来源：http://lc.521024.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pk.shxzskj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gs.huanxung.cn

JS:   `Hello, ${name}!`
来源：http://mv.hnjuh.cn

TS:   `Hello, ${name}!`
来源：http://om.haigaiapp.cn

Java: "Hello, %s!".formatted(name)
来源：http://py.huixiangedu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ty.asd995.cn

Ruby: "Hello, #{name}!"
来源：http://do.gzmigu.cn

C#:   $"Hello, {name}!"
来源：http://ok.huixiangedu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://kg.panjiajie.cn

Py:   "第一行\n第二行"
来源：http://ez.jianghongdianzi.cn

PHP:  "第一行\n第二行"
来源：http://mo.szsharing.cn

JS:   "第一行\n第二行"
来源：http://cf.huixiangedu.cn

TS:   "第一行\n第二行"
来源：http://ta.9csxet.cn

Java: "第一行\n第二行"
来源：http://mb.szxytkj.cn

Go:   "第一行\n第二行"
来源：http://ap.521024.cn

Ruby: "第一行\n第二行"
来源：http://xy.9csxet.cn

C#:   "第一行\n第二行"
来源：http://sm.nicolike.cn

[A14] 注释写法
来源：http://zu.shxzskj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://fz.colortex.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ku.haigaiapp.cn

JS:   // 单行；/* 多行 */
来源：http://xe.huixiangedu.cn

TS:   // 单行；/* 多行 */
来源：http://oc.huanxung.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rb.shtwfgs.cn

Go:   // 单行；/* 多行 */
来源：http://rx.jianghongdianzi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://gk.panjiajie.cn

C#:   // 单行；/* 多行 */
来源：http://uu.asd995.cn

[A15] 空值判断与默认值
来源：http://eq.colortex.cn

Py:   value = data or "默认值"
来源：http://ei.yuexingan06.cn

PHP:  $value = $data ?? "默认值";
来源：http://ni.wgjwhj.cn

JS:   const value = data ?? "默认值";
来源：http://eu.shtwfgs.cn

TS:   const value = data ?? "默认值";
来源：http://rp.huixinmuqiang.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pc.9csxet.cn

Go:   if data == "" { data = "默认值" }
来源：http://pn.yuntaijiaju.cn

Ruby: value = data || "默认值"
来源：http://xk.nszjky.cn

C#:   var value = data ?? "默认值";
来源：http://qu.bookmarksfly.cn

[A16] 真假值判断规则
来源：http://hi.panjiajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://df.yuexingan06.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://am.huixinmuqiang.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ae.jianghongdianzi.cn

TS:   if (!x) {}
来源：http://cf.nszjky.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xh.bjjhwx.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://uh.huixinmuqiang.cn

Ruby: unless x            # nil 与 false 为假
来源：http://mn.szxytkj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cf.huixiangedu.cn

[A17] 位运算
来源：http://ci.haigaiapp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sn.lnxyls.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tq.gzmigu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yi.shxzskj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://em.nszjky.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xx.lnxyls.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rc.bjjhwx.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fb.panjiajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nq.9csxet.cn

[A18] 字符与 ASCII 码互转
来源：http://jz.muxihuayi.cn

Py:   ord("A"); chr(65)
来源：http://ry.huixiangedu.cn

PHP:  ord("A"); chr(65)
来源：http://im.bookmarksfly.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zz.huixiangedu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lh.jctech888.com.cn

Java: (int) 'A'; (char) 65
来源：http://fw.chemitech.net.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://br.huixinmuqiang.cn

Ruby: "A".ord; 65.chr
来源：http://qm.panjiajie.cn

C#:   (int)'A'; (char)65
来源：http://fl.wgjwhj.cn

[A19] 交换两个变量
来源：http://iu.chemitech.net.cn

Py:   a, b = b, a
来源：http://wd.chemitech.net.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://nd.yuexingan06.cn

JS:   [a, b] = [b, a];
来源：http://kx.nszjky.cn

TS:   [a, b] = [b, a];
来源：http://fm.9csxet.cn

Java: int t = a; a = b; b = t;
来源：http://df.muxihuayi.cn

Go:   a, b = b, a
来源：http://rh.yuexingan06.cn

Ruby: a, b = b, a
来源：http://rw.szsharing.cn

C#:   (a, b) = (b, a);
来源：http://hm.nicolike.cn

[A20] 读取标准输入
来源：http://rg.lnxyls.cn

Py:   name = input("请输入：")
来源：http://qv.shxzukj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ar.hahajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ws.521024.cn

TS:   // Node.js：readline 模块
来源：http://xl.nicolike.cn

Java: new Scanner(System.in).nextLine()
来源：http://ls.bjjhwx.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hs.huanxung.cn

Ruby: gets.chomp
来源：http://la.lnxyls.cn

C#:   Console.ReadLine();
来源：http://vk.bookmarksfly.cn

[A21] 保留指定小数位输出
来源：http://ix.haigaiapp.cn

Py:   f"{3.14159:.2f}"
来源：http://nx.colortex.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kg.szxytkj.cn

JS:   (3.14159).toFixed(2)
来源：http://zv.shtwfgs.cn

TS:   (3.14159).toFixed(2)
来源：http://dg.shtwfgs.cn

Java: String.format("%.2f", 3.14159)
来源：http://xm.521024.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ww.szsharing.cn

Ruby: format("%.2f", 3.14159)
来源：http://hf.9csxet.cn

C#:   3.14159.ToString("F2")
来源：http://qp.jctech888.com.cn

[A22] 获取字符串长度
来源：http://dc.shxzukj.cn

Py:   len(s)
来源：http://ul.yuntaijiaju.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lt.shtwfgs.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vk.haigaiapp.cn

TS:   s.length
来源：http://yg.colortex.cn

Java: s.length()
来源：http://ma.521024.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ex.9csxet.cn

Ruby: s.length
来源：http://xr.gzmigu.cn

C#:   s.Length
来源：http://uv.szxytkj.cn

[A23] 大小写转换
来源：http://ry.gzmigu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wy.hnjuh.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rp.chemitech.net.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jq.yuexingan06.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fc.gzmigu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jq.nszjky.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mv.shxzukj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://iq.jctech888.com.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fm.shxzskj.cn

[A24] 去除首尾空白
来源：http://pc.haigaiapp.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jn.lnxyls.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sv.9csxet.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pr.szsharing.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jq.9csxet.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qq.chemitech.net.cn

Go:   strings.TrimSpace(s)
来源：http://ry.szxytkj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://iu.shxzukj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mj.hahajie.cn

[A25] 字符串比较
来源：http://lo.huanxung.cn

Py:   s1 == s2; s1 != s2
来源：http://rw.colortex.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dx.chemitech.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dc.haigaiapp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://il.shxzskj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fj.9csxet.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ng.nszjky.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vb.muxihuayi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sj.chemitech.net.cn

[A26] 类型转换总览
来源：http://jn.bookmarksfly.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cy.szxytkj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kg.wgjwhj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kl.huixinmuqiang.cn

TS:   Number() String() Boolean() x as number
来源：http://pe.chemitech.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ik.bookmarksfly.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kf.asd995.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pf.9csxet.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fw.colortex.cn

================================================================================
来源：http://ci.bjjhwx.cn

B. 流程控制
来源：http://lr.szsharing.cn

================================================================================
来源：http://xi.jianghongdianzi.cn

[B01] 条件判断 if / else
来源：http://zd.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dn.nszjky.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ej.lnxyls.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kb.nicolike.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wc.szsharing.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vt.haigaiapp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ql.muxihuayi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://df.shxzskj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nu.newstarts.cn

[B02] 多分支 else if / elif
来源：http://kk.colortex.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tq.shxzskj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dj.muxihuayi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://we.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cb.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hn.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yk.shxzskj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xu.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://je.shxzukj.cn

[B03] switch / match / case
来源：http://mk.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zg.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ko.521024.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fj.haigaiapp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wu.panjiajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kk.shxzukj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uc.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sm.muxihuayi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ij.bjjhwx.cn

[B04] for 计数循环
来源：http://dv.9csxet.cn

Py:   for i in range(10): print(i)
来源：http://yv.szsharing.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gg.szsharing.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fs.szsharing.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://os.chemitech.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wa.yuntaijiaju.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jp.chemitech.net.cn

Ruby: 10.times { |i| puts i }
来源：http://sb.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uh.yuexingan06.cn

[B05] 遍历数组 / 列表
来源：http://vs.huanxung.cn

Py:   for item in arr: print(item)
来源：http://sv.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fz.huanxung.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kj.colortex.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cq.gzmigu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ei.haigaiapp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://oj.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://pz.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zm.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://ve.szxytkj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mf.shtwfgs.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yw.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ax.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ly.jianghongdianzi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tc.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mh.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gp.shxzukj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dx.jianghongdianzi.cn

[B07] while 循环
来源：http://vq.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://xj.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qe.bjjhwx.cn

JS:   while (i < 10) { i++; }
来源：http://ba.hnjuh.cn

TS:   while (i < 10) { i++; }
来源：http://dj.huanxung.cn

Java: while (i < 10) { i++; }
来源：http://lh.colortex.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mh.shxzskj.cn

Ruby: while i < 10; i += 1; end
来源：http://qr.chemitech.net.cn

C#:   while (i < 10) { i++; }
来源：http://wc.colortex.cn

[B08] do-while（至少执行一次）
来源：http://mp.yuexingan06.cn

Py:   # 无 do-while：用 while True + break
来源：http://bg.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gs.hahajie.cn

JS:   do { i++; } while (i < 10);
来源：http://xm.chemitech.net.cn

TS:   do { i++; } while (i < 10);
来源：http://fu.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://dh.huanxung.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://kx.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ij.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://tl.muxihuayi.cn

[B09] break 与 continue
来源：http://sb.huanxung.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qk.haigaiapp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vd.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pm.yuexingan06.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cm.shxzukj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xs.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xh.huixinmuqiang.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zj.panjiajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vu.nicolike.cn

[B10] 遍历同时拿索引
来源：http://lq.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ck.wgjwhj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ej.newstarts.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ze.shxzukj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jz.bjjhwx.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nt.jianghongdianzi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nn.muxihuayi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cc.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vz.hahajie.cn

[B11] 生成数字序列 / 区间
来源：http://tt.jianghongdianzi.cn

Py:   list(range(0, 10, 2))
来源：http://tm.jctech888.com.cn

PHP:  range(0, 10, 2);
来源：http://ee.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tn.nicolike.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ye.shtwfgs.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mc.szxytkj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zl.lnxyls.cn

Ruby: (0...10).step(2).to_a
来源：http://jm.szsharing.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ds.lnxyls.cn

[B12] 跳出多层循环
来源：http://ok.huixiangedu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lh.shtwfgs.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lr.9csxet.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xn.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kr.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rn.9csxet.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ze.shtwfgs.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sk.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ja.hnjuh.cn


<!-- 参考信息 -->