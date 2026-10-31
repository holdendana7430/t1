代发 wailian999

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://eg.yuexingan06.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ak.wgjwhj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ya.shxzskj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sy.szsharing.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lb.wgjwhj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://zf.yuexingan06.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://di.huixiangedu.cn

[A09] 绝对值与最大最小值
来源：http://nj.shxzskj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ik.nicolike.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wc.lnxyls.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rv.lnxyls.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bt.muxihuayi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xb.colortex.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wz.wgjwhj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dr.chemitech.net.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ju.nszjky.cn

[A10] 生成随机数
来源：http://ov.yuexingan06.cn

Py:   import random; random.randint(1, 100)
来源：http://ey.9csxet.cn

PHP:  random_int(1, 100);
来源：http://ub.bjjhwx.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://om.asd995.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://yi.bjjhwx.cn

Java: new Random().nextInt(100) + 1
来源：http://cl.yuexingan06.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yw.9csxet.cn

Ruby: rand(1..100)
来源：http://wk.shxzskj.cn

C#:   new Random().Next(1, 101)
来源：http://id.wgjwhj.cn

[A11] 条件表达式（三元）
来源：http://nl.shxzskj.cn

Py:   "yes" if x > 0 else "no"
来源：http://ux.bjjhwx.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://uh.hnjuh.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ak.panjiajie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://nq.chemitech.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://lu.chemitech.net.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://nh.muxihuayi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://tu.haigaiapp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://oz.jctech888.com.cn

[A12] 字符串插值 / 格式化
来源：http://yo.hnjuh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vk.huixiangedu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ja.gzmigu.cn

JS:   `Hello, ${name}!`
来源：http://fm.hnjuh.cn

TS:   `Hello, ${name}!`
来源：http://si.huixiangedu.cn

Java: "Hello, %s!".formatted(name)
来源：http://cs.newstarts.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sx.szsharing.cn

Ruby: "Hello, #{name}!"
来源：http://qn.hahajie.cn

C#:   $"Hello, {name}!"
来源：http://cj.shtwfgs.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://de.newstarts.cn

Py:   "第一行\n第二行"
来源：http://tv.lnxyls.cn

PHP:  "第一行\n第二行"
来源：http://xq.huixiangedu.cn

JS:   "第一行\n第二行"
来源：http://lg.nszjky.cn

TS:   "第一行\n第二行"
来源：http://wc.shxzskj.cn

Java: "第一行\n第二行"
来源：http://im.jctech888.com.cn

Go:   "第一行\n第二行"
来源：http://ds.newstarts.cn

Ruby: "第一行\n第二行"
来源：http://nl.shxzskj.cn

C#:   "第一行\n第二行"
来源：http://oo.jctech888.com.cn

[A14] 注释写法
来源：http://ww.jianghongdianzi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ck.9csxet.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://vh.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://bx.9csxet.cn

TS:   // 单行；/* 多行 */
来源：http://yz.huixinmuqiang.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gd.haigaiapp.cn

Go:   // 单行；/* 多行 */
来源：http://sr.shxzukj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://fr.hnjuh.cn

C#:   // 单行；/* 多行 */
来源：http://cp.9csxet.cn

[A15] 空值判断与默认值
来源：http://ej.szsharing.cn

Py:   value = data or "默认值"
来源：http://qb.bookmarksfly.cn

PHP:  $value = $data ?? "默认值";
来源：http://wo.newstarts.cn

JS:   const value = data ?? "默认值";
来源：http://ou.huixinmuqiang.cn

TS:   const value = data ?? "默认值";
来源：http://qr.shtwfgs.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dg.521024.cn

Go:   if data == "" { data = "默认值" }
来源：http://qu.521024.cn

Ruby: value = data || "默认值"
来源：http://qp.szxytkj.cn

C#:   var value = data ?? "默认值";
来源：http://iw.panjiajie.cn

[A16] 真假值判断规则
来源：http://lo.haigaiapp.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mz.hahajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hg.jianghongdianzi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://te.wgjwhj.cn

TS:   if (!x) {}
来源：http://ks.huixinmuqiang.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dj.bookmarksfly.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dx.shxzukj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://dc.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bq.9csxet.cn

[A17] 位运算
来源：http://ki.jctech888.com.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://la.521024.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ns.hahajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pa.newstarts.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qv.muxihuayi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tg.shxzukj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ak.muxihuayi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lf.szxytkj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ax.muxihuayi.cn

[A18] 字符与 ASCII 码互转
来源：http://ta.colortex.cn

Py:   ord("A"); chr(65)
来源：http://se.szxytkj.cn

PHP:  ord("A"); chr(65)
来源：http://up.nicolike.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jk.nicolike.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://av.jctech888.com.cn

Java: (int) 'A'; (char) 65
来源：http://ch.yuntaijiaju.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ql.bookmarksfly.cn

Ruby: "A".ord; 65.chr
来源：http://qt.panjiajie.cn

C#:   (int)'A'; (char)65
来源：http://wk.bjjhwx.cn

[A19] 交换两个变量
来源：http://vf.muxihuayi.cn

Py:   a, b = b, a
来源：http://gg.newstarts.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tc.szsharing.cn

JS:   [a, b] = [b, a];
来源：http://xs.521024.cn

TS:   [a, b] = [b, a];
来源：http://rb.hahajie.cn

Java: int t = a; a = b; b = t;
来源：http://kb.jctech888.com.cn

Go:   a, b = b, a
来源：http://tq.shtwfgs.cn

Ruby: a, b = b, a
来源：http://cr.521024.cn

C#:   (a, b) = (b, a);
来源：http://bu.haigaiapp.cn

[A20] 读取标准输入
来源：http://eb.szsharing.cn

Py:   name = input("请输入：")
来源：http://nh.newstarts.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://li.asd995.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ys.szxytkj.cn

TS:   // Node.js：readline 模块
来源：http://xh.nszjky.cn

Java: new Scanner(System.in).nextLine()
来源：http://us.huanxung.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://at.chemitech.net.cn

Ruby: gets.chomp
来源：http://ts.hahajie.cn

C#:   Console.ReadLine();
来源：http://hv.jctech888.com.cn

[A21] 保留指定小数位输出
来源：http://dy.shtwfgs.cn

Py:   f"{3.14159:.2f}"
来源：http://er.huixiangedu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rv.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://nw.9csxet.cn

TS:   (3.14159).toFixed(2)
来源：http://ca.haigaiapp.cn

Java: String.format("%.2f", 3.14159)
来源：http://ml.wgjwhj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dc.huixiangedu.cn

Ruby: format("%.2f", 3.14159)
来源：http://ke.newstarts.cn

C#:   3.14159.ToString("F2")
来源：http://zi.gzmigu.cn

[A22] 获取字符串长度
来源：http://xq.chemitech.net.cn

Py:   len(s)
来源：http://ww.bjjhwx.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ej.szxytkj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ly.9csxet.cn

TS:   s.length
来源：http://te.bjjhwx.cn

Java: s.length()
来源：http://el.huixiangedu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hy.shxzukj.cn

Ruby: s.length
来源：http://tz.9csxet.cn

C#:   s.Length
来源：http://yx.gzmigu.cn

[A23] 大小写转换
来源：http://wi.lnxyls.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://va.newstarts.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ju.muxihuayi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pt.jianghongdianzi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ky.huanxung.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vq.shxzukj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gn.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://js.huanxung.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jy.wgjwhj.cn

[A24] 去除首尾空白
来源：http://xk.nicolike.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://la.szsharing.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jt.asd995.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mr.szxytkj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jf.jianghongdianzi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://px.szxytkj.cn

Go:   strings.TrimSpace(s)
来源：http://xg.yuntaijiaju.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gx.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jc.lnxyls.cn

[A25] 字符串比较
来源：http://pq.asd995.cn

Py:   s1 == s2; s1 != s2
来源：http://my.szxytkj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gh.lnxyls.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rr.colortex.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lz.chemitech.net.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ai.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ta.asd995.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://io.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ai.huanxung.cn

[A26] 类型转换总览
来源：http://oi.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uv.newstarts.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://eh.colortex.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://eg.szxytkj.cn

TS:   Number() String() Boolean() x as number
来源：http://rn.huixiangedu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://da.hnjuh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ax.chemitech.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://by.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://oo.9csxet.cn

================================================================================
来源：http://tr.asd995.cn

B. 流程控制
来源：http://zl.chemitech.net.cn

================================================================================
来源：http://mn.bookmarksfly.cn

[B01] 条件判断 if / else
来源：http://pf.bookmarksfly.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qr.9csxet.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://th.yuntaijiaju.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dg.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dw.bookmarksfly.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ls.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qn.lnxyls.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fc.shtwfgs.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://li.huanxung.cn

[B02] 多分支 else if / elif
来源：http://ww.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ef.lnxyls.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vm.shxzskj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yq.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ci.hnjuh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rc.muxihuayi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dj.asd995.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lv.bjjhwx.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dz.jianghongdianzi.cn

[B03] switch / match / case
来源：http://xc.colortex.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yc.panjiajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rn.szsharing.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qp.colortex.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xv.asd995.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xm.haigaiapp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ii.panjiajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xg.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xu.huixinmuqiang.cn

[B04] for 计数循环
来源：http://ob.521024.cn

Py:   for i in range(10): print(i)
来源：http://nm.shxzskj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ku.shxzskj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vi.lnxyls.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qy.521024.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pm.jctech888.com.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xw.jctech888.com.cn

Ruby: 10.times { |i| puts i }
来源：http://kj.bookmarksfly.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fr.colortex.cn

[B05] 遍历数组 / 列表
来源：http://am.yuntaijiaju.cn

Py:   for item in arr: print(item)
来源：http://ud.newstarts.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://eg.nszjky.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tr.asd995.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cv.521024.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lp.muxihuayi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zp.jctech888.com.cn

Ruby: arr.each { |item| puts item }
来源：http://kw.shxzskj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kn.shtwfgs.cn

[B06] 遍历字典 / 对象
来源：http://zt.huanxung.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hq.colortex.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ne.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ru.yuntaijiaju.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ef.yuexingan06.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sw.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zf.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jv.jianghongdianzi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tw.gzmigu.cn

[B07] while 循环
来源：http://hl.9csxet.cn

Py:   while i < 10: i += 1
来源：http://yf.asd995.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yh.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://rw.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://ls.shxzukj.cn

Java: while (i < 10) { i++; }
来源：http://tp.jianghongdianzi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pt.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://om.jctech888.com.cn

C#:   while (i < 10) { i++; }
来源：http://mm.9csxet.cn

[B08] do-while（至少执行一次）
来源：http://xy.yuntaijiaju.cn

Py:   # 无 do-while：用 while True + break
来源：http://iy.521024.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ws.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://sm.chemitech.net.cn

TS:   do { i++; } while (i < 10);
来源：http://jv.szxytkj.cn

Java: do { i++; } while (i < 10);
来源：http://fi.jctech888.com.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tv.shxzukj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cr.huixiangedu.cn

C#:   do { i++; } while (i < 10);
来源：http://zc.huixinmuqiang.cn

[B09] break 与 continue
来源：http://lm.muxihuayi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cc.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://th.bookmarksfly.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cs.bjjhwx.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yy.hahajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://he.panjiajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sy.asd995.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wr.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cw.jianghongdianzi.cn

[B10] 遍历同时拿索引
来源：http://sl.jctech888.com.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://no.jianghongdianzi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wj.shxzukj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pb.newstarts.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kb.hnjuh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qi.nicolike.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ot.panjiajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kl.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cy.colortex.cn

[B11] 生成数字序列 / 区间
来源：http://yx.521024.cn

Py:   list(range(0, 10, 2))
来源：http://pi.wgjwhj.cn

PHP:  range(0, 10, 2);
来源：http://xn.bookmarksfly.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fz.panjiajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vp.nszjky.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rt.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vr.hnjuh.cn

Ruby: (0...10).step(2).to_a
来源：http://ru.bjjhwx.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zn.9csxet.cn

[B12] 跳出多层循环
来源：http://vh.yuntaijiaju.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://no.yuexingan06.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://st.bjjhwx.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dd.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://au.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://st.yuexingan06.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://eh.bookmarksfly.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://av.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dt.9csxet.cn

[B13] 判断是否为数字
来源：http://ip.bookmarksfly.cn

Py:   isinstance(x, (int, float))
来源：http://nu.hnjuh.cn

PHP:  is_numeric($x)
来源：http://mh.yuntaijiaju.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vk.521024.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bv.huixiangedu.cn

Java: x instanceof Number
来源：http://wz.yuntaijiaju.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ql.asd995.cn

Ruby: x.is_a?(Numeric)
来源：http://vv.bjjhwx.cn

C#:   x is int or double or decimal
来源：http://mm.nicolike.cn

[B14] 判断值是否在集合内
来源：http://ib.huixiangedu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ga.nicolike.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lw.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://yr.nszjky.cn

TS:   [1, 2, 3].includes(x)
来源：http://je.szxytkj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://km.shxzukj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ij.lnxyls.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fj.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ti.szxytkj.cn

[B15] 布尔运算与取反
来源：http://we.huixinmuqiang.cn

Py:   a and b or not c
来源：http://kb.muxihuayi.cn


<!-- 参考信息 -->