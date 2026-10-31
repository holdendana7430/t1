代发 wailian999

[A10] 生成随机数
来源：http://ns.haigaiapp.cn

Py:   import random; random.randint(1, 100)
来源：http://lg.nicolike.cn

PHP:  random_int(1, 100);
来源：http://ii.huanxung.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jx.yuntaijiaju.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wv.newstarts.cn

Java: new Random().nextInt(100) + 1
来源：http://vw.hahajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jw.521024.cn

Ruby: rand(1..100)
来源：http://ro.shxzukj.cn

C#:   new Random().Next(1, 101)
来源：http://zd.wgjwhj.cn

[A11] 条件表达式（三元）
来源：http://dj.haigaiapp.cn

Py:   "yes" if x > 0 else "no"
来源：http://gc.nszjky.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ca.asd995.cn

JS:   x > 0 ? "yes" : "no"
来源：http://jd.521024.cn

TS:   x > 0 ? "yes" : "no"
来源：http://pz.hahajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://je.521024.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://no.colortex.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vn.huixiangedu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://sy.shxzskj.cn

[A12] 字符串插值 / 格式化
来源：http://wh.shtwfgs.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://st.hahajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cd.shtwfgs.cn

JS:   `Hello, ${name}!`
来源：http://ao.asd995.cn

TS:   `Hello, ${name}!`
来源：http://nx.gzmigu.cn

Java: "Hello, %s!".formatted(name)
来源：http://ez.yuexingan06.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yr.muxihuayi.cn

Ruby: "Hello, #{name}!"
来源：http://kk.muxihuayi.cn

C#:   $"Hello, {name}!"
来源：http://ea.jctech888.com.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://sf.bookmarksfly.cn

Py:   "第一行\n第二行"
来源：http://gc.yuntaijiaju.cn

PHP:  "第一行\n第二行"
来源：http://bm.hahajie.cn

JS:   "第一行\n第二行"
来源：http://rb.szsharing.cn

TS:   "第一行\n第二行"
来源：http://re.hnjuh.cn

Java: "第一行\n第二行"
来源：http://hr.newstarts.cn

Go:   "第一行\n第二行"
来源：http://xu.yuexingan06.cn

Ruby: "第一行\n第二行"
来源：http://rg.newstarts.cn

C#:   "第一行\n第二行"
来源：http://bq.yuexingan06.cn

[A14] 注释写法
来源：http://ov.jctech888.com.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://va.huanxung.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ob.gzmigu.cn

JS:   // 单行；/* 多行 */
来源：http://qy.nicolike.cn

TS:   // 单行；/* 多行 */
来源：http://ut.shxzukj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://uw.wgjwhj.cn

Go:   // 单行；/* 多行 */
来源：http://df.wgjwhj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://dz.bookmarksfly.cn

C#:   // 单行；/* 多行 */
来源：http://wy.shtwfgs.cn

[A15] 空值判断与默认值
来源：http://bq.hahajie.cn

Py:   value = data or "默认值"
来源：http://pk.nicolike.cn

PHP:  $value = $data ?? "默认值";
来源：http://bt.shxzskj.cn

JS:   const value = data ?? "默认值";
来源：http://tv.wgjwhj.cn

TS:   const value = data ?? "默认值";
来源：http://ff.szxytkj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://de.hnjuh.cn

Go:   if data == "" { data = "默认值" }
来源：http://kg.gzmigu.cn

Ruby: value = data || "默认值"
来源：http://ku.muxihuayi.cn

C#:   var value = data ?? "默认值";
来源：http://sf.szsharing.cn

[A16] 真假值判断规则
来源：http://aw.wgjwhj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lz.yuexingan06.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gt.bookmarksfly.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://aj.nszjky.cn

TS:   if (!x) {}
来源：http://ea.newstarts.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zi.asd995.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pg.lnxyls.cn

Ruby: unless x            # nil 与 false 为假
来源：http://fz.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ta.nszjky.cn

[A17] 位运算
来源：http://mj.asd995.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hr.yuexingan06.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fs.panjiajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ae.nszjky.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gz.huixiangedu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://du.shxzukj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xm.lnxyls.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xq.huanxung.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yj.nicolike.cn

[A18] 字符与 ASCII 码互转
来源：http://ps.gzmigu.cn

Py:   ord("A"); chr(65)
来源：http://bb.shxzskj.cn

PHP:  ord("A"); chr(65)
来源：http://sc.shtwfgs.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jj.nicolike.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gh.jctech888.com.cn

Java: (int) 'A'; (char) 65
来源：http://ku.hahajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://iv.yuexingan06.cn

Ruby: "A".ord; 65.chr
来源：http://ms.huixiangedu.cn

C#:   (int)'A'; (char)65
来源：http://tc.jianghongdianzi.cn

[A19] 交换两个变量
来源：http://ny.szsharing.cn

Py:   a, b = b, a
来源：http://vy.hahajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://dg.newstarts.cn

JS:   [a, b] = [b, a];
来源：http://sk.huanxung.cn

TS:   [a, b] = [b, a];
来源：http://bk.colortex.cn

Java: int t = a; a = b; b = t;
来源：http://ya.newstarts.cn

Go:   a, b = b, a
来源：http://js.nicolike.cn

Ruby: a, b = b, a
来源：http://ct.gzmigu.cn

C#:   (a, b) = (b, a);
来源：http://pt.huixinmuqiang.cn

[A20] 读取标准输入
来源：http://vf.521024.cn

Py:   name = input("请输入：")
来源：http://ee.huanxung.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://yc.colortex.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ie.colortex.cn

TS:   // Node.js：readline 模块
来源：http://iv.hnjuh.cn

Java: new Scanner(System.in).nextLine()
来源：http://vf.jianghongdianzi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nu.lnxyls.cn

Ruby: gets.chomp
来源：http://ls.szsharing.cn

C#:   Console.ReadLine();
来源：http://sk.shxzskj.cn

[A21] 保留指定小数位输出
来源：http://hh.wgjwhj.cn

Py:   f"{3.14159:.2f}"
来源：http://lg.bjjhwx.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pv.shtwfgs.cn

JS:   (3.14159).toFixed(2)
来源：http://xz.panjiajie.cn

TS:   (3.14159).toFixed(2)
来源：http://sw.wgjwhj.cn

Java: String.format("%.2f", 3.14159)
来源：http://fv.lnxyls.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://me.yuntaijiaju.cn

Ruby: format("%.2f", 3.14159)
来源：http://sy.huixinmuqiang.cn

C#:   3.14159.ToString("F2")
来源：http://jo.hnjuh.cn

[A22] 获取字符串长度
来源：http://ya.muxihuayi.cn

Py:   len(s)
来源：http://aw.muxihuayi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zx.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bg.shxzskj.cn

TS:   s.length
来源：http://jo.hahajie.cn

Java: s.length()
来源：http://iz.huanxung.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ev.huanxung.cn

Ruby: s.length
来源：http://fb.huixiangedu.cn

C#:   s.Length
来源：http://xv.nicolike.cn

[A23] 大小写转换
来源：http://gu.jctech888.com.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nu.newstarts.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vs.hahajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ng.szxytkj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ym.muxihuayi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ao.9csxet.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jj.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vq.shtwfgs.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lo.yuntaijiaju.cn

[A24] 去除首尾空白
来源：http://kp.huixinmuqiang.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gr.huixinmuqiang.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://oo.wgjwhj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nq.nicolike.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://in.huixinmuqiang.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qh.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://zz.gzmigu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wl.jianghongdianzi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sm.szxytkj.cn

[A25] 字符串比较
来源：http://lf.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://ye.huixiangedu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://js.shtwfgs.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ns.yuexingan06.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rj.yuexingan06.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wa.yuexingan06.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jw.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://sy.panjiajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nh.huanxung.cn

[A26] 类型转换总览
来源：http://mj.yuexingan06.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zn.521024.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qn.bookmarksfly.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uy.nszjky.cn

TS:   Number() String() Boolean() x as number
来源：http://we.lnxyls.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wj.szxytkj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ba.9csxet.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ce.yuntaijiaju.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ly.yuntaijiaju.cn

================================================================================
来源：http://hn.nszjky.cn

B. 流程控制
来源：http://bj.gzmigu.cn

================================================================================
来源：http://za.colortex.cn

[B01] 条件判断 if / else
来源：http://he.shxzukj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vs.haigaiapp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gd.muxihuayi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qy.gzmigu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ot.wgjwhj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vm.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hj.colortex.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cg.szxytkj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://en.lnxyls.cn

[B02] 多分支 else if / elif
来源：http://yk.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mq.nicolike.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nh.colortex.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kc.szxytkj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://st.bjjhwx.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ut.9csxet.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wn.bjjhwx.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vt.yuntaijiaju.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jt.lnxyls.cn

[B03] switch / match / case
来源：http://qv.colortex.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zf.panjiajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zw.yuntaijiaju.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ka.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://am.yuntaijiaju.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://om.jctech888.com.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nc.newstarts.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pt.shtwfgs.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fh.nszjky.cn

[B04] for 计数循环
来源：http://zu.nszjky.cn

Py:   for i in range(10): print(i)
来源：http://yw.huixinmuqiang.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kq.shxzskj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://it.newstarts.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ir.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://go.haigaiapp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gq.huixiangedu.cn

Ruby: 10.times { |i| puts i }
来源：http://iu.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lg.shxzukj.cn

[B05] 遍历数组 / 列表
来源：http://hj.huanxung.cn

Py:   for item in arr: print(item)
来源：http://sv.wgjwhj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qx.szxytkj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yf.colortex.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ji.shxzukj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vc.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ji.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://uc.jianghongdianzi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fy.yuntaijiaju.cn

[B06] 遍历字典 / 对象
来源：http://et.wgjwhj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vj.shxzukj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://an.jianghongdianzi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://km.huixinmuqiang.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bd.muxihuayi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dn.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eg.yuntaijiaju.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ci.shxzukj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yf.bookmarksfly.cn

[B07] while 循环
来源：http://sm.muxihuayi.cn

Py:   while i < 10: i += 1
来源：http://ue.hahajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://er.haigaiapp.cn

JS:   while (i < 10) { i++; }
来源：http://yl.shxzukj.cn

TS:   while (i < 10) { i++; }
来源：http://uz.wgjwhj.cn

Java: while (i < 10) { i++; }
来源：http://xo.yuntaijiaju.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mw.wgjwhj.cn

Ruby: while i < 10; i += 1; end
来源：http://lt.yuexingan06.cn

C#:   while (i < 10) { i++; }
来源：http://go.huanxung.cn

[B08] do-while（至少执行一次）
来源：http://lw.nicolike.cn

Py:   # 无 do-while：用 while True + break
来源：http://fr.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pz.hnjuh.cn

JS:   do { i++; } while (i < 10);
来源：http://gy.huixiangedu.cn

TS:   do { i++; } while (i < 10);
来源：http://tk.wgjwhj.cn

Java: do { i++; } while (i < 10);
来源：http://jy.colortex.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xs.szsharing.cn

Ruby: begin; i += 1; end while i < 10
来源：http://to.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://gv.yuexingan06.cn

[B09] break 与 continue
来源：http://qk.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://is.haigaiapp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ot.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vm.9csxet.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cg.yuexingan06.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wi.hahajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ww.nicolike.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ay.bjjhwx.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qh.nicolike.cn

[B10] 遍历同时拿索引
来源：http://ue.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wb.bookmarksfly.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://aa.jctech888.com.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pn.wgjwhj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uh.huixinmuqiang.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ms.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xa.bookmarksfly.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yn.szxytkj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pc.nszjky.cn

[B11] 生成数字序列 / 区间
来源：http://cs.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://ad.nszjky.cn

PHP:  range(0, 10, 2);
来源：http://ju.szxytkj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dh.lnxyls.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nx.521024.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xy.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dr.gzmigu.cn

Ruby: (0...10).step(2).to_a
来源：http://os.panjiajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lg.asd995.cn

[B12] 跳出多层循环
来源：http://ef.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wu.huixinmuqiang.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://su.lnxyls.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fb.newstarts.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jy.jctech888.com.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://oh.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tz.jianghongdianzi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ug.hahajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mj.9csxet.cn

[B13] 判断是否为数字
来源：http://rl.bookmarksfly.cn

Py:   isinstance(x, (int, float))
来源：http://hb.lnxyls.cn

PHP:  is_numeric($x)
来源：http://td.szsharing.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cf.gzmigu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dg.yuexingan06.cn

Java: x instanceof Number
来源：http://mt.shtwfgs.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zu.shxzskj.cn

Ruby: x.is_a?(Numeric)
来源：http://er.gzmigu.cn

C#:   x is int or double or decimal
来源：http://hk.szsharing.cn

[B14] 判断值是否在集合内
来源：http://si.gzmigu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zb.nicolike.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://de.hahajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://os.szxytkj.cn

TS:   [1, 2, 3].includes(x)
来源：http://pr.chemitech.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yd.shxzukj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yi.asd995.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dv.huanxung.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rn.hnjuh.cn

[B15] 布尔运算与取反
来源：http://au.hahajie.cn

Py:   a and b or not c
来源：http://wx.szsharing.cn

PHP:  $a && $b || !$c
来源：http://yp.colortex.cn

JS:   a && b || !c
来源：http://xo.lnxyls.cn

TS:   a && b || !c
来源：http://az.jctech888.com.cn

Java: a && b || !c
来源：http://ii.asd995.cn

Go:   a && b || !c
来源：http://fc.haigaiapp.cn

Ruby: a && b || !c
来源：http://oe.jctech888.com.cn

C#:   a && b || !c
来源：http://ok.muxihuayi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://og.muxihuayi.cn

Py:   if not data: return
来源：http://kp.panjiajie.cn

PHP:  if (!$data) { return; }
来源：http://je.asd995.cn

JS:   if (!data) return;
来源：http://vn.chemitech.net.cn

TS:   if (!data) return;
来源：http://in.colortex.cn

Java: if (data == null) return;
来源：http://au.muxihuayi.cn

Go:   if data == nil { return }
来源：http://zw.szxytkj.cn

Ruby: return if data.nil?
来源：http://bs.asd995.cn

C#:   if (data == null) return;
来源：http://go.shtwfgs.cn


<!-- 参考信息 -->