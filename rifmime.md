代发 wailian999

[A10] 生成随机数
来源：http://vr.panjiajie.cn

Py:   import random; random.randint(1, 100)
来源：http://ef.yuntaijiaju.cn

PHP:  random_int(1, 100);
来源：http://fs.jctech888.com.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://uy.hahajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://sn.asd995.cn

Java: new Random().nextInt(100) + 1
来源：http://wa.521024.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tr.huixinmuqiang.cn

Ruby: rand(1..100)
来源：http://fe.lnxyls.cn

C#:   new Random().Next(1, 101)
来源：http://zr.shxzukj.cn

[A11] 条件表达式（三元）
来源：http://mo.nszjky.cn

Py:   "yes" if x > 0 else "no"
来源：http://ts.szsharing.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://wb.nicolike.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qi.shtwfgs.cn

TS:   x > 0 ? "yes" : "no"
来源：http://uq.huanxung.cn

Java: x > 0 ? "yes" : "no"
来源：http://yc.shxzskj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://et.nszjky.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jv.shtwfgs.cn

C#:   x > 0 ? "yes" : "no"
来源：http://er.haigaiapp.cn

[A12] 字符串插值 / 格式化
来源：http://qc.newstarts.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://yg.panjiajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gr.huixinmuqiang.cn

JS:   `Hello, ${name}!`
来源：http://kx.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://ew.shtwfgs.cn

Java: "Hello, %s!".formatted(name)
来源：http://eb.yuntaijiaju.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mo.chemitech.net.cn

Ruby: "Hello, #{name}!"
来源：http://gf.bjjhwx.cn

C#:   $"Hello, {name}!"
来源：http://tu.szsharing.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://iw.9csxet.cn

Py:   "第一行\n第二行"
来源：http://la.9csxet.cn

PHP:  "第一行\n第二行"
来源：http://lx.9csxet.cn

JS:   "第一行\n第二行"
来源：http://oj.gzmigu.cn

TS:   "第一行\n第二行"
来源：http://vr.bjjhwx.cn

Java: "第一行\n第二行"
来源：http://cp.yuexingan06.cn

Go:   "第一行\n第二行"
来源：http://md.gzmigu.cn

Ruby: "第一行\n第二行"
来源：http://xv.nicolike.cn

C#:   "第一行\n第二行"
来源：http://ff.bookmarksfly.cn

[A14] 注释写法
来源：http://br.shtwfgs.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://co.hnjuh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://nn.hnjuh.cn

JS:   // 单行；/* 多行 */
来源：http://ue.jctech888.com.cn

TS:   // 单行；/* 多行 */
来源：http://nr.shxzskj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ov.newstarts.cn

Go:   // 单行；/* 多行 */
来源：http://hs.haigaiapp.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ke.muxihuayi.cn

C#:   // 单行；/* 多行 */
来源：http://tp.jianghongdianzi.cn

[A15] 空值判断与默认值
来源：http://rr.szsharing.cn

Py:   value = data or "默认值"
来源：http://qn.shxzukj.cn

PHP:  $value = $data ?? "默认值";
来源：http://xp.chemitech.net.cn

JS:   const value = data ?? "默认值";
来源：http://rc.hnjuh.cn

TS:   const value = data ?? "默认值";
来源：http://cv.bookmarksfly.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wf.huanxung.cn

Go:   if data == "" { data = "默认值" }
来源：http://fl.shxzskj.cn

Ruby: value = data || "默认值"
来源：http://ea.chemitech.net.cn

C#:   var value = data ?? "默认值";
来源：http://wy.haigaiapp.cn

[A16] 真假值判断规则
来源：http://so.9csxet.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hm.shxzskj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pa.lnxyls.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hb.hnjuh.cn

TS:   if (!x) {}
来源：http://vn.nicolike.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yt.panjiajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://of.9csxet.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ln.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jm.haigaiapp.cn

[A17] 位运算
来源：http://rx.jianghongdianzi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lw.bookmarksfly.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ar.szxytkj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xd.shtwfgs.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.521024.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hh.yuntaijiaju.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gl.lnxyls.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pn.jctech888.com.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qu.nicolike.cn

[A18] 字符与 ASCII 码互转
来源：http://qo.jianghongdianzi.cn

Py:   ord("A"); chr(65)
来源：http://bu.bjjhwx.cn

PHP:  ord("A"); chr(65)
来源：http://hm.bookmarksfly.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zz.yuntaijiaju.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wh.521024.cn

Java: (int) 'A'; (char) 65
来源：http://nh.shxzukj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gg.shtwfgs.cn

Ruby: "A".ord; 65.chr
来源：http://po.asd995.cn

C#:   (int)'A'; (char)65
来源：http://ua.szsharing.cn

[A19] 交换两个变量
来源：http://ev.hahajie.cn

Py:   a, b = b, a
来源：http://av.panjiajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://cx.nszjky.cn

JS:   [a, b] = [b, a];
来源：http://gv.panjiajie.cn

TS:   [a, b] = [b, a];
来源：http://cm.chemitech.net.cn

Java: int t = a; a = b; b = t;
来源：http://mz.haigaiapp.cn

Go:   a, b = b, a
来源：http://sl.jctech888.com.cn

Ruby: a, b = b, a
来源：http://fj.huixinmuqiang.cn

C#:   (a, b) = (b, a);
来源：http://gr.shxzskj.cn

[A20] 读取标准输入
来源：http://ha.lnxyls.cn

Py:   name = input("请输入：")
来源：http://nx.szsharing.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://oc.gzmigu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xy.colortex.cn

TS:   // Node.js：readline 模块
来源：http://yl.panjiajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://gs.nicolike.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kz.haigaiapp.cn

Ruby: gets.chomp
来源：http://fn.bjjhwx.cn

C#:   Console.ReadLine();
来源：http://wu.muxihuayi.cn

[A21] 保留指定小数位输出
来源：http://in.wgjwhj.cn

Py:   f"{3.14159:.2f}"
来源：http://dl.bjjhwx.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ki.colortex.cn

JS:   (3.14159).toFixed(2)
来源：http://iw.muxihuayi.cn

TS:   (3.14159).toFixed(2)
来源：http://cl.chemitech.net.cn

Java: String.format("%.2f", 3.14159)
来源：http://qe.newstarts.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sl.shxzskj.cn

Ruby: format("%.2f", 3.14159)
来源：http://mx.colortex.cn

C#:   3.14159.ToString("F2")
来源：http://yz.muxihuayi.cn

[A22] 获取字符串长度
来源：http://pc.huanxung.cn

Py:   len(s)
来源：http://kv.panjiajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bq.panjiajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hp.wgjwhj.cn

TS:   s.length
来源：http://ll.huixinmuqiang.cn

Java: s.length()
来源：http://eb.bookmarksfly.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rr.shxzskj.cn

Ruby: s.length
来源：http://tv.huixinmuqiang.cn

C#:   s.Length
来源：http://zh.shxzskj.cn

[A23] 大小写转换
来源：http://io.nszjky.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gc.hahajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nu.hahajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ze.shtwfgs.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ay.nszjky.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yc.hnjuh.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://id.nicolike.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gf.szsharing.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://mi.chemitech.net.cn

[A24] 去除首尾空白
来源：http://fe.yuntaijiaju.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jk.hahajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qy.huixinmuqiang.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bf.shtwfgs.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ih.newstarts.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hn.szsharing.cn

Go:   strings.TrimSpace(s)
来源：http://vq.yuntaijiaju.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xj.wgjwhj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mt.yuntaijiaju.cn

[A25] 字符串比较
来源：http://qp.521024.cn

Py:   s1 == s2; s1 != s2
来源：http://si.muxihuayi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mn.521024.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://it.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ry.gzmigu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://es.huixiangedu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://py.huanxung.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tm.bookmarksfly.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lp.yuntaijiaju.cn

[A26] 类型转换总览
来源：http://dl.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://is.huixiangedu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zs.shxzskj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qd.hahajie.cn

TS:   Number() String() Boolean() x as number
来源：http://ej.shxzukj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bm.newstarts.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nq.nicolike.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kb.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dq.muxihuayi.cn

================================================================================
来源：http://jz.9csxet.cn

B. 流程控制
来源：http://hp.hahajie.cn

================================================================================
来源：http://qn.9csxet.cn

[B01] 条件判断 if / else
来源：http://ou.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ob.jctech888.com.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://aa.huixinmuqiang.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yw.lnxyls.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uo.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://im.jctech888.com.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gk.jianghongdianzi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vb.bjjhwx.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://db.wgjwhj.cn

[B02] 多分支 else if / elif
来源：http://ye.colortex.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://li.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mh.jianghongdianzi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ii.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pc.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eo.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yx.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://du.newstarts.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ve.huixiangedu.cn

[B03] switch / match / case
来源：http://oa.panjiajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yc.yuntaijiaju.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ip.jctech888.com.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://je.newstarts.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uh.shxzskj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ox.hahajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cw.gzmigu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rg.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://my.colortex.cn

[B04] for 计数循环
来源：http://jp.shxzukj.cn

Py:   for i in range(10): print(i)
来源：http://ml.gzmigu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://oc.bjjhwx.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vp.chemitech.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wm.521024.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bf.hahajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fj.nszjky.cn

Ruby: 10.times { |i| puts i }
来源：http://jc.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://et.shxzukj.cn

[B05] 遍历数组 / 列表
来源：http://fd.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://xj.asd995.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nm.chemitech.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kw.bookmarksfly.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sw.jctech888.com.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sz.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pc.asd995.cn

Ruby: arr.each { |item| puts item }
来源：http://ek.jianghongdianzi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://go.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://eh.nszjky.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://en.gzmigu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hm.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tx.jianghongdianzi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bf.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lq.gzmigu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xv.huanxung.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hl.521024.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://de.huixiangedu.cn

[B07] while 循环
来源：http://oe.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://qh.shxzskj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pn.shtwfgs.cn

JS:   while (i < 10) { i++; }
来源：http://jn.shxzskj.cn

TS:   while (i < 10) { i++; }
来源：http://ld.521024.cn

Java: while (i < 10) { i++; }
来源：http://sd.asd995.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pm.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://hm.chemitech.net.cn

C#:   while (i < 10) { i++; }
来源：http://av.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://ns.newstarts.cn

Py:   # 无 do-while：用 while True + break
来源：http://cd.jctech888.com.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kv.wgjwhj.cn

JS:   do { i++; } while (i < 10);
来源：http://gp.jctech888.com.cn

TS:   do { i++; } while (i < 10);
来源：http://ba.gzmigu.cn

Java: do { i++; } while (i < 10);
来源：http://ct.9csxet.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ww.shxzukj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jg.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://jw.521024.cn

[B09] break 与 continue
来源：http://zq.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://oe.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xo.nicolike.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iy.chemitech.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xe.shtwfgs.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sn.bjjhwx.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lu.szxytkj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vb.shtwfgs.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://he.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://kr.bookmarksfly.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tv.lnxyls.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jq.huixinmuqiang.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ga.yuntaijiaju.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wj.wgjwhj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nj.szsharing.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hx.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ap.lnxyls.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kd.yuntaijiaju.cn

[B11] 生成数字序列 / 区间
来源：http://ti.hnjuh.cn

Py:   list(range(0, 10, 2))
来源：http://up.521024.cn

PHP:  range(0, 10, 2);
来源：http://bi.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cl.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hv.huixiangedu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qx.hahajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ma.szsharing.cn

Ruby: (0...10).step(2).to_a
来源：http://jq.huixiangedu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ql.muxihuayi.cn

[B12] 跳出多层循环
来源：http://av.huixinmuqiang.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://on.bookmarksfly.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nv.yuntaijiaju.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xs.panjiajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sv.szsharing.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vs.521024.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gs.muxihuayi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://el.hahajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sx.szsharing.cn

[B13] 判断是否为数字
来源：http://hz.hnjuh.cn

Py:   isinstance(x, (int, float))
来源：http://im.hahajie.cn

PHP:  is_numeric($x)
来源：http://sn.jianghongdianzi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jl.huixinmuqiang.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cj.chemitech.net.cn

Java: x instanceof Number
来源：http://ue.huixinmuqiang.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ot.szxytkj.cn

Ruby: x.is_a?(Numeric)
来源：http://ue.newstarts.cn

C#:   x is int or double or decimal
来源：http://bq.jctech888.com.cn

[B14] 判断值是否在集合内
来源：http://pw.shxzskj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rg.521024.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ud.jctech888.com.cn

JS:   [1, 2, 3].includes(x)
来源：http://jj.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://ur.nszjky.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rz.jianghongdianzi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://or.hahajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gq.bookmarksfly.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ut.muxihuayi.cn

[B15] 布尔运算与取反
来源：http://yu.huanxung.cn

Py:   a and b or not c
来源：http://qe.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://ye.bjjhwx.cn

JS:   a && b || !c
来源：http://ad.521024.cn

TS:   a && b || !c
来源：http://lo.nszjky.cn

Java: a && b || !c
来源：http://zz.huanxung.cn

Go:   a && b || !c
来源：http://ih.9csxet.cn

Ruby: a && b || !c
来源：http://sp.lnxyls.cn

C#:   a && b || !c
来源：http://ag.szsharing.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sl.chemitech.net.cn

Py:   if not data: return
来源：http://id.hnjuh.cn

PHP:  if (!$data) { return; }
来源：http://lg.hahajie.cn

JS:   if (!data) return;
来源：http://wf.lnxyls.cn

TS:   if (!data) return;
来源：http://ky.nicolike.cn

Java: if (data == null) return;
来源：http://oy.shxzukj.cn

Go:   if data == nil { return }
来源：http://ef.nicolike.cn

Ruby: return if data.nil?
来源：http://qq.9csxet.cn

C#:   if (data == null) return;
来源：http://vm.wgjwhj.cn


<!-- 参考信息 -->