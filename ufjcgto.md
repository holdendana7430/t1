代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://jt.bjjhwx.cn

C#:   x > 0 ? "yes" : "no"
来源：http://jo.jctech888.com.cn

[A12] 字符串插值 / 格式化
来源：http://dd.nszjky.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://oa.shxzukj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pg.panjiajie.cn

JS:   `Hello, ${name}!`
来源：http://uk.colortex.cn

TS:   `Hello, ${name}!`
来源：http://dm.gzmigu.cn

Java: "Hello, %s!".formatted(name)
来源：http://na.jctech888.com.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://lm.chemitech.net.cn

Ruby: "Hello, #{name}!"
来源：http://gq.lnxyls.cn

C#:   $"Hello, {name}!"
来源：http://wb.jianghongdianzi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://gc.bookmarksfly.cn

Py:   "第一行\n第二行"
来源：http://eb.jianghongdianzi.cn

PHP:  "第一行\n第二行"
来源：http://da.szsharing.cn

JS:   "第一行\n第二行"
来源：http://br.wgjwhj.cn

TS:   "第一行\n第二行"
来源：http://vl.huanxung.cn

Java: "第一行\n第二行"
来源：http://jm.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://oz.newstarts.cn

Ruby: "第一行\n第二行"
来源：http://ac.jctech888.com.cn

C#:   "第一行\n第二行"
来源：http://qr.nszjky.cn

[A14] 注释写法
来源：http://hm.yuexingan06.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ui.chemitech.net.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://cy.chemitech.net.cn

JS:   // 单行；/* 多行 */
来源：http://on.lnxyls.cn

TS:   // 单行；/* 多行 */
来源：http://yh.asd995.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://sc.hahajie.cn

Go:   // 单行；/* 多行 */
来源：http://tp.colortex.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ma.bookmarksfly.cn

C#:   // 单行；/* 多行 */
来源：http://gw.wgjwhj.cn

[A15] 空值判断与默认值
来源：http://hh.hahajie.cn

Py:   value = data or "默认值"
来源：http://qq.panjiajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://pm.nszjky.cn

JS:   const value = data ?? "默认值";
来源：http://ud.haigaiapp.cn

TS:   const value = data ?? "默认值";
来源：http://db.nszjky.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://er.huixinmuqiang.cn

Go:   if data == "" { data = "默认值" }
来源：http://oc.haigaiapp.cn

Ruby: value = data || "默认值"
来源：http://hb.lnxyls.cn

C#:   var value = data ?? "默认值";
来源：http://bs.huixinmuqiang.cn

[A16] 真假值判断规则
来源：http://mj.lnxyls.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wg.chemitech.net.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ue.chemitech.net.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://av.szsharing.cn

TS:   if (!x) {}
来源：http://ea.huixiangedu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qw.yuexingan06.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ji.shxzskj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zs.shxzskj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gu.asd995.cn

[A17] 位运算
来源：http://jy.hnjuh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sd.yuexingan06.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qu.yuexingan06.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ak.hnjuh.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mz.szsharing.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ci.lnxyls.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ml.9csxet.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xl.szsharing.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ty.hahajie.cn

[A18] 字符与 ASCII 码互转
来源：http://ry.haigaiapp.cn

Py:   ord("A"); chr(65)
来源：http://dp.shxzskj.cn

PHP:  ord("A"); chr(65)
来源：http://ec.panjiajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wp.shxzukj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://so.colortex.cn

Java: (int) 'A'; (char) 65
来源：http://zq.nicolike.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rj.haigaiapp.cn

Ruby: "A".ord; 65.chr
来源：http://kz.shxzskj.cn

C#:   (int)'A'; (char)65
来源：http://ff.shxzukj.cn

[A19] 交换两个变量
来源：http://vb.nicolike.cn

Py:   a, b = b, a
来源：http://uw.hnjuh.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tl.hnjuh.cn

JS:   [a, b] = [b, a];
来源：http://hu.huixinmuqiang.cn

TS:   [a, b] = [b, a];
来源：http://et.colortex.cn

Java: int t = a; a = b; b = t;
来源：http://eh.hnjuh.cn

Go:   a, b = b, a
来源：http://ps.colortex.cn

Ruby: a, b = b, a
来源：http://gs.asd995.cn

C#:   (a, b) = (b, a);
来源：http://yc.haigaiapp.cn

[A20] 读取标准输入
来源：http://xy.nszjky.cn

Py:   name = input("请输入：")
来源：http://mx.newstarts.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ew.nszjky.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tb.gzmigu.cn

TS:   // Node.js：readline 模块
来源：http://jo.huixinmuqiang.cn

Java: new Scanner(System.in).nextLine()
来源：http://vz.wgjwhj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://by.shxzskj.cn

Ruby: gets.chomp
来源：http://nl.szsharing.cn

C#:   Console.ReadLine();
来源：http://jh.yuexingan06.cn

[A21] 保留指定小数位输出
来源：http://lq.asd995.cn

Py:   f"{3.14159:.2f}"
来源：http://fs.bjjhwx.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tq.shxzskj.cn

JS:   (3.14159).toFixed(2)
来源：http://xn.muxihuayi.cn

TS:   (3.14159).toFixed(2)
来源：http://bq.panjiajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://py.shxzukj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wc.gzmigu.cn

Ruby: format("%.2f", 3.14159)
来源：http://gs.bookmarksfly.cn

C#:   3.14159.ToString("F2")
来源：http://sy.newstarts.cn

[A22] 获取字符串长度
来源：http://kx.bjjhwx.cn

Py:   len(s)
来源：http://fk.nszjky.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://to.szsharing.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://su.huixiangedu.cn

TS:   s.length
来源：http://yx.panjiajie.cn

Java: s.length()
来源：http://fz.521024.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lt.nszjky.cn

Ruby: s.length
来源：http://ee.jctech888.com.cn

C#:   s.Length
来源：http://ri.shxzukj.cn

[A23] 大小写转换
来源：http://oh.shtwfgs.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ie.asd995.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://av.lnxyls.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wm.9csxet.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ih.colortex.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ek.huanxung.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://be.asd995.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vo.yuexingan06.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://in.bookmarksfly.cn

[A24] 去除首尾空白
来源：http://ia.hnjuh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zz.hnjuh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hc.wgjwhj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hb.asd995.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tw.nicolike.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://od.yuexingan06.cn

Go:   strings.TrimSpace(s)
来源：http://gv.yuntaijiaju.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ld.521024.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nd.huixiangedu.cn

[A25] 字符串比较
来源：http://hj.hnjuh.cn

Py:   s1 == s2; s1 != s2
来源：http://wj.nszjky.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://up.bookmarksfly.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nd.shxzskj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://aq.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dn.hahajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lp.jianghongdianzi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pp.shxzukj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://in.nszjky.cn

[A26] 类型转换总览
来源：http://dw.szsharing.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vj.shxzukj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://oq.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ic.gzmigu.cn

TS:   Number() String() Boolean() x as number
来源：http://ni.shxzukj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://td.asd995.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ab.szsharing.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ui.shxzukj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pc.nicolike.cn

================================================================================
来源：http://ta.szxytkj.cn

B. 流程控制
来源：http://ac.szsharing.cn

================================================================================
来源：http://ep.nszjky.cn

[B01] 条件判断 if / else
来源：http://hu.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rm.nszjky.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://iw.colortex.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xs.shxzukj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://go.nicolike.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ie.9csxet.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tr.9csxet.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://al.gzmigu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jr.jctech888.com.cn

[B02] 多分支 else if / elif
来源：http://vm.haigaiapp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://av.szsharing.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ix.asd995.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://od.jianghongdianzi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ar.bjjhwx.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ug.hahajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://td.shtwfgs.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ru.bjjhwx.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ua.colortex.cn

[B03] switch / match / case
来源：http://nx.panjiajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ox.521024.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ym.hnjuh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dl.jianghongdianzi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xv.hnjuh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xj.muxihuayi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nl.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ej.szsharing.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bv.nszjky.cn

[B04] for 计数循环
来源：http://qn.newstarts.cn

Py:   for i in range(10): print(i)
来源：http://xu.colortex.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gf.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ht.haigaiapp.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yd.yuexingan06.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ti.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nv.newstarts.cn

Ruby: 10.times { |i| puts i }
来源：http://uk.bjjhwx.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ym.huixinmuqiang.cn

[B05] 遍历数组 / 列表
来源：http://bk.szxytkj.cn

Py:   for item in arr: print(item)
来源：http://wa.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mu.szxytkj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://al.bjjhwx.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wi.szsharing.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fq.jianghongdianzi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lf.gzmigu.cn

Ruby: arr.each { |item| puts item }
来源：http://in.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zv.huixinmuqiang.cn

[B06] 遍历字典 / 对象
来源：http://vl.shxzukj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bf.hnjuh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cv.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cd.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hh.hnjuh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sc.szxytkj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ob.panjiajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pm.szxytkj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mm.bjjhwx.cn

[B07] while 循环
来源：http://aq.nszjky.cn

Py:   while i < 10: i += 1
来源：http://gs.gzmigu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wg.hnjuh.cn

JS:   while (i < 10) { i++; }
来源：http://hl.nszjky.cn

TS:   while (i < 10) { i++; }
来源：http://vd.yuntaijiaju.cn

Java: while (i < 10) { i++; }
来源：http://ua.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://md.newstarts.cn

Ruby: while i < 10; i += 1; end
来源：http://qd.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://nt.chemitech.net.cn

[B08] do-while（至少执行一次）
来源：http://vo.wgjwhj.cn

Py:   # 无 do-while：用 while True + break
来源：http://gh.lnxyls.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gp.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://ei.jctech888.com.cn

TS:   do { i++; } while (i < 10);
来源：http://uk.szsharing.cn

Java: do { i++; } while (i < 10);
来源：http://ql.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hf.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://sq.shxzukj.cn

C#:   do { i++; } while (i < 10);
来源：http://fr.bookmarksfly.cn

[B09] break 与 continue
来源：http://ys.yuntaijiaju.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mz.shtwfgs.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cg.jianghongdianzi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ds.jianghongdianzi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rc.shxzukj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sn.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cc.jctech888.com.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://px.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wr.newstarts.cn

[B10] 遍历同时拿索引
来源：http://ix.huixinmuqiang.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zz.521024.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zt.shxzukj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://av.huanxung.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gn.newstarts.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fx.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fa.wgjwhj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ii.muxihuayi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yk.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://ym.bjjhwx.cn

Py:   list(range(0, 10, 2))
来源：http://ag.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://ye.yuntaijiaju.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vs.yuntaijiaju.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bj.wgjwhj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yr.jianghongdianzi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yq.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://lo.huixinmuqiang.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oh.521024.cn

[B12] 跳出多层循环
来源：http://ft.muxihuayi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ru.gzmigu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dm.lnxyls.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tv.huanxung.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jc.hahajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tx.haigaiapp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uw.nicolike.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://iz.huanxung.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ty.wgjwhj.cn

[B13] 判断是否为数字
来源：http://fq.9csxet.cn

Py:   isinstance(x, (int, float))
来源：http://tw.jianghongdianzi.cn

PHP:  is_numeric($x)
来源：http://ly.jctech888.com.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ik.szxytkj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wt.szxytkj.cn

Java: x instanceof Number
来源：http://zz.huixiangedu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uu.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://ib.huixiangedu.cn

C#:   x is int or double or decimal
来源：http://dd.huanxung.cn

[B14] 判断值是否在集合内
来源：http://ab.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wo.shxzukj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ir.haigaiapp.cn

JS:   [1, 2, 3].includes(x)
来源：http://fw.9csxet.cn

TS:   [1, 2, 3].includes(x)
来源：http://vv.shxzukj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mu.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gs.muxihuayi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://uy.nszjky.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gk.shxzskj.cn

[B15] 布尔运算与取反
来源：http://wd.shxzukj.cn

Py:   a and b or not c
来源：http://ri.shxzskj.cn

PHP:  $a && $b || !$c
来源：http://mi.huanxung.cn

JS:   a && b || !c
来源：http://fo.yuntaijiaju.cn

TS:   a && b || !c
来源：http://ei.huanxung.cn

Java: a && b || !c
来源：http://ok.bjjhwx.cn

Go:   a && b || !c
来源：http://sk.nicolike.cn

Ruby: a && b || !c
来源：http://ve.szxytkj.cn

C#:   a && b || !c
来源：http://zy.nszjky.cn

[B16] 卫语句：不满足条件提前返回
来源：http://us.muxihuayi.cn

Py:   if not data: return
来源：http://xu.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://ak.521024.cn

JS:   if (!data) return;
来源：http://mp.hahajie.cn

TS:   if (!data) return;
来源：http://qq.colortex.cn

Java: if (data == null) return;
来源：http://jg.bjjhwx.cn

Go:   if data == nil { return }
来源：http://ea.jianghongdianzi.cn

Ruby: return if data.nil?
来源：http://po.szsharing.cn

C#:   if (data == null) return;
来源：http://hx.haigaiapp.cn

================================================================================
来源：http://du.haigaiapp.cn

C. 函数与作用域
来源：http://im.9csxet.cn

================================================================================
来源：http://lf.asd995.cn

[C01] 定义函数
来源：http://tv.shxzskj.cn

Py:   def add(a, b): return a + b
来源：http://xz.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://km.shxzukj.cn

JS:   function add(a, b) { return a + b; }
来源：http://pl.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qa.chemitech.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jp.panjiajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qq.szsharing.cn

Ruby: def add(a, b); a + b; end
来源：http://zq.yuntaijiaju.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ip.hahajie.cn

[C02] 默认参数
来源：http://tu.panjiajie.cn

Py:   def greet(name="World"): return name
来源：http://qp.haigaiapp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xb.shtwfgs.cn

JS:   function greet(name = "World") { return name; }
来源：http://ut.huanxung.cn


<!-- 参考信息 -->