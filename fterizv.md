代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://mt.jctech888.com.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dd.bjjhwx.cn

Java: x > 0 ? "yes" : "no"
来源：http://gm.9csxet.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xf.gzmigu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://up.wgjwhj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://zl.bjjhwx.cn

[A12] 字符串插值 / 格式化
来源：http://ew.bookmarksfly.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bg.gzmigu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xo.hnjuh.cn

JS:   `Hello, ${name}!`
来源：http://jp.lnxyls.cn

TS:   `Hello, ${name}!`
来源：http://ub.hnjuh.cn

Java: "Hello, %s!".formatted(name)
来源：http://oa.9csxet.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qn.huixiangedu.cn

Ruby: "Hello, #{name}!"
来源：http://xv.wgjwhj.cn

C#:   $"Hello, {name}!"
来源：http://hq.bookmarksfly.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://dc.yuntaijiaju.cn

Py:   "第一行\n第二行"
来源：http://lw.huanxung.cn

PHP:  "第一行\n第二行"
来源：http://wq.newstarts.cn

JS:   "第一行\n第二行"
来源：http://km.szsharing.cn

TS:   "第一行\n第二行"
来源：http://vn.panjiajie.cn

Java: "第一行\n第二行"
来源：http://cq.szxytkj.cn

Go:   "第一行\n第二行"
来源：http://op.huixinmuqiang.cn

Ruby: "第一行\n第二行"
来源：http://ss.huixinmuqiang.cn

C#:   "第一行\n第二行"
来源：http://wf.bookmarksfly.cn

[A14] 注释写法
来源：http://co.szsharing.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://xo.muxihuayi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://mu.hnjuh.cn

JS:   // 单行；/* 多行 */
来源：http://fi.lnxyls.cn

TS:   // 单行；/* 多行 */
来源：http://gg.shtwfgs.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qa.lnxyls.cn

Go:   // 单行；/* 多行 */
来源：http://xz.hnjuh.cn

Ruby: # 单行；=begin 多行 =end
来源：http://no.huanxung.cn

C#:   // 单行；/* 多行 */
来源：http://hi.shtwfgs.cn

[A15] 空值判断与默认值
来源：http://vj.nszjky.cn

Py:   value = data or "默认值"
来源：http://om.bjjhwx.cn

PHP:  $value = $data ?? "默认值";
来源：http://if.nszjky.cn

JS:   const value = data ?? "默认值";
来源：http://ej.colortex.cn

TS:   const value = data ?? "默认值";
来源：http://db.jianghongdianzi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ua.panjiajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://wi.nicolike.cn

Ruby: value = data || "默认值"
来源：http://yq.huixiangedu.cn

C#:   var value = data ?? "默认值";
来源：http://kz.gzmigu.cn

[A16] 真假值判断规则
来源：http://yh.shxzskj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gs.wgjwhj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fb.lnxyls.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zc.szxytkj.cn

TS:   if (!x) {}
来源：http://pf.haigaiapp.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lb.nszjky.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xm.szsharing.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ud.szxytkj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://dr.muxihuayi.cn

[A17] 位运算
来源：http://zh.9csxet.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ht.chemitech.net.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://po.chemitech.net.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lw.newstarts.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ti.bookmarksfly.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dq.hnjuh.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jy.szsharing.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fx.bookmarksfly.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pk.huixiangedu.cn

[A18] 字符与 ASCII 码互转
来源：http://pd.haigaiapp.cn

Py:   ord("A"); chr(65)
来源：http://uh.wgjwhj.cn

PHP:  ord("A"); chr(65)
来源：http://je.colortex.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wb.9csxet.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ig.shtwfgs.cn

Java: (int) 'A'; (char) 65
来源：http://qw.shtwfgs.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ve.asd995.cn

Ruby: "A".ord; 65.chr
来源：http://ro.bjjhwx.cn

C#:   (int)'A'; (char)65
来源：http://dm.colortex.cn

[A19] 交换两个变量
来源：http://ko.bookmarksfly.cn

Py:   a, b = b, a
来源：http://tk.wgjwhj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ld.shtwfgs.cn

JS:   [a, b] = [b, a];
来源：http://zp.haigaiapp.cn

TS:   [a, b] = [b, a];
来源：http://xm.jctech888.com.cn

Java: int t = a; a = b; b = t;
来源：http://vw.newstarts.cn

Go:   a, b = b, a
来源：http://mz.lnxyls.cn

Ruby: a, b = b, a
来源：http://fq.shxzukj.cn

C#:   (a, b) = (b, a);
来源：http://su.muxihuayi.cn

[A20] 读取标准输入
来源：http://ll.shxzukj.cn

Py:   name = input("请输入：")
来源：http://pc.haigaiapp.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://nn.lnxyls.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ju.nszjky.cn

TS:   // Node.js：readline 模块
来源：http://ur.chemitech.net.cn

Java: new Scanner(System.in).nextLine()
来源：http://pv.newstarts.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hc.szxytkj.cn

Ruby: gets.chomp
来源：http://dk.shtwfgs.cn

C#:   Console.ReadLine();
来源：http://yj.colortex.cn

[A21] 保留指定小数位输出
来源：http://xw.hahajie.cn

Py:   f"{3.14159:.2f}"
来源：http://ks.hnjuh.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xb.newstarts.cn

JS:   (3.14159).toFixed(2)
来源：http://ar.hnjuh.cn

TS:   (3.14159).toFixed(2)
来源：http://dq.hahajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://mk.jianghongdianzi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ih.panjiajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://wa.chemitech.net.cn

C#:   3.14159.ToString("F2")
来源：http://ls.hahajie.cn

[A22] 获取字符串长度
来源：http://av.szxytkj.cn

Py:   len(s)
来源：http://be.nszjky.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pg.huixinmuqiang.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lk.huanxung.cn

TS:   s.length
来源：http://xz.jianghongdianzi.cn

Java: s.length()
来源：http://mo.newstarts.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tc.9csxet.cn

Ruby: s.length
来源：http://ay.shtwfgs.cn

C#:   s.Length
来源：http://vz.wgjwhj.cn

[A23] 大小写转换
来源：http://qy.haigaiapp.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rh.nicolike.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pe.nszjky.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gn.newstarts.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mp.9csxet.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ql.9csxet.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gd.muxihuayi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vx.szxytkj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://co.bookmarksfly.cn

[A24] 去除首尾空白
来源：http://xz.wgjwhj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lg.szxytkj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ec.wgjwhj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gt.asd995.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rw.huanxung.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://td.newstarts.cn

Go:   strings.TrimSpace(s)
来源：http://fb.lnxyls.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gp.bookmarksfly.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hd.szsharing.cn

[A25] 字符串比较
来源：http://xd.shtwfgs.cn

Py:   s1 == s2; s1 != s2
来源：http://jt.521024.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sa.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bx.szsharing.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qq.gzmigu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ie.shtwfgs.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bg.gzmigu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://kk.muxihuayi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xo.colortex.cn

[A26] 类型转换总览
来源：http://rz.shtwfgs.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vn.9csxet.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ni.huixinmuqiang.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://py.szsharing.cn

TS:   Number() String() Boolean() x as number
来源：http://od.hahajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dc.bookmarksfly.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pn.nicolike.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dj.szsharing.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ct.nicolike.cn

================================================================================
来源：http://mx.haigaiapp.cn

B. 流程控制
来源：http://jz.9csxet.cn

================================================================================
来源：http://cw.huixiangedu.cn

[B01] 条件判断 if / else
来源：http://nw.jctech888.com.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ia.szxytkj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wl.nicolike.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mn.colortex.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ya.shxzukj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ib.shxzukj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zh.yuntaijiaju.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lo.shtwfgs.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fs.shtwfgs.cn

[B02] 多分支 else if / elif
来源：http://bo.haigaiapp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ge.shxzskj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://oj.shxzukj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ab.lnxyls.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yx.jctech888.com.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wy.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sl.521024.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tn.nicolike.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://os.yuexingan06.cn

[B03] switch / match / case
来源：http://qt.colortex.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xu.wgjwhj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ns.szsharing.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rp.shxzukj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rp.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hg.colortex.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nz.shtwfgs.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sc.panjiajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://be.521024.cn

[B04] for 计数循环
来源：http://tb.newstarts.cn

Py:   for i in range(10): print(i)
来源：http://dm.shtwfgs.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nh.szsharing.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ze.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rq.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qq.newstarts.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uc.shxzukj.cn

Ruby: 10.times { |i| puts i }
来源：http://ab.bookmarksfly.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ik.huixinmuqiang.cn

[B05] 遍历数组 / 列表
来源：http://cf.wgjwhj.cn

Py:   for item in arr: print(item)
来源：http://aj.asd995.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qc.haigaiapp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ug.jianghongdianzi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://il.bjjhwx.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sm.gzmigu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fd.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://jr.colortex.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ml.9csxet.cn

[B06] 遍历字典 / 对象
来源：http://nn.panjiajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gc.huixinmuqiang.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fx.bookmarksfly.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wn.nicolike.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eo.bookmarksfly.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://py.hnjuh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jy.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bz.gzmigu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lf.jianghongdianzi.cn

[B07] while 循环
来源：http://pe.huixinmuqiang.cn

Py:   while i < 10: i += 1
来源：http://yn.gzmigu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xk.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://ab.nszjky.cn

TS:   while (i < 10) { i++; }
来源：http://bn.shxzukj.cn

Java: while (i < 10) { i++; }
来源：http://io.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hx.panjiajie.cn

Ruby: while i < 10; i += 1; end
来源：http://ou.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://dd.haigaiapp.cn

[B08] do-while（至少执行一次）
来源：http://bm.yuntaijiaju.cn

Py:   # 无 do-while：用 while True + break
来源：http://pr.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zx.szxytkj.cn

JS:   do { i++; } while (i < 10);
来源：http://xt.huanxung.cn

TS:   do { i++; } while (i < 10);
来源：http://hd.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://oa.muxihuayi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bc.yuntaijiaju.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lw.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://iz.shtwfgs.cn

[B09] break 与 continue
来源：http://zq.bookmarksfly.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dj.nszjky.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wi.nszjky.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://os.nicolike.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gu.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tz.shxzskj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xt.521024.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gw.521024.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jx.wgjwhj.cn

[B10] 遍历同时拿索引
来源：http://wa.521024.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://af.gzmigu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hy.yuexingan06.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://my.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ml.521024.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.panjiajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ly.chemitech.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bw.shtwfgs.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fz.huanxung.cn

[B11] 生成数字序列 / 区间
来源：http://ry.jctech888.com.cn

Py:   list(range(0, 10, 2))
来源：http://ea.yuexingan06.cn

PHP:  range(0, 10, 2);
来源：http://fn.yuntaijiaju.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wo.jianghongdianzi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jq.szxytkj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xw.shtwfgs.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yi.lnxyls.cn

Ruby: (0...10).step(2).to_a
来源：http://tb.shtwfgs.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://le.huixiangedu.cn

[B12] 跳出多层循环
来源：http://mn.muxihuayi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rv.521024.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sb.nszjky.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kj.gzmigu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uy.szxytkj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://oj.shxzskj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dh.521024.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ct.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cc.yuntaijiaju.cn

[B13] 判断是否为数字
来源：http://qh.jctech888.com.cn

Py:   isinstance(x, (int, float))
来源：http://wd.shtwfgs.cn

PHP:  is_numeric($x)
来源：http://ab.chemitech.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dc.chemitech.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qo.wgjwhj.cn

Java: x instanceof Number
来源：http://yb.jctech888.com.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zs.huanxung.cn

Ruby: x.is_a?(Numeric)
来源：http://sk.shtwfgs.cn

C#:   x is int or double or decimal
来源：http://bz.nicolike.cn

[B14] 判断值是否在集合内
来源：http://qi.hnjuh.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qh.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bc.newstarts.cn

JS:   [1, 2, 3].includes(x)
来源：http://bu.huanxung.cn

TS:   [1, 2, 3].includes(x)
来源：http://hn.wgjwhj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://br.huixiangedu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ph.huixiangedu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://oe.bjjhwx.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sy.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://dx.chemitech.net.cn

Py:   a and b or not c
来源：http://ky.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://ty.lnxyls.cn

JS:   a && b || !c
来源：http://qn.haigaiapp.cn

TS:   a && b || !c
来源：http://uy.hahajie.cn

Java: a && b || !c
来源：http://dn.nszjky.cn

Go:   a && b || !c
来源：http://nc.szsharing.cn

Ruby: a && b || !c
来源：http://pa.huanxung.cn

C#:   a && b || !c
来源：http://lh.panjiajie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vq.521024.cn

Py:   if not data: return
来源：http://jq.yuexingan06.cn

PHP:  if (!$data) { return; }
来源：http://ge.muxihuayi.cn

JS:   if (!data) return;
来源：http://hd.colortex.cn

TS:   if (!data) return;
来源：http://fp.shxzukj.cn

Java: if (data == null) return;
来源：http://tf.huixinmuqiang.cn

Go:   if data == nil { return }
来源：http://ld.szxytkj.cn

Ruby: return if data.nil?
来源：http://dp.hnjuh.cn

C#:   if (data == null) return;
来源：http://lw.haigaiapp.cn

================================================================================
来源：http://zl.bjjhwx.cn

C. 函数与作用域
来源：http://qw.hnjuh.cn

================================================================================
来源：http://fn.jianghongdianzi.cn

[C01] 定义函数
来源：http://wk.panjiajie.cn

Py:   def add(a, b): return a + b
来源：http://ya.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mf.yuexingan06.cn

JS:   function add(a, b) { return a + b; }
来源：http://kp.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dc.shtwfgs.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rb.521024.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cp.hahajie.cn

Ruby: def add(a, b); a + b; end
来源：http://nk.newstarts.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ef.szsharing.cn


<!-- 参考信息 -->