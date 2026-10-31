代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bz.huixiangedu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qo.panjiajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ll.9csxet.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kl.panjiajie.cn

[A10] 生成随机数
来源：http://oi.shxzskj.cn

Py:   import random; random.randint(1, 100)
来源：http://zi.nicolike.cn

PHP:  random_int(1, 100);
来源：http://ja.gzmigu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ll.muxihuayi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ap.shxzukj.cn

Java: new Random().nextInt(100) + 1
来源：http://fd.jianghongdianzi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xo.shxzskj.cn

Ruby: rand(1..100)
来源：http://mo.9csxet.cn

C#:   new Random().Next(1, 101)
来源：http://qz.9csxet.cn

[A11] 条件表达式（三元）
来源：http://ju.asd995.cn

Py:   "yes" if x > 0 else "no"
来源：http://ya.nszjky.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://mb.bookmarksfly.cn

JS:   x > 0 ? "yes" : "no"
来源：http://kg.hnjuh.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ad.nicolike.cn

Java: x > 0 ? "yes" : "no"
来源：http://yv.521024.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://li.yuexingan06.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://nr.lnxyls.cn

C#:   x > 0 ? "yes" : "no"
来源：http://hy.haigaiapp.cn

[A12] 字符串插值 / 格式化
来源：http://zv.hnjuh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wk.haigaiapp.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qt.muxihuayi.cn

JS:   `Hello, ${name}!`
来源：http://li.nicolike.cn

TS:   `Hello, ${name}!`
来源：http://sp.colortex.cn

Java: "Hello, %s!".formatted(name)
来源：http://hi.huanxung.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ix.szxytkj.cn

Ruby: "Hello, #{name}!"
来源：http://vo.asd995.cn

C#:   $"Hello, {name}!"
来源：http://mi.bookmarksfly.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://le.lnxyls.cn

Py:   "第一行\n第二行"
来源：http://ly.panjiajie.cn

PHP:  "第一行\n第二行"
来源：http://tk.nicolike.cn

JS:   "第一行\n第二行"
来源：http://id.521024.cn

TS:   "第一行\n第二行"
来源：http://nn.jianghongdianzi.cn

Java: "第一行\n第二行"
来源：http://lq.jctech888.com.cn

Go:   "第一行\n第二行"
来源：http://jm.chemitech.net.cn

Ruby: "第一行\n第二行"
来源：http://fl.lnxyls.cn

C#:   "第一行\n第二行"
来源：http://ud.szxytkj.cn

[A14] 注释写法
来源：http://fs.shtwfgs.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://su.huixiangedu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ko.chemitech.net.cn

JS:   // 单行；/* 多行 */
来源：http://ns.asd995.cn

TS:   // 单行；/* 多行 */
来源：http://ne.asd995.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yg.jianghongdianzi.cn

Go:   // 单行；/* 多行 */
来源：http://pw.bookmarksfly.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vg.jctech888.com.cn

C#:   // 单行；/* 多行 */
来源：http://yi.nszjky.cn

[A15] 空值判断与默认值
来源：http://cm.jianghongdianzi.cn

Py:   value = data or "默认值"
来源：http://hf.asd995.cn

PHP:  $value = $data ?? "默认值";
来源：http://ej.shtwfgs.cn

JS:   const value = data ?? "默认值";
来源：http://sr.shtwfgs.cn

TS:   const value = data ?? "默认值";
来源：http://mb.newstarts.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kc.shxzskj.cn

Go:   if data == "" { data = "默认值" }
来源：http://dj.muxihuayi.cn

Ruby: value = data || "默认值"
来源：http://ma.asd995.cn

C#:   var value = data ?? "默认值";
来源：http://ty.colortex.cn

[A16] 真假值判断规则
来源：http://rt.jianghongdianzi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vc.jianghongdianzi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nv.bjjhwx.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rj.nicolike.cn

TS:   if (!x) {}
来源：http://pe.szsharing.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jq.bjjhwx.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ti.521024.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lk.9csxet.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sk.jianghongdianzi.cn

[A17] 位运算
来源：http://mm.nszjky.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qe.hnjuh.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tv.hahajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bu.szsharing.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lj.colortex.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kk.gzmigu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ac.szxytkj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gl.yuexingan06.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vv.hahajie.cn

[A18] 字符与 ASCII 码互转
来源：http://so.jctech888.com.cn

Py:   ord("A"); chr(65)
来源：http://ls.yuexingan06.cn

PHP:  ord("A"); chr(65)
来源：http://md.huixiangedu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ou.colortex.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wb.jianghongdianzi.cn

Java: (int) 'A'; (char) 65
来源：http://pp.szxytkj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ks.colortex.cn

Ruby: "A".ord; 65.chr
来源：http://nc.huanxung.cn

C#:   (int)'A'; (char)65
来源：http://kp.nicolike.cn

[A19] 交换两个变量
来源：http://xx.bjjhwx.cn

Py:   a, b = b, a
来源：http://hz.huixiangedu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://sj.chemitech.net.cn

JS:   [a, b] = [b, a];
来源：http://tr.521024.cn

TS:   [a, b] = [b, a];
来源：http://co.bookmarksfly.cn

Java: int t = a; a = b; b = t;
来源：http://vu.huixinmuqiang.cn

Go:   a, b = b, a
来源：http://vj.yuntaijiaju.cn

Ruby: a, b = b, a
来源：http://an.szsharing.cn

C#:   (a, b) = (b, a);
来源：http://px.haigaiapp.cn

[A20] 读取标准输入
来源：http://gj.nicolike.cn

Py:   name = input("请输入：")
来源：http://xa.huixinmuqiang.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://hy.521024.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hy.huixinmuqiang.cn

TS:   // Node.js：readline 模块
来源：http://gz.szsharing.cn

Java: new Scanner(System.in).nextLine()
来源：http://kx.nicolike.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ow.shxzskj.cn

Ruby: gets.chomp
来源：http://ul.yuntaijiaju.cn

C#:   Console.ReadLine();
来源：http://kd.colortex.cn

[A21] 保留指定小数位输出
来源：http://nh.szsharing.cn

Py:   f"{3.14159:.2f}"
来源：http://rx.jctech888.com.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yo.panjiajie.cn

JS:   (3.14159).toFixed(2)
来源：http://ve.panjiajie.cn

TS:   (3.14159).toFixed(2)
来源：http://uw.huixinmuqiang.cn

Java: String.format("%.2f", 3.14159)
来源：http://be.colortex.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.nszjky.cn

Ruby: format("%.2f", 3.14159)
来源：http://qc.shxzukj.cn

C#:   3.14159.ToString("F2")
来源：http://ma.huixiangedu.cn

[A22] 获取字符串长度
来源：http://cn.haigaiapp.cn

Py:   len(s)
来源：http://is.szxytkj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wu.yuexingan06.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hm.huixinmuqiang.cn

TS:   s.length
来源：http://br.panjiajie.cn

Java: s.length()
来源：http://ri.szxytkj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://og.shtwfgs.cn

Ruby: s.length
来源：http://bv.bookmarksfly.cn

C#:   s.Length
来源：http://td.shtwfgs.cn

[A23] 大小写转换
来源：http://ff.muxihuayi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ky.shxzukj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://it.haigaiapp.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ph.9csxet.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://iw.shxzukj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ns.shtwfgs.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ct.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dy.yuntaijiaju.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xw.yuntaijiaju.cn

[A24] 去除首尾空白
来源：http://ls.hnjuh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qu.9csxet.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nx.nicolike.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tn.hahajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zv.muxihuayi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kx.wgjwhj.cn

Go:   strings.TrimSpace(s)
来源：http://zi.yuntaijiaju.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jx.huixinmuqiang.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ec.asd995.cn

[A25] 字符串比较
来源：http://ol.szsharing.cn

Py:   s1 == s2; s1 != s2
来源：http://mw.yuntaijiaju.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vn.chemitech.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nv.asd995.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kt.newstarts.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ya.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jr.asd995.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ph.huanxung.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://oh.nszjky.cn

[A26] 类型转换总览
来源：http://ad.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qp.nszjky.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gl.jianghongdianzi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nb.jctech888.com.cn

TS:   Number() String() Boolean() x as number
来源：http://vp.521024.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tg.colortex.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qu.yuexingan06.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lp.hahajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zq.shtwfgs.cn

================================================================================
来源：http://hs.jianghongdianzi.cn

B. 流程控制
来源：http://ia.szsharing.cn

================================================================================
来源：http://yu.huanxung.cn

[B01] 条件判断 if / else
来源：http://rt.colortex.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qt.asd995.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://eg.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wr.gzmigu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sb.huanxung.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wf.panjiajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://oz.521024.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uq.gzmigu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zk.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://ow.yuexingan06.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lu.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://np.haigaiapp.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jd.nszjky.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ky.521024.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nd.chemitech.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bb.szsharing.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gi.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qx.shtwfgs.cn

[B03] switch / match / case
来源：http://dx.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wq.shxzskj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://um.muxihuayi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ll.lnxyls.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lq.yuntaijiaju.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sb.bjjhwx.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dm.huixiangedu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tn.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ji.jctech888.com.cn

[B04] for 计数循环
来源：http://kv.bookmarksfly.cn

Py:   for i in range(10): print(i)
来源：http://yn.huanxung.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yv.chemitech.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iy.szsharing.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bs.gzmigu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://et.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ef.colortex.cn

Ruby: 10.times { |i| puts i }
来源：http://pf.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yv.huixiangedu.cn

[B05] 遍历数组 / 列表
来源：http://jy.muxihuayi.cn

Py:   for item in arr: print(item)
来源：http://yr.bookmarksfly.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gx.lnxyls.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gy.jianghongdianzi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fz.gzmigu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mu.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cb.huanxung.cn

Ruby: arr.each { |item| puts item }
来源：http://fx.szxytkj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ri.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://nv.yuntaijiaju.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ar.shtwfgs.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qq.huanxung.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vo.shxzukj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tw.newstarts.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fd.521024.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zz.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tk.huanxung.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vd.hahajie.cn

[B07] while 循环
来源：http://ho.newstarts.cn

Py:   while i < 10: i += 1
来源：http://no.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ga.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://up.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://om.521024.cn

Java: while (i < 10) { i++; }
来源：http://tp.szsharing.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gl.muxihuayi.cn

Ruby: while i < 10; i += 1; end
来源：http://rq.huixiangedu.cn

C#:   while (i < 10) { i++; }
来源：http://we.shxzskj.cn

[B08] do-while（至少执行一次）
来源：http://du.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://bk.jianghongdianzi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gx.yuntaijiaju.cn

JS:   do { i++; } while (i < 10);
来源：http://yb.nicolike.cn

TS:   do { i++; } while (i < 10);
来源：http://uy.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://wd.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wh.nicolike.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cg.521024.cn

C#:   do { i++; } while (i < 10);
来源：http://ct.colortex.cn

[B09] break 与 continue
来源：http://wx.521024.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://he.bjjhwx.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nv.shxzskj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ts.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wc.huixiangedu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mw.nszjky.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nz.nicolike.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gn.huixiangedu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wq.jctech888.com.cn

[B10] 遍历同时拿索引
来源：http://wu.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ks.nicolike.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vu.lnxyls.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://em.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hp.hahajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wb.colortex.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nx.yuexingan06.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qn.shxzukj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mj.jctech888.com.cn

[B11] 生成数字序列 / 区间
来源：http://al.asd995.cn

Py:   list(range(0, 10, 2))
来源：http://ir.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://cq.newstarts.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://au.muxihuayi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tq.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rv.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dd.huixiangedu.cn

Ruby: (0...10).step(2).to_a
来源：http://rm.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://of.yuexingan06.cn

[B12] 跳出多层循环
来源：http://rp.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fx.bookmarksfly.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sk.gzmigu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ea.yuntaijiaju.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xr.asd995.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nj.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oq.shtwfgs.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jw.yuntaijiaju.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cy.shxzukj.cn

[B13] 判断是否为数字
来源：http://gw.hahajie.cn

Py:   isinstance(x, (int, float))
来源：http://vc.gzmigu.cn

PHP:  is_numeric($x)
来源：http://aq.nicolike.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xq.huixiangedu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rh.haigaiapp.cn

Java: x instanceof Number
来源：http://ol.chemitech.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pt.shxzukj.cn

Ruby: x.is_a?(Numeric)
来源：http://ai.nicolike.cn

C#:   x is int or double or decimal
来源：http://jw.chemitech.net.cn

[B14] 判断值是否在集合内
来源：http://on.panjiajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qe.jctech888.com.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lk.521024.cn

JS:   [1, 2, 3].includes(x)
来源：http://si.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://ug.shxzskj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vg.nicolike.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qk.jianghongdianzi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hr.bookmarksfly.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pk.hahajie.cn

[B15] 布尔运算与取反
来源：http://ob.huanxung.cn

Py:   a and b or not c
来源：http://uo.gzmigu.cn

PHP:  $a && $b || !$c
来源：http://ko.colortex.cn

JS:   a && b || !c
来源：http://ub.wgjwhj.cn

TS:   a && b || !c
来源：http://ht.nicolike.cn

Java: a && b || !c
来源：http://kd.muxihuayi.cn

Go:   a && b || !c
来源：http://hf.nicolike.cn

Ruby: a && b || !c
来源：http://mb.huixiangedu.cn

C#:   a && b || !c
来源：http://fc.colortex.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qc.colortex.cn

Py:   if not data: return
来源：http://jo.haigaiapp.cn

PHP:  if (!$data) { return; }
来源：http://kc.bjjhwx.cn

JS:   if (!data) return;
来源：http://hp.bjjhwx.cn

TS:   if (!data) return;
来源：http://rn.lnxyls.cn


<!-- 参考信息 -->