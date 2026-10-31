代发 wailian999

[A10] 生成随机数
来源：http://ir.newstarts.cn

Py:   import random; random.randint(1, 100)
来源：http://og.9csxet.cn

PHP:  random_int(1, 100);
来源：http://sg.panjiajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zf.shtwfgs.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://yn.yuexingan06.cn

Java: new Random().nextInt(100) + 1
来源：http://yz.bookmarksfly.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ld.lnxyls.cn

Ruby: rand(1..100)
来源：http://qx.muxihuayi.cn

C#:   new Random().Next(1, 101)
来源：http://xo.nicolike.cn

[A11] 条件表达式（三元）
来源：http://cy.shxzskj.cn

Py:   "yes" if x > 0 else "no"
来源：http://ph.521024.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://wi.hahajie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://uj.jctech888.com.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dc.haigaiapp.cn

Java: x > 0 ? "yes" : "no"
来源：http://wd.asd995.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wj.colortex.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://fe.huixinmuqiang.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ef.shxzukj.cn

[A12] 字符串插值 / 格式化
来源：http://lb.jctech888.com.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://eu.bookmarksfly.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://la.nicolike.cn

JS:   `Hello, ${name}!`
来源：http://yk.yuexingan06.cn

TS:   `Hello, ${name}!`
来源：http://ie.yuntaijiaju.cn

Java: "Hello, %s!".formatted(name)
来源：http://zm.521024.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jw.chemitech.net.cn

Ruby: "Hello, #{name}!"
来源：http://tb.bjjhwx.cn

C#:   $"Hello, {name}!"
来源：http://wh.huanxung.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://vk.muxihuayi.cn

Py:   "第一行\n第二行"
来源：http://ei.bjjhwx.cn

PHP:  "第一行\n第二行"
来源：http://ti.muxihuayi.cn

JS:   "第一行\n第二行"
来源：http://xc.hahajie.cn

TS:   "第一行\n第二行"
来源：http://tr.huixiangedu.cn

Java: "第一行\n第二行"
来源：http://nn.shxzukj.cn

Go:   "第一行\n第二行"
来源：http://sf.jianghongdianzi.cn

Ruby: "第一行\n第二行"
来源：http://wg.shtwfgs.cn

C#:   "第一行\n第二行"
来源：http://ux.yuntaijiaju.cn

[A14] 注释写法
来源：http://ub.yuexingan06.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://tz.gzmigu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://qu.szxytkj.cn

JS:   // 单行；/* 多行 */
来源：http://ne.muxihuayi.cn

TS:   // 单行；/* 多行 */
来源：http://eg.521024.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://sz.huixinmuqiang.cn

Go:   // 单行；/* 多行 */
来源：http://rb.asd995.cn

Ruby: # 单行；=begin 多行 =end
来源：http://rv.haigaiapp.cn

C#:   // 单行；/* 多行 */
来源：http://yx.jianghongdianzi.cn

[A15] 空值判断与默认值
来源：http://te.bookmarksfly.cn

Py:   value = data or "默认值"
来源：http://fi.9csxet.cn

PHP:  $value = $data ?? "默认值";
来源：http://ne.chemitech.net.cn

JS:   const value = data ?? "默认值";
来源：http://og.jianghongdianzi.cn

TS:   const value = data ?? "默认值";
来源：http://mp.huanxung.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://im.szsharing.cn

Go:   if data == "" { data = "默认值" }
来源：http://mx.huanxung.cn

Ruby: value = data || "默认值"
来源：http://lg.chemitech.net.cn

C#:   var value = data ?? "默认值";
来源：http://kt.hahajie.cn

[A16] 真假值判断规则
来源：http://an.lnxyls.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ii.szsharing.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://in.chemitech.net.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://oi.yuntaijiaju.cn

TS:   if (!x) {}
来源：http://ba.asd995.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rb.jianghongdianzi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://na.jianghongdianzi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://um.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://iy.muxihuayi.cn

[A17] 位运算
来源：http://pw.huixiangedu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fz.shxzukj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hx.jianghongdianzi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sn.jianghongdianzi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fy.huanxung.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ia.jianghongdianzi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://na.yuntaijiaju.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kl.yuntaijiaju.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ik.bookmarksfly.cn

[A18] 字符与 ASCII 码互转
来源：http://ht.asd995.cn

Py:   ord("A"); chr(65)
来源：http://xv.szxytkj.cn

PHP:  ord("A"); chr(65)
来源：http://to.nicolike.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cc.panjiajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yr.shxzukj.cn

Java: (int) 'A'; (char) 65
来源：http://fm.9csxet.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yg.bjjhwx.cn

Ruby: "A".ord; 65.chr
来源：http://mn.huixinmuqiang.cn

C#:   (int)'A'; (char)65
来源：http://cq.haigaiapp.cn

[A19] 交换两个变量
来源：http://nw.panjiajie.cn

Py:   a, b = b, a
来源：http://cj.shxzskj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://hx.colortex.cn

JS:   [a, b] = [b, a];
来源：http://sz.huanxung.cn

TS:   [a, b] = [b, a];
来源：http://bk.colortex.cn

Java: int t = a; a = b; b = t;
来源：http://aw.yuntaijiaju.cn

Go:   a, b = b, a
来源：http://ae.yuexingan06.cn

Ruby: a, b = b, a
来源：http://le.asd995.cn

C#:   (a, b) = (b, a);
来源：http://pl.nicolike.cn

[A20] 读取标准输入
来源：http://wm.9csxet.cn

Py:   name = input("请输入：")
来源：http://nh.huixinmuqiang.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gq.gzmigu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kz.yuntaijiaju.cn

TS:   // Node.js：readline 模块
来源：http://uf.wgjwhj.cn

Java: new Scanner(System.in).nextLine()
来源：http://hk.lnxyls.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://es.yuntaijiaju.cn

Ruby: gets.chomp
来源：http://gp.bookmarksfly.cn

C#:   Console.ReadLine();
来源：http://kb.yuntaijiaju.cn

[A21] 保留指定小数位输出
来源：http://ru.szsharing.cn

Py:   f"{3.14159:.2f}"
来源：http://bt.chemitech.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kr.nszjky.cn

JS:   (3.14159).toFixed(2)
来源：http://zg.bjjhwx.cn

TS:   (3.14159).toFixed(2)
来源：http://hm.huixinmuqiang.cn

Java: String.format("%.2f", 3.14159)
来源：http://eu.szxytkj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://eg.nicolike.cn

Ruby: format("%.2f", 3.14159)
来源：http://tz.hahajie.cn

C#:   3.14159.ToString("F2")
来源：http://fc.hahajie.cn

[A22] 获取字符串长度
来源：http://ex.hahajie.cn

Py:   len(s)
来源：http://qq.huanxung.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rr.newstarts.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pu.bjjhwx.cn

TS:   s.length
来源：http://ub.lnxyls.cn

Java: s.length()
来源：http://qg.haigaiapp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dd.bjjhwx.cn

Ruby: s.length
来源：http://ji.shxzskj.cn

C#:   s.Length
来源：http://jb.hahajie.cn

[A23] 大小写转换
来源：http://vw.huanxung.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nm.gzmigu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ql.huixiangedu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://oc.521024.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vs.szsharing.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://we.lnxyls.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qf.asd995.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jj.huixiangedu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://oe.szsharing.cn

[A24] 去除首尾空白
来源：http://ny.shxzskj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xq.haigaiapp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rs.jctech888.com.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qz.huanxung.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nx.nszjky.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://uo.shxzukj.cn

Go:   strings.TrimSpace(s)
来源：http://sw.gzmigu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vc.yuntaijiaju.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://eu.huixiangedu.cn

[A25] 字符串比较
来源：http://wt.newstarts.cn

Py:   s1 == s2; s1 != s2
来源：http://sm.wgjwhj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ap.yuexingan06.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wr.9csxet.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sr.muxihuayi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mc.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ov.shtwfgs.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gu.bjjhwx.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ux.jctech888.com.cn

[A26] 类型转换总览
来源：http://pq.nszjky.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uj.9csxet.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://it.huixiangedu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ic.gzmigu.cn

TS:   Number() String() Boolean() x as number
来源：http://ea.bookmarksfly.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ss.wgjwhj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dp.wgjwhj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://je.szxytkj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qe.bjjhwx.cn

================================================================================
来源：http://kn.lnxyls.cn

B. 流程控制
来源：http://rx.panjiajie.cn

================================================================================
来源：http://xq.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://uf.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://sf.huixiangedu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ly.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pr.nicolike.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ad.huixiangedu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ax.jctech888.com.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://io.jctech888.com.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ei.wgjwhj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jv.nicolike.cn

[B02] 多分支 else if / elif
来源：http://kk.lnxyls.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tg.hnjuh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wf.bookmarksfly.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nv.hahajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oh.nicolike.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dw.bookmarksfly.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://am.shtwfgs.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://io.lnxyls.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qn.yuntaijiaju.cn

[B03] switch / match / case
来源：http://wu.lnxyls.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ov.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ww.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bd.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bh.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mf.huixiangedu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://da.huixinmuqiang.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zq.huixinmuqiang.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rp.szxytkj.cn

[B04] for 计数循环
来源：http://ku.muxihuayi.cn

Py:   for i in range(10): print(i)
来源：http://vz.bookmarksfly.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ei.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sn.szsharing.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fg.szsharing.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sp.yuntaijiaju.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ik.nszjky.cn

Ruby: 10.times { |i| puts i }
来源：http://ku.szxytkj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pv.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://fs.newstarts.cn

Py:   for item in arr: print(item)
来源：http://fd.yuntaijiaju.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jf.asd995.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://cn.hnjuh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wz.colortex.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xt.wgjwhj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://uo.nszjky.cn

Ruby: arr.each { |item| puts item }
来源：http://sh.bookmarksfly.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ns.huixinmuqiang.cn

[B06] 遍历字典 / 对象
来源：http://rs.9csxet.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ha.shtwfgs.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hm.bookmarksfly.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cv.shxzukj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zs.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ix.lnxyls.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ni.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xb.chemitech.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yw.521024.cn

[B07] while 循环
来源：http://wp.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://ld.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zp.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://qb.colortex.cn

TS:   while (i < 10) { i++; }
来源：http://rd.asd995.cn

Java: while (i < 10) { i++; }
来源：http://se.bjjhwx.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fz.szsharing.cn

Ruby: while i < 10; i += 1; end
来源：http://yz.newstarts.cn

C#:   while (i < 10) { i++; }
来源：http://zi.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://ok.panjiajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://ax.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://as.yuexingan06.cn

JS:   do { i++; } while (i < 10);
来源：http://sb.shtwfgs.cn

TS:   do { i++; } while (i < 10);
来源：http://fc.9csxet.cn

Java: do { i++; } while (i < 10);
来源：http://zp.panjiajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ot.521024.cn

Ruby: begin; i += 1; end while i < 10
来源：http://sl.szsharing.cn

C#:   do { i++; } while (i < 10);
来源：http://nv.szxytkj.cn

[B09] break 与 continue
来源：http://en.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ui.shxzskj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xr.521024.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ma.jctech888.com.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nu.huanxung.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fv.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dq.newstarts.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ly.yuexingan06.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ns.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://wh.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ul.yuntaijiaju.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://iq.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lz.yuntaijiaju.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cg.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://by.huixinmuqiang.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zc.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://oh.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yd.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://jp.szxytkj.cn

Py:   list(range(0, 10, 2))
来源：http://qo.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://we.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yc.colortex.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vu.huixiangedu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zh.jctech888.com.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oe.muxihuayi.cn

Ruby: (0...10).step(2).to_a
来源：http://qe.huanxung.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ki.jctech888.com.cn

[B12] 跳出多层循环
来源：http://jg.jianghongdianzi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ea.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ey.chemitech.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wv.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mj.huixinmuqiang.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ro.gzmigu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hk.gzmigu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tk.szsharing.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zw.huixiangedu.cn

[B13] 判断是否为数字
来源：http://uz.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://dw.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://xv.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://py.nszjky.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eu.jianghongdianzi.cn

Java: x instanceof Number
来源：http://ca.nszjky.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ro.lnxyls.cn

Ruby: x.is_a?(Numeric)
来源：http://dy.asd995.cn

C#:   x is int or double or decimal
来源：http://sx.haigaiapp.cn

[B14] 判断值是否在集合内
来源：http://me.bjjhwx.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yv.gzmigu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ml.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://ek.jianghongdianzi.cn

TS:   [1, 2, 3].includes(x)
来源：http://lc.nszjky.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jj.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rq.jctech888.com.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fr.asd995.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hb.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://cq.chemitech.net.cn

Py:   a and b or not c
来源：http://kw.asd995.cn

PHP:  $a && $b || !$c
来源：http://ld.bjjhwx.cn

JS:   a && b || !c
来源：http://rl.bookmarksfly.cn

TS:   a && b || !c
来源：http://bn.chemitech.net.cn

Java: a && b || !c
来源：http://xm.hahajie.cn

Go:   a && b || !c
来源：http://vh.szxytkj.cn

Ruby: a && b || !c
来源：http://sf.shxzukj.cn

C#:   a && b || !c
来源：http://ib.bookmarksfly.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xk.newstarts.cn

Py:   if not data: return
来源：http://na.huixinmuqiang.cn

PHP:  if (!$data) { return; }
来源：http://cm.huixinmuqiang.cn

JS:   if (!data) return;
来源：http://ee.muxihuayi.cn

TS:   if (!data) return;
来源：http://ly.bookmarksfly.cn

Java: if (data == null) return;
来源：http://hj.shxzukj.cn

Go:   if data == nil { return }
来源：http://yw.yuntaijiaju.cn

Ruby: return if data.nil?
来源：http://bz.yuntaijiaju.cn

C#:   if (data == null) return;
来源：http://vx.haigaiapp.cn


<!-- 参考信息 -->