代发 wailian999

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xz.shtwfgs.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ww.hnjuh.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yr.yuexingan06.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ys.yuexingan06.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yj.yuntaijiaju.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://wg.shtwfgs.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bx.yuexingan06.cn

[A09] 绝对值与最大最小值
来源：http://yb.nicolike.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://sf.9csxet.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cu.hahajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rk.shtwfgs.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yu.nicolike.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pk.gzmigu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jl.muxihuayi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nn.shtwfgs.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kp.bookmarksfly.cn

[A10] 生成随机数
来源：http://hh.jctech888.com.cn

Py:   import random; random.randint(1, 100)
来源：http://jq.hahajie.cn

PHP:  random_int(1, 100);
来源：http://gy.huixinmuqiang.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ki.shxzukj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fq.szsharing.cn

Java: new Random().nextInt(100) + 1
来源：http://oa.huixiangedu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pe.bjjhwx.cn

Ruby: rand(1..100)
来源：http://vr.chemitech.net.cn

C#:   new Random().Next(1, 101)
来源：http://fp.yuntaijiaju.cn

[A11] 条件表达式（三元）
来源：http://lv.lnxyls.cn

Py:   "yes" if x > 0 else "no"
来源：http://oe.yuntaijiaju.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://vo.haigaiapp.cn

JS:   x > 0 ? "yes" : "no"
来源：http://mv.shxzukj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://cd.yuntaijiaju.cn

Java: x > 0 ? "yes" : "no"
来源：http://ft.huixiangedu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://hb.jctech888.com.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ue.9csxet.cn

C#:   x > 0 ? "yes" : "no"
来源：http://wd.9csxet.cn

[A12] 字符串插值 / 格式化
来源：http://ik.gzmigu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ot.colortex.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rh.szsharing.cn

JS:   `Hello, ${name}!`
来源：http://gs.asd995.cn

TS:   `Hello, ${name}!`
来源：http://zf.521024.cn

Java: "Hello, %s!".formatted(name)
来源：http://nc.haigaiapp.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hy.9csxet.cn

Ruby: "Hello, #{name}!"
来源：http://zi.shtwfgs.cn

C#:   $"Hello, {name}!"
来源：http://ek.hnjuh.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://mj.huixiangedu.cn

Py:   "第一行\n第二行"
来源：http://sa.asd995.cn

PHP:  "第一行\n第二行"
来源：http://am.yuexingan06.cn

JS:   "第一行\n第二行"
来源：http://rs.hnjuh.cn

TS:   "第一行\n第二行"
来源：http://gf.huixinmuqiang.cn

Java: "第一行\n第二行"
来源：http://ki.panjiajie.cn

Go:   "第一行\n第二行"
来源：http://vf.newstarts.cn

Ruby: "第一行\n第二行"
来源：http://py.colortex.cn

C#:   "第一行\n第二行"
来源：http://lq.9csxet.cn

[A14] 注释写法
来源：http://pq.huixiangedu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://em.nicolike.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://sd.hnjuh.cn

JS:   // 单行；/* 多行 */
来源：http://ws.shxzskj.cn

TS:   // 单行；/* 多行 */
来源：http://cf.hnjuh.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xz.bjjhwx.cn

Go:   // 单行；/* 多行 */
来源：http://iv.wgjwhj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://kj.chemitech.net.cn

C#:   // 单行；/* 多行 */
来源：http://gm.jianghongdianzi.cn

[A15] 空值判断与默认值
来源：http://dk.yuexingan06.cn

Py:   value = data or "默认值"
来源：http://zv.lnxyls.cn

PHP:  $value = $data ?? "默认值";
来源：http://pw.colortex.cn

JS:   const value = data ?? "默认值";
来源：http://qn.jianghongdianzi.cn

TS:   const value = data ?? "默认值";
来源：http://hz.gzmigu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zf.chemitech.net.cn

Go:   if data == "" { data = "默认值" }
来源：http://sg.newstarts.cn

Ruby: value = data || "默认值"
来源：http://bi.521024.cn

C#:   var value = data ?? "默认值";
来源：http://qq.huanxung.cn

[A16] 真假值判断规则
来源：http://gy.huixinmuqiang.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jj.huixiangedu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://td.nicolike.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fy.nicolike.cn

TS:   if (!x) {}
来源：http://jy.gzmigu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lo.colortex.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tw.hahajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lc.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tg.jianghongdianzi.cn

[A17] 位运算
来源：http://jh.yuntaijiaju.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hp.yuntaijiaju.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hw.huanxung.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gb.9csxet.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tm.huixinmuqiang.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ry.gzmigu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wq.nszjky.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rz.panjiajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://je.szxytkj.cn

[A18] 字符与 ASCII 码互转
来源：http://ri.newstarts.cn

Py:   ord("A"); chr(65)
来源：http://og.huixinmuqiang.cn

PHP:  ord("A"); chr(65)
来源：http://wj.muxihuayi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kr.jctech888.com.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hk.nszjky.cn

Java: (int) 'A'; (char) 65
来源：http://jm.nszjky.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ev.nszjky.cn

Ruby: "A".ord; 65.chr
来源：http://dx.newstarts.cn

C#:   (int)'A'; (char)65
来源：http://jk.9csxet.cn

[A19] 交换两个变量
来源：http://vh.wgjwhj.cn

Py:   a, b = b, a
来源：http://np.shxzukj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://gc.asd995.cn

JS:   [a, b] = [b, a];
来源：http://ac.521024.cn

TS:   [a, b] = [b, a];
来源：http://cq.bookmarksfly.cn

Java: int t = a; a = b; b = t;
来源：http://po.panjiajie.cn

Go:   a, b = b, a
来源：http://od.shxzukj.cn

Ruby: a, b = b, a
来源：http://cw.szxytkj.cn

C#:   (a, b) = (b, a);
来源：http://dw.9csxet.cn

[A20] 读取标准输入
来源：http://jw.asd995.cn

Py:   name = input("请输入：")
来源：http://hb.hnjuh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://vv.bookmarksfly.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xp.huanxung.cn

TS:   // Node.js：readline 模块
来源：http://wv.shtwfgs.cn

Java: new Scanner(System.in).nextLine()
来源：http://gl.szsharing.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bb.chemitech.net.cn

Ruby: gets.chomp
来源：http://yo.bjjhwx.cn

C#:   Console.ReadLine();
来源：http://mc.9csxet.cn

[A21] 保留指定小数位输出
来源：http://ax.panjiajie.cn

Py:   f"{3.14159:.2f}"
来源：http://sn.newstarts.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bi.bookmarksfly.cn

JS:   (3.14159).toFixed(2)
来源：http://qd.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://af.shtwfgs.cn

Java: String.format("%.2f", 3.14159)
来源：http://je.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fn.hahajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://gg.chemitech.net.cn

C#:   3.14159.ToString("F2")
来源：http://oq.nicolike.cn

[A22] 获取字符串长度
来源：http://yg.lnxyls.cn

Py:   len(s)
来源：http://vs.gzmigu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gv.nszjky.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ei.colortex.cn

TS:   s.length
来源：http://tl.huixiangedu.cn

Java: s.length()
来源：http://qi.chemitech.net.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jz.szsharing.cn

Ruby: s.length
来源：http://yk.panjiajie.cn

C#:   s.Length
来源：http://dd.bookmarksfly.cn

[A23] 大小写转换
来源：http://bt.panjiajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rh.huixiangedu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ic.szxytkj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://np.bookmarksfly.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ob.szsharing.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cw.lnxyls.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pg.wgjwhj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lu.huixinmuqiang.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jl.shxzskj.cn

[A24] 去除首尾空白
来源：http://wy.yuexingan06.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zy.shxzukj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ni.nicolike.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wc.szsharing.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fr.shtwfgs.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qz.lnxyls.cn

Go:   strings.TrimSpace(s)
来源：http://hb.panjiajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qs.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ax.nicolike.cn

[A25] 字符串比较
来源：http://aw.shtwfgs.cn

Py:   s1 == s2; s1 != s2
来源：http://fb.asd995.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lk.bjjhwx.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pd.jctech888.com.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kq.asd995.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sh.yuexingan06.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vm.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://au.haigaiapp.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://up.gzmigu.cn

[A26] 类型转换总览
来源：http://or.shtwfgs.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yl.szxytkj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wv.nszjky.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uo.shtwfgs.cn

TS:   Number() String() Boolean() x as number
来源：http://vq.9csxet.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zm.bookmarksfly.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://in.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://gr.szxytkj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fk.yuexingan06.cn

================================================================================
来源：http://na.hahajie.cn

B. 流程控制
来源：http://to.lnxyls.cn

================================================================================
来源：http://gz.jianghongdianzi.cn

[B01] 条件判断 if / else
来源：http://gx.colortex.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ms.shtwfgs.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zh.bjjhwx.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sk.nicolike.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cl.jctech888.com.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://by.nicolike.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lw.wgjwhj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qi.szsharing.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cl.nszjky.cn

[B02] 多分支 else if / elif
来源：http://ux.yuexingan06.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zo.colortex.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tu.muxihuayi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cu.hnjuh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tf.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bx.jianghongdianzi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jm.nszjky.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://er.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lo.huixinmuqiang.cn

[B03] switch / match / case
来源：http://gd.newstarts.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://eg.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oy.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mg.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gr.wgjwhj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ct.muxihuayi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://va.muxihuayi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xq.shxzskj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mf.bjjhwx.cn

[B04] for 计数循环
来源：http://mx.huanxung.cn

Py:   for i in range(10): print(i)
来源：http://xp.lnxyls.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zf.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rh.szsharing.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rj.shxzskj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ew.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kj.521024.cn

Ruby: 10.times { |i| puts i }
来源：http://vf.huixiangedu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xd.asd995.cn

[B05] 遍历数组 / 列表
来源：http://hp.hnjuh.cn

Py:   for item in arr: print(item)
来源：http://wy.lnxyls.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dg.huanxung.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://js.panjiajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jr.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ed.yuexingan06.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xe.panjiajie.cn

Ruby: arr.each { |item| puts item }
来源：http://wn.9csxet.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jh.colortex.cn

[B06] 遍历字典 / 对象
来源：http://el.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ct.huixiangedu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ap.muxihuayi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cp.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://md.newstarts.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ly.jctech888.com.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://aq.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xz.newstarts.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rh.521024.cn

[B07] while 循环
来源：http://gd.9csxet.cn

Py:   while i < 10: i += 1
来源：http://om.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ci.521024.cn

JS:   while (i < 10) { i++; }
来源：http://bn.colortex.cn

TS:   while (i < 10) { i++; }
来源：http://ar.gzmigu.cn

Java: while (i < 10) { i++; }
来源：http://lj.asd995.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zb.asd995.cn

Ruby: while i < 10; i += 1; end
来源：http://zq.asd995.cn

C#:   while (i < 10) { i++; }
来源：http://ns.nszjky.cn

[B08] do-while（至少执行一次）
来源：http://qs.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://gm.jianghongdianzi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nx.yuexingan06.cn

JS:   do { i++; } while (i < 10);
来源：http://po.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://vj.hahajie.cn

Java: do { i++; } while (i < 10);
来源：http://tq.muxihuayi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bu.bookmarksfly.cn

Ruby: begin; i += 1; end while i < 10
来源：http://az.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://rr.9csxet.cn

[B09] break 与 continue
来源：http://dq.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vx.yuexingan06.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cd.yuexingan06.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ox.haigaiapp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://be.huixinmuqiang.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wo.muxihuayi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nn.newstarts.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bh.jianghongdianzi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://of.asd995.cn

[B10] 遍历同时拿索引
来源：http://vs.521024.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://va.hahajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kk.huixinmuqiang.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pa.huanxung.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ay.szxytkj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fi.wgjwhj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gz.yuexingan06.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rd.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zx.nicolike.cn

[B11] 生成数字序列 / 区间
来源：http://zo.521024.cn

Py:   list(range(0, 10, 2))
来源：http://ds.shxzskj.cn

PHP:  range(0, 10, 2);
来源：http://xj.wgjwhj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ck.lnxyls.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yn.huanxung.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fb.szxytkj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hs.lnxyls.cn

Ruby: (0...10).step(2).to_a
来源：http://ih.bjjhwx.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://aj.nszjky.cn

[B12] 跳出多层循环
来源：http://tq.wgjwhj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uj.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fh.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tn.hahajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tc.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wr.chemitech.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dp.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dg.lnxyls.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cq.jctech888.com.cn

[B13] 判断是否为数字
来源：http://as.bjjhwx.cn

Py:   isinstance(x, (int, float))
来源：http://yk.szsharing.cn

PHP:  is_numeric($x)
来源：http://ga.bookmarksfly.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vp.colortex.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xk.yuntaijiaju.cn

Java: x instanceof Number
来源：http://qd.bookmarksfly.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ul.chemitech.net.cn

Ruby: x.is_a?(Numeric)
来源：http://om.gzmigu.cn

C#:   x is int or double or decimal
来源：http://ss.nszjky.cn

[B14] 判断值是否在集合内
来源：http://rl.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bt.lnxyls.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lv.521024.cn

JS:   [1, 2, 3].includes(x)
来源：http://zc.jctech888.com.cn

TS:   [1, 2, 3].includes(x)
来源：http://yz.huixiangedu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jf.hnjuh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tx.lnxyls.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pt.chemitech.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://eg.hahajie.cn

[B15] 布尔运算与取反
来源：http://zy.huixiangedu.cn

Py:   a and b or not c
来源：http://vi.bookmarksfly.cn


<!-- 参考信息 -->