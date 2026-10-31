代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://py.szxytkj.cn

Java: new Random().nextInt(100) + 1
来源：http://ob.521024.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zu.shxzukj.cn

Ruby: rand(1..100)
来源：http://cf.yuexingan06.cn

C#:   new Random().Next(1, 101)
来源：http://oj.bjjhwx.cn

[A11] 条件表达式（三元）
来源：http://kl.yuntaijiaju.cn

Py:   "yes" if x > 0 else "no"
来源：http://ip.newstarts.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://uv.szxytkj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://bv.szxytkj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://lh.haigaiapp.cn

Java: x > 0 ? "yes" : "no"
来源：http://rn.huixiangedu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xx.yuntaijiaju.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://gx.shxzukj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://nk.9csxet.cn

[A12] 字符串插值 / 格式化
来源：http://xv.nicolike.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kb.521024.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ic.jianghongdianzi.cn

JS:   `Hello, ${name}!`
来源：http://jw.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://td.jianghongdianzi.cn

Java: "Hello, %s!".formatted(name)
来源：http://jo.asd995.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sf.9csxet.cn

Ruby: "Hello, #{name}!"
来源：http://ib.yuntaijiaju.cn

C#:   $"Hello, {name}!"
来源：http://kl.lnxyls.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://jr.gzmigu.cn

Py:   "第一行\n第二行"
来源：http://am.huixiangedu.cn

PHP:  "第一行\n第二行"
来源：http://lp.muxihuayi.cn

JS:   "第一行\n第二行"
来源：http://wl.shxzukj.cn

TS:   "第一行\n第二行"
来源：http://dn.jianghongdianzi.cn

Java: "第一行\n第二行"
来源：http://nn.newstarts.cn

Go:   "第一行\n第二行"
来源：http://vc.nszjky.cn

Ruby: "第一行\n第二行"
来源：http://bt.asd995.cn

C#:   "第一行\n第二行"
来源：http://ah.haigaiapp.cn

[A14] 注释写法
来源：http://cb.asd995.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://fx.asd995.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ah.hahajie.cn

JS:   // 单行；/* 多行 */
来源：http://wn.huixinmuqiang.cn

TS:   // 单行；/* 多行 */
来源：http://gd.huanxung.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hn.jctech888.com.cn

Go:   // 单行；/* 多行 */
来源：http://ah.bookmarksfly.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vc.gzmigu.cn

C#:   // 单行；/* 多行 */
来源：http://di.huixinmuqiang.cn

[A15] 空值判断与默认值
来源：http://qn.shxzukj.cn

Py:   value = data or "默认值"
来源：http://cx.panjiajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://mn.nicolike.cn

JS:   const value = data ?? "默认值";
来源：http://rm.bjjhwx.cn

TS:   const value = data ?? "默认值";
来源：http://xc.hnjuh.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ov.nicolike.cn

Go:   if data == "" { data = "默认值" }
来源：http://cy.bjjhwx.cn

Ruby: value = data || "默认值"
来源：http://ig.haigaiapp.cn

C#:   var value = data ?? "默认值";
来源：http://et.huixinmuqiang.cn

[A16] 真假值判断规则
来源：http://zu.shxzskj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yc.lnxyls.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wl.jctech888.com.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://za.521024.cn

TS:   if (!x) {}
来源：http://gw.9csxet.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ld.colortex.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ix.bjjhwx.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hl.nicolike.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hu.hnjuh.cn

[A17] 位运算
来源：http://uk.huixiangedu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://su.jianghongdianzi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ad.huixinmuqiang.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qi.szxytkj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://th.hahajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gb.jianghongdianzi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wx.chemitech.net.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://st.huixiangedu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qi.bookmarksfly.cn

[A18] 字符与 ASCII 码互转
来源：http://vb.newstarts.cn

Py:   ord("A"); chr(65)
来源：http://xw.szsharing.cn

PHP:  ord("A"); chr(65)
来源：http://px.shxzukj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xo.chemitech.net.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bg.gzmigu.cn

Java: (int) 'A'; (char) 65
来源：http://pq.jianghongdianzi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vt.newstarts.cn

Ruby: "A".ord; 65.chr
来源：http://ig.huixiangedu.cn

C#:   (int)'A'; (char)65
来源：http://we.gzmigu.cn

[A19] 交换两个变量
来源：http://il.9csxet.cn

Py:   a, b = b, a
来源：http://re.panjiajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ul.nszjky.cn

JS:   [a, b] = [b, a];
来源：http://uq.muxihuayi.cn

TS:   [a, b] = [b, a];
来源：http://jh.muxihuayi.cn

Java: int t = a; a = b; b = t;
来源：http://dk.wgjwhj.cn

Go:   a, b = b, a
来源：http://zi.chemitech.net.cn

Ruby: a, b = b, a
来源：http://sr.hnjuh.cn

C#:   (a, b) = (b, a);
来源：http://pp.haigaiapp.cn

[A20] 读取标准输入
来源：http://ez.shxzskj.cn

Py:   name = input("请输入：")
来源：http://va.jianghongdianzi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://te.nicolike.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://no.newstarts.cn

TS:   // Node.js：readline 模块
来源：http://hc.nicolike.cn

Java: new Scanner(System.in).nextLine()
来源：http://pm.szxytkj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.huixiangedu.cn

Ruby: gets.chomp
来源：http://aa.hnjuh.cn

C#:   Console.ReadLine();
来源：http://pb.yuexingan06.cn

[A21] 保留指定小数位输出
来源：http://nf.nszjky.cn

Py:   f"{3.14159:.2f}"
来源：http://br.huixiangedu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zf.chemitech.net.cn

JS:   (3.14159).toFixed(2)
来源：http://ah.huixinmuqiang.cn

TS:   (3.14159).toFixed(2)
来源：http://wk.huixiangedu.cn

Java: String.format("%.2f", 3.14159)
来源：http://ej.521024.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vi.bjjhwx.cn

Ruby: format("%.2f", 3.14159)
来源：http://dw.szsharing.cn

C#:   3.14159.ToString("F2")
来源：http://jt.yuexingan06.cn

[A22] 获取字符串长度
来源：http://vc.shxzukj.cn

Py:   len(s)
来源：http://bw.jianghongdianzi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ef.panjiajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vz.9csxet.cn

TS:   s.length
来源：http://yx.yuexingan06.cn

Java: s.length()
来源：http://ud.panjiajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yk.jctech888.com.cn

Ruby: s.length
来源：http://vs.huanxung.cn

C#:   s.Length
来源：http://ib.shxzskj.cn

[A23] 大小写转换
来源：http://ls.hahajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://un.chemitech.net.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ky.nicolike.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fe.wgjwhj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://as.hahajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kc.huanxung.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://en.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pc.huanxung.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ho.shxzskj.cn

[A24] 去除首尾空白
来源：http://jr.wgjwhj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fl.panjiajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yr.newstarts.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hd.huixinmuqiang.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vb.shtwfgs.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ij.9csxet.cn

Go:   strings.TrimSpace(s)
来源：http://oy.yuexingan06.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ee.nicolike.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tq.hnjuh.cn

[A25] 字符串比较
来源：http://dy.bjjhwx.cn

Py:   s1 == s2; s1 != s2
来源：http://ts.haigaiapp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ic.jianghongdianzi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ei.gzmigu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dy.9csxet.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sw.newstarts.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vo.muxihuayi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fu.hnjuh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sj.nszjky.cn

[A26] 类型转换总览
来源：http://mc.shxzskj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nw.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cn.huixiangedu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vv.yuntaijiaju.cn

TS:   Number() String() Boolean() x as number
来源：http://ed.huanxung.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cf.nszjky.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mf.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yk.szxytkj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qj.newstarts.cn

================================================================================
来源：http://df.yuntaijiaju.cn

B. 流程控制
来源：http://vq.bjjhwx.cn

================================================================================
来源：http://mk.hahajie.cn

[B01] 条件判断 if / else
来源：http://kn.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://az.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xi.chemitech.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jn.shxzukj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oi.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ha.hahajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ic.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sa.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tz.nicolike.cn

[B02] 多分支 else if / elif
来源：http://ym.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ro.shxzukj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://he.bookmarksfly.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://is.shxzukj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mg.bjjhwx.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mu.nicolike.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rq.hnjuh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mj.panjiajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dm.yuexingan06.cn

[B03] switch / match / case
来源：http://sz.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xi.jianghongdianzi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ax.szxytkj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pp.shxzskj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fy.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rn.nszjky.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fj.huixiangedu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vo.szxytkj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jm.huanxung.cn

[B04] for 计数循环
来源：http://ky.szsharing.cn

Py:   for i in range(10): print(i)
来源：http://uy.asd995.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ib.shxzskj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ux.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xf.shxzskj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://il.huixinmuqiang.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zh.chemitech.net.cn

Ruby: 10.times { |i| puts i }
来源：http://zi.bookmarksfly.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fm.lnxyls.cn

[B05] 遍历数组 / 列表
来源：http://tf.huanxung.cn

Py:   for item in arr: print(item)
来源：http://bn.huixiangedu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wa.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fs.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kf.shxzukj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hp.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://eo.huanxung.cn

Ruby: arr.each { |item| puts item }
来源：http://jx.bookmarksfly.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bk.huanxung.cn

[B06] 遍历字典 / 对象
来源：http://nz.hahajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nl.bookmarksfly.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zg.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ds.bjjhwx.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cp.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dq.shxzskj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eo.wgjwhj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yj.jianghongdianzi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wl.9csxet.cn

[B07] while 循环
来源：http://yj.lnxyls.cn

Py:   while i < 10: i += 1
来源：http://he.huanxung.cn

PHP:  while ($i < 10) { $i++; }
来源：http://se.jctech888.com.cn

JS:   while (i < 10) { i++; }
来源：http://bc.gzmigu.cn

TS:   while (i < 10) { i++; }
来源：http://ds.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://uv.muxihuayi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dt.hahajie.cn

Ruby: while i < 10; i += 1; end
来源：http://qo.newstarts.cn

C#:   while (i < 10) { i++; }
来源：http://fi.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://xy.nszjky.cn

Py:   # 无 do-while：用 while True + break
来源：http://ra.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ae.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://ow.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://es.9csxet.cn

Java: do { i++; } while (i < 10);
来源：http://ry.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://aw.jctech888.com.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fx.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://mo.colortex.cn

[B09] break 与 continue
来源：http://rd.gzmigu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://en.yuexingan06.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nr.yuexingan06.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ep.shxzukj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://il.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yv.lnxyls.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://df.bookmarksfly.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dn.nicolike.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ek.huanxung.cn

[B10] 遍历同时拿索引
来源：http://gp.szsharing.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://al.colortex.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tn.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ew.yuexingan06.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sd.huixiangedu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xj.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gm.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qd.colortex.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bc.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://at.huixiangedu.cn

Py:   list(range(0, 10, 2))
来源：http://sr.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://co.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nm.bookmarksfly.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pe.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uh.haigaiapp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qz.nicolike.cn

Ruby: (0...10).step(2).to_a
来源：http://fk.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qy.colortex.cn

[B12] 跳出多层循环
来源：http://fh.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lv.shxzukj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kz.colortex.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ry.521024.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sb.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ji.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tp.yuntaijiaju.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://co.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://il.wgjwhj.cn

[B13] 判断是否为数字
来源：http://yb.shxzukj.cn

Py:   isinstance(x, (int, float))
来源：http://tl.szxytkj.cn

PHP:  is_numeric($x)
来源：http://wz.colortex.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kx.yuntaijiaju.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ty.panjiajie.cn

Java: x instanceof Number
来源：http://sa.huixiangedu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://da.colortex.cn

Ruby: x.is_a?(Numeric)
来源：http://mh.chemitech.net.cn

C#:   x is int or double or decimal
来源：http://op.hnjuh.cn

[B14] 判断值是否在集合内
来源：http://ei.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sy.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gf.hnjuh.cn

JS:   [1, 2, 3].includes(x)
来源：http://vn.shxzukj.cn

TS:   [1, 2, 3].includes(x)
来源：http://iz.jianghongdianzi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ek.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rl.hahajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vg.panjiajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://eq.haigaiapp.cn

[B15] 布尔运算与取反
来源：http://bf.muxihuayi.cn

Py:   a and b or not c
来源：http://do.szxytkj.cn

PHP:  $a && $b || !$c
来源：http://mp.jianghongdianzi.cn

JS:   a && b || !c
来源：http://jy.newstarts.cn

TS:   a && b || !c
来源：http://qf.shxzukj.cn

Java: a && b || !c
来源：http://hw.shxzukj.cn

Go:   a && b || !c
来源：http://ts.9csxet.cn

Ruby: a && b || !c
来源：http://bf.nicolike.cn

C#:   a && b || !c
来源：http://nx.hnjuh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ou.521024.cn

Py:   if not data: return
来源：http://rv.wgjwhj.cn

PHP:  if (!$data) { return; }
来源：http://qp.lnxyls.cn

JS:   if (!data) return;
来源：http://xd.nicolike.cn

TS:   if (!data) return;
来源：http://nk.jctech888.com.cn

Java: if (data == null) return;
来源：http://rh.shtwfgs.cn

Go:   if data == nil { return }
来源：http://me.lnxyls.cn

Ruby: return if data.nil?
来源：http://pr.gzmigu.cn

C#:   if (data == null) return;
来源：http://xm.huixiangedu.cn

================================================================================
来源：http://ux.shtwfgs.cn

C. 函数与作用域
来源：http://hv.lnxyls.cn

================================================================================
来源：http://vr.hnjuh.cn

[C01] 定义函数
来源：http://xx.szsharing.cn


<!-- 参考信息 -->