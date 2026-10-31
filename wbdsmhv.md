代发 wailian999

Java: 7 / 2; 7 % 2
来源：http://uz.chemitech.net.cn

Go:   7 / 2; 7 % 2
来源：http://ps.wgjwhj.cn

Ruby: 7 / 2; 7 % 2
来源：http://qi.jctech888.com.cn

C#:   7 / 2; 7 % 2
来源：http://tl.haigaiapp.cn

[A06] 字符串转数字
来源：http://mo.hnjuh.cn

Py:   int("42"); float("3.14")
来源：http://jt.jianghongdianzi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ay.newstarts.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mb.colortex.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ml.hnjuh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://lx.9csxet.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bq.panjiajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://qd.shxzukj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pu.bjjhwx.cn

[A07] 数字转字符串
来源：http://xc.huanxung.cn

Py:   str(42)
来源：http://tz.muxihuayi.cn

PHP:  (string) 42; strval(42)
来源：http://th.shxzukj.cn

JS:   String(42); (42).toString()
来源：http://yt.wgjwhj.cn

TS:   String(42)
来源：http://rm.colortex.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://uf.jctech888.com.cn

Go:   strconv.Itoa(42)
来源：http://if.huixinmuqiang.cn

Ruby: 42.to_s
来源：http://ln.nicolike.cn

C#:   42.ToString()
来源：http://zz.huixinmuqiang.cn

[A08] 取整与四舍五入
来源：http://ka.wgjwhj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tf.bookmarksfly.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://pu.bookmarksfly.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tx.gzmigu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bg.shtwfgs.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gt.gzmigu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gg.yuntaijiaju.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://lv.gzmigu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xy.yuexingan06.cn

[A09] 绝对值与最大最小值
来源：http://nf.yuexingan06.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dh.bjjhwx.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vd.shxzskj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nx.bookmarksfly.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://sy.shtwfgs.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fo.haigaiapp.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nb.chemitech.net.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bs.yuntaijiaju.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hs.wgjwhj.cn

[A10] 生成随机数
来源：http://nt.szxytkj.cn

Py:   import random; random.randint(1, 100)
来源：http://xd.panjiajie.cn

PHP:  random_int(1, 100);
来源：http://pz.bjjhwx.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://re.jctech888.com.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lj.shtwfgs.cn

Java: new Random().nextInt(100) + 1
来源：http://sd.521024.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fz.hnjuh.cn

Ruby: rand(1..100)
来源：http://yd.yuntaijiaju.cn

C#:   new Random().Next(1, 101)
来源：http://vy.bookmarksfly.cn

[A11] 条件表达式（三元）
来源：http://kk.shtwfgs.cn

Py:   "yes" if x > 0 else "no"
来源：http://bx.9csxet.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ep.yuexingan06.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pe.hahajie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://hz.muxihuayi.cn

Java: x > 0 ? "yes" : "no"
来源：http://xc.panjiajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://fw.chemitech.net.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://we.chemitech.net.cn

C#:   x > 0 ? "yes" : "no"
来源：http://an.yuntaijiaju.cn

[A12] 字符串插值 / 格式化
来源：http://hi.wgjwhj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://yc.huixinmuqiang.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://iv.wgjwhj.cn

JS:   `Hello, ${name}!`
来源：http://ba.chemitech.net.cn

TS:   `Hello, ${name}!`
来源：http://lc.gzmigu.cn

Java: "Hello, %s!".formatted(name)
来源：http://mr.panjiajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fk.bookmarksfly.cn

Ruby: "Hello, #{name}!"
来源：http://rg.huixinmuqiang.cn

C#:   $"Hello, {name}!"
来源：http://jj.shtwfgs.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://tx.colortex.cn

Py:   "第一行\n第二行"
来源：http://vd.lnxyls.cn

PHP:  "第一行\n第二行"
来源：http://lg.521024.cn

JS:   "第一行\n第二行"
来源：http://ex.hnjuh.cn

TS:   "第一行\n第二行"
来源：http://yd.gzmigu.cn

Java: "第一行\n第二行"
来源：http://hl.jianghongdianzi.cn

Go:   "第一行\n第二行"
来源：http://sn.huixiangedu.cn

Ruby: "第一行\n第二行"
来源：http://so.huixiangedu.cn

C#:   "第一行\n第二行"
来源：http://ba.muxihuayi.cn

[A14] 注释写法
来源：http://zu.muxihuayi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://kf.szsharing.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://mf.asd995.cn

JS:   // 单行；/* 多行 */
来源：http://gg.haigaiapp.cn

TS:   // 单行；/* 多行 */
来源：http://jp.newstarts.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://av.szxytkj.cn

Go:   // 单行；/* 多行 */
来源：http://eb.521024.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xs.bookmarksfly.cn

C#:   // 单行；/* 多行 */
来源：http://qx.huixinmuqiang.cn

[A15] 空值判断与默认值
来源：http://qg.muxihuayi.cn

Py:   value = data or "默认值"
来源：http://wa.lnxyls.cn

PHP:  $value = $data ?? "默认值";
来源：http://ko.muxihuayi.cn

JS:   const value = data ?? "默认值";
来源：http://co.bookmarksfly.cn

TS:   const value = data ?? "默认值";
来源：http://kz.nszjky.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ai.haigaiapp.cn

Go:   if data == "" { data = "默认值" }
来源：http://aa.bookmarksfly.cn

Ruby: value = data || "默认值"
来源：http://es.haigaiapp.cn

C#:   var value = data ?? "默认值";
来源：http://xo.521024.cn

[A16] 真假值判断规则
来源：http://ap.hnjuh.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xb.hahajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tj.9csxet.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vv.521024.cn

TS:   if (!x) {}
来源：http://wh.muxihuayi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dl.muxihuayi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ho.colortex.cn

Ruby: unless x            # nil 与 false 为假
来源：http://sw.9csxet.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yx.asd995.cn

[A17] 位运算
来源：http://dt.newstarts.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qj.shxzukj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uy.shtwfgs.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sh.shtwfgs.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wy.huixiangedu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rh.muxihuayi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fi.lnxyls.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xi.hnjuh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iu.yuexingan06.cn

[A18] 字符与 ASCII 码互转
来源：http://hs.asd995.cn

Py:   ord("A"); chr(65)
来源：http://ct.bjjhwx.cn

PHP:  ord("A"); chr(65)
来源：http://qx.yuntaijiaju.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rn.huixiangedu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ok.jctech888.com.cn

Java: (int) 'A'; (char) 65
来源：http://qq.wgjwhj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jc.521024.cn

Ruby: "A".ord; 65.chr
来源：http://ss.muxihuayi.cn

C#:   (int)'A'; (char)65
来源：http://cm.szxytkj.cn

[A19] 交换两个变量
来源：http://hk.shxzukj.cn

Py:   a, b = b, a
来源：http://ay.yuntaijiaju.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://bm.szxytkj.cn

JS:   [a, b] = [b, a];
来源：http://ax.bookmarksfly.cn

TS:   [a, b] = [b, a];
来源：http://um.nszjky.cn

Java: int t = a; a = b; b = t;
来源：http://ig.huixinmuqiang.cn

Go:   a, b = b, a
来源：http://hs.shtwfgs.cn

Ruby: a, b = b, a
来源：http://my.newstarts.cn

C#:   (a, b) = (b, a);
来源：http://tk.yuntaijiaju.cn

[A20] 读取标准输入
来源：http://bj.chemitech.net.cn

Py:   name = input("请输入：")
来源：http://pq.szxytkj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://lc.nicolike.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wx.haigaiapp.cn

TS:   // Node.js：readline 模块
来源：http://xs.shxzskj.cn

Java: new Scanner(System.in).nextLine()
来源：http://xf.newstarts.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sw.hahajie.cn

Ruby: gets.chomp
来源：http://qw.gzmigu.cn

C#:   Console.ReadLine();
来源：http://oj.521024.cn

[A21] 保留指定小数位输出
来源：http://sd.newstarts.cn

Py:   f"{3.14159:.2f}"
来源：http://zu.yuexingan06.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ou.gzmigu.cn

JS:   (3.14159).toFixed(2)
来源：http://wi.wgjwhj.cn

TS:   (3.14159).toFixed(2)
来源：http://bg.newstarts.cn

Java: String.format("%.2f", 3.14159)
来源：http://ma.nszjky.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tt.lnxyls.cn

Ruby: format("%.2f", 3.14159)
来源：http://od.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://dt.hnjuh.cn

[A22] 获取字符串长度
来源：http://qo.panjiajie.cn

Py:   len(s)
来源：http://sz.shxzukj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ty.nicolike.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yx.hahajie.cn

TS:   s.length
来源：http://dd.wgjwhj.cn

Java: s.length()
来源：http://xq.huixinmuqiang.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hq.9csxet.cn

Ruby: s.length
来源：http://vc.521024.cn

C#:   s.Length
来源：http://uh.huanxung.cn

[A23] 大小写转换
来源：http://pi.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ou.huixinmuqiang.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://td.gzmigu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mx.huixinmuqiang.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ia.jianghongdianzi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rb.hnjuh.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gh.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yq.shtwfgs.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jc.yuexingan06.cn

[A24] 去除首尾空白
来源：http://ri.gzmigu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ht.yuexingan06.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fr.shxzskj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yz.shtwfgs.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kd.9csxet.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xp.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://lq.hnjuh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gb.jctech888.com.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://aj.muxihuayi.cn

[A25] 字符串比较
来源：http://ak.szsharing.cn

Py:   s1 == s2; s1 != s2
来源：http://pj.haigaiapp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qc.hahajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ku.newstarts.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ws.asd995.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cd.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ea.shtwfgs.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://og.shtwfgs.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lt.bjjhwx.cn

[A26] 类型转换总览
来源：http://jw.nicolike.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dz.colortex.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://al.muxihuayi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nm.bjjhwx.cn

TS:   Number() String() Boolean() x as number
来源：http://xb.9csxet.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://af.panjiajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zg.gzmigu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jb.muxihuayi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://za.szxytkj.cn

================================================================================
来源：http://dn.9csxet.cn

B. 流程控制
来源：http://ux.szsharing.cn

================================================================================
来源：http://aq.szsharing.cn

[B01] 条件判断 if / else
来源：http://bd.yuexingan06.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ve.asd995.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rl.bookmarksfly.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tz.bjjhwx.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://if.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cw.nszjky.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pj.jianghongdianzi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ws.bjjhwx.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xq.chemitech.net.cn

[B02] 多分支 else if / elif
来源：http://vi.szxytkj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ic.shxzukj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ax.hnjuh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://md.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ub.nszjky.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hk.yuexingan06.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zs.521024.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vs.jctech888.com.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://op.hnjuh.cn

[B03] switch / match / case
来源：http://tz.nszjky.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xs.jctech888.com.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ri.yuexingan06.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kp.wgjwhj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rj.shtwfgs.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://um.wgjwhj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rd.shxzskj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xo.huixinmuqiang.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fx.wgjwhj.cn

[B04] for 计数循环
来源：http://bq.bookmarksfly.cn

Py:   for i in range(10): print(i)
来源：http://sz.asd995.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fw.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fr.panjiajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fj.shtwfgs.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jw.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ul.asd995.cn

Ruby: 10.times { |i| puts i }
来源：http://ut.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uc.colortex.cn

[B05] 遍历数组 / 列表
来源：http://to.nszjky.cn

Py:   for item in arr: print(item)
来源：http://oj.wgjwhj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tj.huixiangedu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xd.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gn.shxzukj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yj.colortex.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ao.colortex.cn

Ruby: arr.each { |item| puts item }
来源：http://en.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hx.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://iu.shtwfgs.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zg.nicolike.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zg.hnjuh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pf.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ly.jctech888.com.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uc.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yb.hnjuh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ko.chemitech.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ou.jianghongdianzi.cn

[B07] while 循环
来源：http://vs.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://ta.shxzukj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ve.szsharing.cn

JS:   while (i < 10) { i++; }
来源：http://pj.shxzukj.cn

TS:   while (i < 10) { i++; }
来源：http://dw.521024.cn

Java: while (i < 10) { i++; }
来源：http://yp.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fo.shxzskj.cn

Ruby: while i < 10; i += 1; end
来源：http://hi.yuexingan06.cn

C#:   while (i < 10) { i++; }
来源：http://zt.yuexingan06.cn

[B08] do-while（至少执行一次）
来源：http://gn.huixiangedu.cn

Py:   # 无 do-while：用 while True + break
来源：http://aj.huanxung.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qd.jctech888.com.cn

JS:   do { i++; } while (i < 10);
来源：http://vl.huixiangedu.cn

TS:   do { i++; } while (i < 10);
来源：http://ws.9csxet.cn

Java: do { i++; } while (i < 10);
来源：http://jf.panjiajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ux.szsharing.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rs.shxzukj.cn

C#:   do { i++; } while (i < 10);
来源：http://vb.jianghongdianzi.cn

[B09] break 与 continue
来源：http://xq.jctech888.com.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bn.hahajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ys.huanxung.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ul.hnjuh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vd.huanxung.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ux.shxzukj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ot.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cx.9csxet.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iw.nicolike.cn

[B10] 遍历同时拿索引
来源：http://sb.huixinmuqiang.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://af.wgjwhj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bm.shtwfgs.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://np.hnjuh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tq.wgjwhj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://px.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qx.shxzskj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ah.yuntaijiaju.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://am.bjjhwx.cn

[B11] 生成数字序列 / 区间
来源：http://od.hnjuh.cn

Py:   list(range(0, 10, 2))
来源：http://ht.shxzskj.cn

PHP:  range(0, 10, 2);
来源：http://ci.lnxyls.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oz.bjjhwx.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://af.shtwfgs.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jp.bjjhwx.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qy.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://bc.asd995.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tz.hnjuh.cn

[B12] 跳出多层循环
来源：http://sh.521024.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ai.521024.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zn.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wp.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tl.szsharing.cn


<!-- 参考信息 -->