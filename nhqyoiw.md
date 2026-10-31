代发 wailian999

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://to.shxzukj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://cx.yuexingan06.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rp.hnjuh.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gs.hahajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hq.gzmigu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ml.shxzskj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://at.hahajie.cn

[A09] 绝对值与最大最小值
来源：http://pz.wgjwhj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zx.asd995.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kv.jctech888.com.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tq.haigaiapp.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bf.lnxyls.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nh.yuexingan06.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rb.panjiajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rf.nszjky.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pl.szsharing.cn

[A10] 生成随机数
来源：http://pa.shxzskj.cn

Py:   import random; random.randint(1, 100)
来源：http://zd.hahajie.cn

PHP:  random_int(1, 100);
来源：http://jm.chemitech.net.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://re.shtwfgs.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zc.gzmigu.cn

Java: new Random().nextInt(100) + 1
来源：http://rd.huanxung.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://un.wgjwhj.cn

Ruby: rand(1..100)
来源：http://ad.521024.cn

C#:   new Random().Next(1, 101)
来源：http://qq.szsharing.cn

[A11] 条件表达式（三元）
来源：http://pt.huanxung.cn

Py:   "yes" if x > 0 else "no"
来源：http://mp.newstarts.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://pq.9csxet.cn

JS:   x > 0 ? "yes" : "no"
来源：http://kz.chemitech.net.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ap.chemitech.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://pn.chemitech.net.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://kt.jianghongdianzi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://gw.huixiangedu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ic.huanxung.cn

[A12] 字符串插值 / 格式化
来源：http://if.wgjwhj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://po.asd995.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://oi.szsharing.cn

JS:   `Hello, ${name}!`
来源：http://zm.bookmarksfly.cn

TS:   `Hello, ${name}!`
来源：http://fd.lnxyls.cn

Java: "Hello, %s!".formatted(name)
来源：http://gj.nszjky.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gd.lnxyls.cn

Ruby: "Hello, #{name}!"
来源：http://aa.szsharing.cn

C#:   $"Hello, {name}!"
来源：http://qr.shxzskj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://qf.asd995.cn

Py:   "第一行\n第二行"
来源：http://uu.huanxung.cn

PHP:  "第一行\n第二行"
来源：http://kl.yuntaijiaju.cn

JS:   "第一行\n第二行"
来源：http://yf.shxzukj.cn

TS:   "第一行\n第二行"
来源：http://va.nszjky.cn

Java: "第一行\n第二行"
来源：http://hc.hnjuh.cn

Go:   "第一行\n第二行"
来源：http://oo.nicolike.cn

Ruby: "第一行\n第二行"
来源：http://ba.shxzukj.cn

C#:   "第一行\n第二行"
来源：http://ao.jianghongdianzi.cn

[A14] 注释写法
来源：http://hb.yuexingan06.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://oa.shxzukj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://jb.shxzskj.cn

JS:   // 单行；/* 多行 */
来源：http://xb.huixinmuqiang.cn

TS:   // 单行；/* 多行 */
来源：http://cn.lnxyls.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fz.newstarts.cn

Go:   // 单行；/* 多行 */
来源：http://us.shxzskj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://jo.hahajie.cn

C#:   // 单行；/* 多行 */
来源：http://ec.szxytkj.cn

[A15] 空值判断与默认值
来源：http://kl.bjjhwx.cn

Py:   value = data or "默认值"
来源：http://fc.bookmarksfly.cn

PHP:  $value = $data ?? "默认值";
来源：http://pp.521024.cn

JS:   const value = data ?? "默认值";
来源：http://nr.nszjky.cn

TS:   const value = data ?? "默认值";
来源：http://lh.shxzukj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rh.hahajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://hv.shxzskj.cn

Ruby: value = data || "默认值"
来源：http://el.hnjuh.cn

C#:   var value = data ?? "默认值";
来源：http://dp.wgjwhj.cn

[A16] 真假值判断规则
来源：http://ef.shtwfgs.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://id.panjiajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dm.jctech888.com.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dg.shxzukj.cn

TS:   if (!x) {}
来源：http://oe.panjiajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ub.hahajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ul.yuexingan06.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lm.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lt.9csxet.cn

[A17] 位运算
来源：http://ye.chemitech.net.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jg.szxytkj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nb.huanxung.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wm.bookmarksfly.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://og.hahajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eu.yuntaijiaju.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://em.lnxyls.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dk.huixinmuqiang.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zk.hahajie.cn

[A18] 字符与 ASCII 码互转
来源：http://yt.huanxung.cn

Py:   ord("A"); chr(65)
来源：http://sc.yuntaijiaju.cn

PHP:  ord("A"); chr(65)
来源：http://pq.szsharing.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zg.szxytkj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ev.huixinmuqiang.cn

Java: (int) 'A'; (char) 65
来源：http://qs.muxihuayi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dg.huixiangedu.cn

Ruby: "A".ord; 65.chr
来源：http://ho.jctech888.com.cn

C#:   (int)'A'; (char)65
来源：http://md.bjjhwx.cn

[A19] 交换两个变量
来源：http://sb.muxihuayi.cn

Py:   a, b = b, a
来源：http://yu.shtwfgs.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://br.521024.cn

JS:   [a, b] = [b, a];
来源：http://qj.gzmigu.cn

TS:   [a, b] = [b, a];
来源：http://ws.colortex.cn

Java: int t = a; a = b; b = t;
来源：http://tg.szsharing.cn

Go:   a, b = b, a
来源：http://jg.shxzukj.cn

Ruby: a, b = b, a
来源：http://aq.bookmarksfly.cn

C#:   (a, b) = (b, a);
来源：http://uf.lnxyls.cn

[A20] 读取标准输入
来源：http://fj.muxihuayi.cn

Py:   name = input("请输入：")
来源：http://rg.jianghongdianzi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://nb.huanxung.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nv.hahajie.cn

TS:   // Node.js：readline 模块
来源：http://gh.asd995.cn

Java: new Scanner(System.in).nextLine()
来源：http://ei.hnjuh.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ae.gzmigu.cn

Ruby: gets.chomp
来源：http://yx.colortex.cn

C#:   Console.ReadLine();
来源：http://kx.lnxyls.cn

[A21] 保留指定小数位输出
来源：http://pb.yuexingan06.cn

Py:   f"{3.14159:.2f}"
来源：http://ad.hahajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qk.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://tr.chemitech.net.cn

TS:   (3.14159).toFixed(2)
来源：http://qy.chemitech.net.cn

Java: String.format("%.2f", 3.14159)
来源：http://yb.jianghongdianzi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qz.muxihuayi.cn

Ruby: format("%.2f", 3.14159)
来源：http://ba.yuntaijiaju.cn

C#:   3.14159.ToString("F2")
来源：http://da.yuntaijiaju.cn

[A22] 获取字符串长度
来源：http://nn.panjiajie.cn

Py:   len(s)
来源：http://ff.shxzukj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hc.521024.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kd.nszjky.cn

TS:   s.length
来源：http://qb.hahajie.cn

Java: s.length()
来源：http://vm.asd995.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jm.wgjwhj.cn

Ruby: s.length
来源：http://lt.jctech888.com.cn

C#:   s.Length
来源：http://es.yuntaijiaju.cn

[A23] 大小写转换
来源：http://js.jianghongdianzi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://mj.jianghongdianzi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gi.huixinmuqiang.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yl.hahajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qx.panjiajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fh.haigaiapp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jl.nicolike.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qi.bookmarksfly.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vc.newstarts.cn

[A24] 去除首尾空白
来源：http://ch.newstarts.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sr.bjjhwx.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pz.szsharing.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://om.panjiajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ja.gzmigu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yj.nszjky.cn

Go:   strings.TrimSpace(s)
来源：http://di.yuntaijiaju.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yr.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zv.muxihuayi.cn

[A25] 字符串比较
来源：http://kg.bjjhwx.cn

Py:   s1 == s2; s1 != s2
来源：http://wv.bookmarksfly.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mr.521024.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://oy.hahajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://um.shxzukj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://we.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zd.shxzskj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vr.bjjhwx.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xs.shtwfgs.cn

[A26] 类型转换总览
来源：http://dq.newstarts.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pw.shxzukj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://oz.bookmarksfly.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://iw.panjiajie.cn

TS:   Number() String() Boolean() x as number
来源：http://om.asd995.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bg.chemitech.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://on.huanxung.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://id.nszjky.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ob.asd995.cn

================================================================================
来源：http://fn.hahajie.cn

B. 流程控制
来源：http://vd.gzmigu.cn

================================================================================
来源：http://rc.shxzskj.cn

[B01] 条件判断 if / else
来源：http://it.szxytkj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dg.shxzskj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://iu.jianghongdianzi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xu.hahajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fa.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://su.chemitech.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://en.szxytkj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vh.521024.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rg.jianghongdianzi.cn

[B02] 多分支 else if / elif
来源：http://gl.shtwfgs.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tn.bookmarksfly.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yr.huanxung.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zv.gzmigu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cn.huanxung.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zj.nicolike.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dp.huixinmuqiang.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ui.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ej.newstarts.cn

[B03] switch / match / case
来源：http://bz.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mu.asd995.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://du.nszjky.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tf.wgjwhj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qm.lnxyls.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hr.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sb.panjiajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bd.haigaiapp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://td.panjiajie.cn

[B04] for 计数循环
来源：http://gt.yuntaijiaju.cn

Py:   for i in range(10): print(i)
来源：http://kk.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wg.wgjwhj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hj.hnjuh.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vf.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pk.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rw.wgjwhj.cn

Ruby: 10.times { |i| puts i }
来源：http://bt.lnxyls.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lu.asd995.cn

[B05] 遍历数组 / 列表
来源：http://ji.nszjky.cn

Py:   for item in arr: print(item)
来源：http://bg.hnjuh.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gf.panjiajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rs.shxzskj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://um.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zc.colortex.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rn.asd995.cn

Ruby: arr.each { |item| puts item }
来源：http://gc.jctech888.com.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://eu.muxihuayi.cn

[B06] 遍历字典 / 对象
来源：http://dd.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ba.nicolike.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zj.jianghongdianzi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nt.haigaiapp.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nx.lnxyls.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rp.yuexingan06.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fj.huanxung.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pp.nicolike.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zm.hnjuh.cn

[B07] while 循环
来源：http://ex.szsharing.cn

Py:   while i < 10: i += 1
来源：http://vi.hahajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mu.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://gq.bookmarksfly.cn

TS:   while (i < 10) { i++; }
来源：http://qg.szxytkj.cn

Java: while (i < 10) { i++; }
来源：http://yk.nicolike.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sy.lnxyls.cn

Ruby: while i < 10; i += 1; end
来源：http://xs.huixinmuqiang.cn

C#:   while (i < 10) { i++; }
来源：http://eg.huanxung.cn

[B08] do-while（至少执行一次）
来源：http://ao.szsharing.cn

Py:   # 无 do-while：用 while True + break
来源：http://vo.huixinmuqiang.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ok.huixiangedu.cn

JS:   do { i++; } while (i < 10);
来源：http://jz.huixiangedu.cn

TS:   do { i++; } while (i < 10);
来源：http://qa.huixinmuqiang.cn

Java: do { i++; } while (i < 10);
来源：http://pq.jianghongdianzi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tm.521024.cn

Ruby: begin; i += 1; end while i < 10
来源：http://re.yuexingan06.cn

C#:   do { i++; } while (i < 10);
来源：http://jq.panjiajie.cn

[B09] break 与 continue
来源：http://ha.newstarts.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gy.huixinmuqiang.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://iy.521024.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zx.hnjuh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xu.nicolike.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tr.newstarts.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oz.huanxung.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://do.huixinmuqiang.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qa.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://yx.panjiajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://oi.9csxet.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yn.yuexingan06.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xf.nicolike.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qt.yuntaijiaju.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vl.nszjky.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://va.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yc.bjjhwx.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tb.lnxyls.cn

[B11] 生成数字序列 / 区间
来源：http://tr.9csxet.cn

Py:   list(range(0, 10, 2))
来源：http://pb.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://gb.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hr.huixiangedu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fk.gzmigu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yo.panjiajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kp.muxihuayi.cn

Ruby: (0...10).step(2).to_a
来源：http://xs.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zq.szsharing.cn

[B12] 跳出多层循环
来源：http://bp.yuntaijiaju.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://on.szxytkj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gt.jctech888.com.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ip.newstarts.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ah.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xr.huanxung.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://up.jctech888.com.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pk.shtwfgs.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tw.huixiangedu.cn

[B13] 判断是否为数字
来源：http://wh.szxytkj.cn

Py:   isinstance(x, (int, float))
来源：http://xj.yuexingan06.cn

PHP:  is_numeric($x)
来源：http://mx.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uv.yuntaijiaju.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oa.nszjky.cn

Java: x instanceof Number
来源：http://ue.szxytkj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lt.szsharing.cn

Ruby: x.is_a?(Numeric)
来源：http://jj.nszjky.cn

C#:   x is int or double or decimal
来源：http://qf.chemitech.net.cn

[B14] 判断值是否在集合内
来源：http://bp.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ts.huanxung.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fh.hnjuh.cn

JS:   [1, 2, 3].includes(x)
来源：http://kk.nicolike.cn

TS:   [1, 2, 3].includes(x)
来源：http://pu.shtwfgs.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ws.huixiangedu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gg.yuexingan06.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fa.shxzukj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mh.hnjuh.cn

[B15] 布尔运算与取反
来源：http://dr.huanxung.cn

Py:   a and b or not c
来源：http://ob.wgjwhj.cn


<!-- 参考信息 -->