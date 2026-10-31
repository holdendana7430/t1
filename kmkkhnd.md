代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ec.haigaiapp.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tn.jctech888.com.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://la.wgjwhj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zr.yuexingan06.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ek.521024.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://iv.gzmigu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fm.yuntaijiaju.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xf.haigaiapp.cn

[A10] 生成随机数
来源：http://mz.yuexingan06.cn

Py:   import random; random.randint(1, 100)
来源：http://ba.shxzukj.cn

PHP:  random_int(1, 100);
来源：http://qo.lnxyls.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pn.huixinmuqiang.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cn.jctech888.com.cn

Java: new Random().nextInt(100) + 1
来源：http://ad.muxihuayi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pf.shtwfgs.cn

Ruby: rand(1..100)
来源：http://eh.szsharing.cn

C#:   new Random().Next(1, 101)
来源：http://pw.huanxung.cn

[A11] 条件表达式（三元）
来源：http://xv.szxytkj.cn

Py:   "yes" if x > 0 else "no"
来源：http://uy.haigaiapp.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://jd.szxytkj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://dv.shxzukj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://hd.9csxet.cn

Java: x > 0 ? "yes" : "no"
来源：http://ay.huanxung.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://pw.szxytkj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://cw.yuexingan06.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xz.shtwfgs.cn

[A12] 字符串插值 / 格式化
来源：http://hn.newstarts.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://yn.huixinmuqiang.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://dt.hnjuh.cn

JS:   `Hello, ${name}!`
来源：http://oy.huixinmuqiang.cn

TS:   `Hello, ${name}!`
来源：http://fd.nicolike.cn

Java: "Hello, %s!".formatted(name)
来源：http://ef.bookmarksfly.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gm.yuexingan06.cn

Ruby: "Hello, #{name}!"
来源：http://wo.bjjhwx.cn

C#:   $"Hello, {name}!"
来源：http://pp.lnxyls.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://bb.shxzukj.cn

Py:   "第一行\n第二行"
来源：http://kn.panjiajie.cn

PHP:  "第一行\n第二行"
来源：http://xc.huanxung.cn

JS:   "第一行\n第二行"
来源：http://kv.asd995.cn

TS:   "第一行\n第二行"
来源：http://ck.lnxyls.cn

Java: "第一行\n第二行"
来源：http://zg.lnxyls.cn

Go:   "第一行\n第二行"
来源：http://ec.szsharing.cn

Ruby: "第一行\n第二行"
来源：http://qw.yuntaijiaju.cn

C#:   "第一行\n第二行"
来源：http://kp.nszjky.cn

[A14] 注释写法
来源：http://ib.jianghongdianzi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://wj.asd995.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ri.jianghongdianzi.cn

JS:   // 单行；/* 多行 */
来源：http://ww.yuntaijiaju.cn

TS:   // 单行；/* 多行 */
来源：http://wy.muxihuayi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://la.chemitech.net.cn

Go:   // 单行；/* 多行 */
来源：http://op.panjiajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://iq.jianghongdianzi.cn

C#:   // 单行；/* 多行 */
来源：http://rl.huixiangedu.cn

[A15] 空值判断与默认值
来源：http://ww.9csxet.cn

Py:   value = data or "默认值"
来源：http://fd.yuexingan06.cn

PHP:  $value = $data ?? "默认值";
来源：http://jp.muxihuayi.cn

JS:   const value = data ?? "默认值";
来源：http://ee.bookmarksfly.cn

TS:   const value = data ?? "默认值";
来源：http://gp.asd995.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tq.nicolike.cn

Go:   if data == "" { data = "默认值" }
来源：http://vi.huanxung.cn

Ruby: value = data || "默认值"
来源：http://oo.9csxet.cn

C#:   var value = data ?? "默认值";
来源：http://on.521024.cn

[A16] 真假值判断规则
来源：http://ca.yuntaijiaju.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wm.asd995.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qs.jctech888.com.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sb.bookmarksfly.cn

TS:   if (!x) {}
来源：http://zz.szxytkj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dy.9csxet.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mw.colortex.cn

Ruby: unless x            # nil 与 false 为假
来源：http://fa.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ls.wgjwhj.cn

[A17] 位运算
来源：http://tv.szsharing.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uj.colortex.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lh.9csxet.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://na.bookmarksfly.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ml.nicolike.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tc.yuntaijiaju.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rh.521024.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yv.jianghongdianzi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hi.yuntaijiaju.cn

[A18] 字符与 ASCII 码互转
来源：http://ti.521024.cn

Py:   ord("A"); chr(65)
来源：http://bd.shxzukj.cn

PHP:  ord("A"); chr(65)
来源：http://qk.521024.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rk.huixiangedu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zm.szxytkj.cn

Java: (int) 'A'; (char) 65
来源：http://ft.jctech888.com.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bg.huanxung.cn

Ruby: "A".ord; 65.chr
来源：http://rh.newstarts.cn

C#:   (int)'A'; (char)65
来源：http://xt.lnxyls.cn

[A19] 交换两个变量
来源：http://vq.lnxyls.cn

Py:   a, b = b, a
来源：http://ir.lnxyls.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ge.newstarts.cn

JS:   [a, b] = [b, a];
来源：http://pt.bjjhwx.cn

TS:   [a, b] = [b, a];
来源：http://vs.colortex.cn

Java: int t = a; a = b; b = t;
来源：http://ce.asd995.cn

Go:   a, b = b, a
来源：http://ye.huixinmuqiang.cn

Ruby: a, b = b, a
来源：http://yf.521024.cn

C#:   (a, b) = (b, a);
来源：http://un.huixinmuqiang.cn

[A20] 读取标准输入
来源：http://ne.huixinmuqiang.cn

Py:   name = input("请输入：")
来源：http://fc.asd995.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ub.gzmigu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nk.shxzskj.cn

TS:   // Node.js：readline 模块
来源：http://ur.bookmarksfly.cn

Java: new Scanner(System.in).nextLine()
来源：http://ty.wgjwhj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vr.nicolike.cn

Ruby: gets.chomp
来源：http://ea.chemitech.net.cn

C#:   Console.ReadLine();
来源：http://tp.hahajie.cn

[A21] 保留指定小数位输出
来源：http://my.yuntaijiaju.cn

Py:   f"{3.14159:.2f}"
来源：http://zn.jianghongdianzi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ep.hahajie.cn

JS:   (3.14159).toFixed(2)
来源：http://bp.gzmigu.cn

TS:   (3.14159).toFixed(2)
来源：http://it.shxzskj.cn

Java: String.format("%.2f", 3.14159)
来源：http://hg.jianghongdianzi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gp.szsharing.cn

Ruby: format("%.2f", 3.14159)
来源：http://fa.yuexingan06.cn

C#:   3.14159.ToString("F2")
来源：http://jn.chemitech.net.cn

[A22] 获取字符串长度
来源：http://rd.wgjwhj.cn

Py:   len(s)
来源：http://zs.jctech888.com.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ea.gzmigu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ul.wgjwhj.cn

TS:   s.length
来源：http://sq.panjiajie.cn

Java: s.length()
来源：http://zh.wgjwhj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xw.bjjhwx.cn

Ruby: s.length
来源：http://it.yuntaijiaju.cn

C#:   s.Length
来源：http://os.yuexingan06.cn

[A23] 大小写转换
来源：http://vp.yuntaijiaju.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gs.bjjhwx.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mm.jctech888.com.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xu.szsharing.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ml.szsharing.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kb.yuntaijiaju.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sx.newstarts.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rn.yuexingan06.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nk.szsharing.cn

[A24] 去除首尾空白
来源：http://ga.chemitech.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pw.hahajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://et.hnjuh.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://as.yuntaijiaju.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nc.shxzskj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ow.shxzukj.cn

Go:   strings.TrimSpace(s)
来源：http://ri.shxzukj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yz.panjiajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nm.huixiangedu.cn

[A25] 字符串比较
来源：http://ok.bjjhwx.cn

Py:   s1 == s2; s1 != s2
来源：http://uh.nicolike.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zl.muxihuayi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nv.lnxyls.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vs.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://db.colortex.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vq.bjjhwx.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cm.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jg.haigaiapp.cn

[A26] 类型转换总览
来源：http://wm.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ck.bookmarksfly.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ko.muxihuayi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sz.bookmarksfly.cn

TS:   Number() String() Boolean() x as number
来源：http://fn.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yq.521024.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rs.wgjwhj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lp.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ig.yuntaijiaju.cn

================================================================================
来源：http://ct.muxihuayi.cn

B. 流程控制
来源：http://lr.asd995.cn

================================================================================
来源：http://gs.hahajie.cn

[B01] 条件判断 if / else
来源：http://ox.wgjwhj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://od.gzmigu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pb.szsharing.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zz.haigaiapp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hv.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bl.colortex.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xb.huanxung.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gu.asd995.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sp.yuexingan06.cn

[B02] 多分支 else if / elif
来源：http://xd.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ld.yuexingan06.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xn.bjjhwx.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tv.yuexingan06.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://av.gzmigu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ft.haigaiapp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lt.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sv.szxytkj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ud.muxihuayi.cn

[B03] switch / match / case
来源：http://tf.muxihuayi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uz.wgjwhj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sq.muxihuayi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rb.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jv.hnjuh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ln.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mu.shtwfgs.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fa.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fc.newstarts.cn

[B04] for 计数循环
来源：http://zi.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://fy.shxzukj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pe.chemitech.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ej.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ql.9csxet.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://id.lnxyls.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ma.chemitech.net.cn

Ruby: 10.times { |i| puts i }
来源：http://kt.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tg.bookmarksfly.cn

[B05] 遍历数组 / 列表
来源：http://uv.jctech888.com.cn

Py:   for item in arr: print(item)
来源：http://ia.hahajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gc.huixinmuqiang.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ud.shxzskj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jt.jctech888.com.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://be.szsharing.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gh.haigaiapp.cn

Ruby: arr.each { |item| puts item }
来源：http://ru.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fz.shxzskj.cn

[B06] 遍历字典 / 对象
来源：http://wh.nicolike.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://iz.huanxung.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nd.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vz.shxzskj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sh.shxzukj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lj.asd995.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ms.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nz.gzmigu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lc.nicolike.cn

[B07] while 循环
来源：http://xj.szsharing.cn

Py:   while i < 10: i += 1
来源：http://az.shxzukj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://aa.panjiajie.cn

JS:   while (i < 10) { i++; }
来源：http://kx.521024.cn

TS:   while (i < 10) { i++; }
来源：http://do.yuexingan06.cn

Java: while (i < 10) { i++; }
来源：http://cq.nicolike.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xl.bjjhwx.cn

Ruby: while i < 10; i += 1; end
来源：http://gi.wgjwhj.cn

C#:   while (i < 10) { i++; }
来源：http://qo.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://it.haigaiapp.cn

Py:   # 无 do-while：用 while True + break
来源：http://yi.yuexingan06.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xp.colortex.cn

JS:   do { i++; } while (i < 10);
来源：http://hl.newstarts.cn

TS:   do { i++; } while (i < 10);
来源：http://ne.chemitech.net.cn

Java: do { i++; } while (i < 10);
来源：http://hg.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hh.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ib.chemitech.net.cn

C#:   do { i++; } while (i < 10);
来源：http://th.jianghongdianzi.cn

[B09] break 与 continue
来源：http://is.haigaiapp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ht.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bf.yuntaijiaju.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ei.szsharing.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ox.shxzukj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vb.nszjky.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ha.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ii.lnxyls.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wv.bookmarksfly.cn

[B10] 遍历同时拿索引
来源：http://fy.lnxyls.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ml.nszjky.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ed.jctech888.com.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gk.huixiangedu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mo.chemitech.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gi.shxzukj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ge.wgjwhj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rv.jctech888.com.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xa.muxihuayi.cn

[B11] 生成数字序列 / 区间
来源：http://tr.colortex.cn

Py:   list(range(0, 10, 2))
来源：http://gy.wgjwhj.cn

PHP:  range(0, 10, 2);
来源：http://hf.yuntaijiaju.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fu.huixiangedu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ce.shtwfgs.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wr.shtwfgs.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ni.lnxyls.cn

Ruby: (0...10).step(2).to_a
来源：http://bl.9csxet.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ce.wgjwhj.cn

[B12] 跳出多层循环
来源：http://um.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kw.9csxet.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kf.asd995.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://je.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bp.shxzskj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pw.newstarts.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ft.newstarts.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kx.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ze.nicolike.cn

[B13] 判断是否为数字
来源：http://yg.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://lh.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://bo.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ht.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ww.lnxyls.cn

Java: x instanceof Number
来源：http://jh.newstarts.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://me.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://eq.shxzukj.cn

C#:   x is int or double or decimal
来源：http://if.bookmarksfly.cn

[B14] 判断值是否在集合内
来源：http://ed.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://up.newstarts.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fj.521024.cn

JS:   [1, 2, 3].includes(x)
来源：http://ly.bookmarksfly.cn

TS:   [1, 2, 3].includes(x)
来源：http://om.9csxet.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hv.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zc.szsharing.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ub.jianghongdianzi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bk.chemitech.net.cn

[B15] 布尔运算与取反
来源：http://hz.lnxyls.cn

Py:   a and b or not c
来源：http://tx.huanxung.cn

PHP:  $a && $b || !$c
来源：http://eo.newstarts.cn

JS:   a && b || !c
来源：http://ao.huanxung.cn

TS:   a && b || !c
来源：http://dp.szxytkj.cn

Java: a && b || !c
来源：http://py.haigaiapp.cn

Go:   a && b || !c
来源：http://rv.chemitech.net.cn

Ruby: a && b || !c
来源：http://hu.colortex.cn

C#:   a && b || !c
来源：http://pt.muxihuayi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mz.gzmigu.cn


<!-- 参考信息 -->