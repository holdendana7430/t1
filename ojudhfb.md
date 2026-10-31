代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://uw.huixiangedu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ky.nszjky.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dt.shtwfgs.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bt.colortex.cn

[A10] 生成随机数
来源：http://fn.huixiangedu.cn

Py:   import random; random.randint(1, 100)
来源：http://ex.asd995.cn

PHP:  random_int(1, 100);
来源：http://kx.huixiangedu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ex.nicolike.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kj.asd995.cn

Java: new Random().nextInt(100) + 1
来源：http://gr.shtwfgs.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hu.szsharing.cn

Ruby: rand(1..100)
来源：http://hk.nicolike.cn

C#:   new Random().Next(1, 101)
来源：http://bx.nicolike.cn

[A11] 条件表达式（三元）
来源：http://vc.jctech888.com.cn

Py:   "yes" if x > 0 else "no"
来源：http://hv.colortex.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://el.bookmarksfly.cn

JS:   x > 0 ? "yes" : "no"
来源：http://tq.lnxyls.cn

TS:   x > 0 ? "yes" : "no"
来源：http://jn.newstarts.cn

Java: x > 0 ? "yes" : "no"
来源：http://le.szsharing.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wo.shtwfgs.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ky.521024.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ki.shtwfgs.cn

[A12] 字符串插值 / 格式化
来源：http://jg.yuexingan06.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://sp.jianghongdianzi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pr.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://be.colortex.cn

TS:   `Hello, ${name}!`
来源：http://bv.521024.cn

Java: "Hello, %s!".formatted(name)
来源：http://oa.jctech888.com.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ib.shxzskj.cn

Ruby: "Hello, #{name}!"
来源：http://kc.haigaiapp.cn

C#:   $"Hello, {name}!"
来源：http://el.lnxyls.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ez.shxzskj.cn

Py:   "第一行\n第二行"
来源：http://qt.shtwfgs.cn

PHP:  "第一行\n第二行"
来源：http://ek.jctech888.com.cn

JS:   "第一行\n第二行"
来源：http://yl.wgjwhj.cn

TS:   "第一行\n第二行"
来源：http://rf.gzmigu.cn

Java: "第一行\n第二行"
来源：http://sh.gzmigu.cn

Go:   "第一行\n第二行"
来源：http://vd.bjjhwx.cn

Ruby: "第一行\n第二行"
来源：http://hg.jianghongdianzi.cn

C#:   "第一行\n第二行"
来源：http://ov.lnxyls.cn

[A14] 注释写法
来源：http://mp.szsharing.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://he.asd995.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://oi.asd995.cn

JS:   // 单行；/* 多行 */
来源：http://dw.panjiajie.cn

TS:   // 单行；/* 多行 */
来源：http://nh.yuntaijiaju.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://sk.shxzukj.cn

Go:   // 单行；/* 多行 */
来源：http://de.bjjhwx.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ce.bookmarksfly.cn

C#:   // 单行；/* 多行 */
来源：http://yw.szxytkj.cn

[A15] 空值判断与默认值
来源：http://yt.panjiajie.cn

Py:   value = data or "默认值"
来源：http://hj.szsharing.cn

PHP:  $value = $data ?? "默认值";
来源：http://we.jianghongdianzi.cn

JS:   const value = data ?? "默认值";
来源：http://ev.9csxet.cn

TS:   const value = data ?? "默认值";
来源：http://cu.jianghongdianzi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rj.wgjwhj.cn

Go:   if data == "" { data = "默认值" }
来源：http://qq.colortex.cn

Ruby: value = data || "默认值"
来源：http://xp.shxzskj.cn

C#:   var value = data ?? "默认值";
来源：http://rh.nszjky.cn

[A16] 真假值判断规则
来源：http://pg.jctech888.com.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lv.szsharing.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fg.hnjuh.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ys.jctech888.com.cn

TS:   if (!x) {}
来源：http://bs.wgjwhj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hp.jctech888.com.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tn.bookmarksfly.cn

Ruby: unless x            # nil 与 false 为假
来源：http://yx.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kb.gzmigu.cn

[A17] 位运算
来源：http://ja.huanxung.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lz.lnxyls.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ko.asd995.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gj.hnjuh.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xt.nszjky.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://na.asd995.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://db.bjjhwx.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://za.huixiangedu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oj.szsharing.cn

[A18] 字符与 ASCII 码互转
来源：http://wz.bjjhwx.cn

Py:   ord("A"); chr(65)
来源：http://tm.shxzskj.cn

PHP:  ord("A"); chr(65)
来源：http://vm.huixinmuqiang.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ib.yuexingan06.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://il.521024.cn

Java: (int) 'A'; (char) 65
来源：http://bz.521024.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tl.lnxyls.cn

Ruby: "A".ord; 65.chr
来源：http://jk.szsharing.cn

C#:   (int)'A'; (char)65
来源：http://jy.panjiajie.cn

[A19] 交换两个变量
来源：http://ct.yuntaijiaju.cn

Py:   a, b = b, a
来源：http://ws.muxihuayi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jw.hnjuh.cn

JS:   [a, b] = [b, a];
来源：http://jo.gzmigu.cn

TS:   [a, b] = [b, a];
来源：http://aj.bookmarksfly.cn

Java: int t = a; a = b; b = t;
来源：http://ah.asd995.cn

Go:   a, b = b, a
来源：http://eb.colortex.cn

Ruby: a, b = b, a
来源：http://ju.bjjhwx.cn

C#:   (a, b) = (b, a);
来源：http://ci.shxzukj.cn

[A20] 读取标准输入
来源：http://ny.haigaiapp.cn

Py:   name = input("请输入：")
来源：http://xl.gzmigu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zc.hahajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lv.huanxung.cn

TS:   // Node.js：readline 模块
来源：http://ib.huixiangedu.cn

Java: new Scanner(System.in).nextLine()
来源：http://fk.huixinmuqiang.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jl.muxihuayi.cn

Ruby: gets.chomp
来源：http://dm.gzmigu.cn

C#:   Console.ReadLine();
来源：http://wd.szxytkj.cn

[A21] 保留指定小数位输出
来源：http://tt.haigaiapp.cn

Py:   f"{3.14159:.2f}"
来源：http://ul.shxzukj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jn.szsharing.cn

JS:   (3.14159).toFixed(2)
来源：http://qq.bjjhwx.cn

TS:   (3.14159).toFixed(2)
来源：http://uf.haigaiapp.cn

Java: String.format("%.2f", 3.14159)
来源：http://rc.yuexingan06.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nz.hahajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://qr.lnxyls.cn

C#:   3.14159.ToString("F2")
来源：http://de.chemitech.net.cn

[A22] 获取字符串长度
来源：http://hz.wgjwhj.cn

Py:   len(s)
来源：http://rs.hnjuh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jn.asd995.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ea.jianghongdianzi.cn

TS:   s.length
来源：http://ez.szsharing.cn

Java: s.length()
来源：http://fy.9csxet.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ib.newstarts.cn

Ruby: s.length
来源：http://pe.jianghongdianzi.cn

C#:   s.Length
来源：http://rh.bjjhwx.cn

[A23] 大小写转换
来源：http://wh.hahajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://al.szxytkj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fk.huixinmuqiang.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ql.haigaiapp.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tl.hahajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ie.colortex.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mt.nicolike.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kr.nicolike.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://pm.muxihuayi.cn

[A24] 去除首尾空白
来源：http://js.521024.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fc.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wp.shxzskj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xg.szxytkj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bb.chemitech.net.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gu.huixiangedu.cn

Go:   strings.TrimSpace(s)
来源：http://xe.huanxung.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gx.huanxung.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jz.yuexingan06.cn

[A25] 字符串比较
来源：http://zg.521024.cn

Py:   s1 == s2; s1 != s2
来源：http://uu.muxihuayi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cp.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://an.huixiangedu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gi.shxzskj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bn.shtwfgs.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cf.muxihuayi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://al.colortex.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ux.panjiajie.cn

[A26] 类型转换总览
来源：http://no.521024.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qw.chemitech.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uz.bookmarksfly.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://eu.nszjky.cn

TS:   Number() String() Boolean() x as number
来源：http://if.bjjhwx.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://th.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ro.nicolike.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://xi.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ur.hahajie.cn

================================================================================
来源：http://nx.muxihuayi.cn

B. 流程控制
来源：http://nm.shxzukj.cn

================================================================================
来源：http://mn.newstarts.cn

[B01] 条件判断 if / else
来源：http://pm.9csxet.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ws.yuexingan06.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vi.nicolike.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dd.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gq.szxytkj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vt.wgjwhj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ea.nszjky.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vb.jctech888.com.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xc.szsharing.cn

[B02] 多分支 else if / elif
来源：http://df.muxihuayi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xl.9csxet.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ri.szxytkj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gs.haigaiapp.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://an.yuexingan06.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zy.szsharing.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tk.szsharing.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ea.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mg.szsharing.cn

[B03] switch / match / case
来源：http://sg.shtwfgs.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xp.hahajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kq.colortex.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cj.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cc.gzmigu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xz.haigaiapp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vv.panjiajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qd.panjiajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tn.szxytkj.cn

[B04] for 计数循环
来源：http://aw.panjiajie.cn

Py:   for i in range(10): print(i)
来源：http://vy.yuntaijiaju.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://au.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ed.muxihuayi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yw.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tm.hnjuh.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wu.newstarts.cn

Ruby: 10.times { |i| puts i }
来源：http://yk.huixiangedu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tb.yuexingan06.cn

[B05] 遍历数组 / 列表
来源：http://yb.9csxet.cn

Py:   for item in arr: print(item)
来源：http://ii.bjjhwx.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jv.colortex.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ip.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gi.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sl.521024.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kz.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://hj.huixiangedu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://as.colortex.cn

[B06] 遍历字典 / 对象
来源：http://cd.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zh.lnxyls.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nh.szsharing.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mh.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://to.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mo.huixinmuqiang.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vs.shtwfgs.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://br.muxihuayi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zq.nicolike.cn

[B07] while 循环
来源：http://mj.huixinmuqiang.cn

Py:   while i < 10: i += 1
来源：http://nt.bjjhwx.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zu.szxytkj.cn

JS:   while (i < 10) { i++; }
来源：http://dr.asd995.cn

TS:   while (i < 10) { i++; }
来源：http://yb.panjiajie.cn

Java: while (i < 10) { i++; }
来源：http://mo.haigaiapp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fo.9csxet.cn

Ruby: while i < 10; i += 1; end
来源：http://wl.szxytkj.cn

C#:   while (i < 10) { i++; }
来源：http://to.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://ea.huixiangedu.cn

Py:   # 无 do-while：用 while True + break
来源：http://es.yuexingan06.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zv.jctech888.com.cn

JS:   do { i++; } while (i < 10);
来源：http://mp.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://zx.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://iz.nicolike.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yy.szsharing.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mm.haigaiapp.cn

C#:   do { i++; } while (i < 10);
来源：http://nq.hnjuh.cn

[B09] break 与 continue
来源：http://jd.asd995.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tv.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xp.huanxung.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gv.521024.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://up.yuexingan06.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://id.nicolike.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ed.hahajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://re.huixiangedu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rb.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://dk.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qd.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ug.huixinmuqiang.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hp.yuexingan06.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ej.huixiangedu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sb.jctech888.com.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xt.gzmigu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dr.hnjuh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://iq.huixiangedu.cn

[B11] 生成数字序列 / 区间
来源：http://ks.huanxung.cn

Py:   list(range(0, 10, 2))
来源：http://nj.muxihuayi.cn

PHP:  range(0, 10, 2);
来源：http://od.szxytkj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bb.shxzukj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bl.lnxyls.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ai.gzmigu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jn.bookmarksfly.cn

Ruby: (0...10).step(2).to_a
来源：http://gc.jianghongdianzi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gp.bjjhwx.cn

[B12] 跳出多层循环
来源：http://qz.hahajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zc.asd995.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yh.521024.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uq.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fw.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lf.asd995.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dg.jctech888.com.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vz.haigaiapp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vj.panjiajie.cn

[B13] 判断是否为数字
来源：http://yv.bjjhwx.cn

Py:   isinstance(x, (int, float))
来源：http://xe.nicolike.cn

PHP:  is_numeric($x)
来源：http://ad.huanxung.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cd.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nq.yuntaijiaju.cn

Java: x instanceof Number
来源：http://ie.colortex.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vu.wgjwhj.cn

Ruby: x.is_a?(Numeric)
来源：http://if.shtwfgs.cn

C#:   x is int or double or decimal
来源：http://hg.gzmigu.cn

[B14] 判断值是否在集合内
来源：http://qk.szsharing.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://go.szxytkj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vn.haigaiapp.cn

JS:   [1, 2, 3].includes(x)
来源：http://rr.shtwfgs.cn

TS:   [1, 2, 3].includes(x)
来源：http://xp.chemitech.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rp.jctech888.com.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nq.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hj.lnxyls.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mo.yuntaijiaju.cn

[B15] 布尔运算与取反
来源：http://xu.nszjky.cn

Py:   a and b or not c
来源：http://cw.shtwfgs.cn

PHP:  $a && $b || !$c
来源：http://rg.panjiajie.cn

JS:   a && b || !c
来源：http://ta.bjjhwx.cn

TS:   a && b || !c
来源：http://kc.nicolike.cn

Java: a && b || !c
来源：http://tx.hahajie.cn

Go:   a && b || !c
来源：http://fy.yuntaijiaju.cn

Ruby: a && b || !c
来源：http://oc.gzmigu.cn

C#:   a && b || !c
来源：http://cp.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ot.nicolike.cn

Py:   if not data: return
来源：http://nm.521024.cn

PHP:  if (!$data) { return; }
来源：http://dp.chemitech.net.cn

JS:   if (!data) return;
来源：http://fj.huixinmuqiang.cn

TS:   if (!data) return;
来源：http://gv.huixinmuqiang.cn


<!-- 参考信息 -->