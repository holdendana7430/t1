代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://nk.newstarts.cn

[A11] 条件表达式（三元）
来源：http://hs.colortex.cn

Py:   "yes" if x > 0 else "no"
来源：http://ga.szxytkj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://do.jctech888.com.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xi.jctech888.com.cn

TS:   x > 0 ? "yes" : "no"
来源：http://hq.panjiajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://td.newstarts.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://fy.bookmarksfly.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://su.nicolike.cn

C#:   x > 0 ? "yes" : "no"
来源：http://yu.bookmarksfly.cn

[A12] 字符串插值 / 格式化
来源：http://ol.jianghongdianzi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://on.gzmigu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nj.haigaiapp.cn

JS:   `Hello, ${name}!`
来源：http://zx.hnjuh.cn

TS:   `Hello, ${name}!`
来源：http://zg.shxzukj.cn

Java: "Hello, %s!".formatted(name)
来源：http://el.wgjwhj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tx.haigaiapp.cn

Ruby: "Hello, #{name}!"
来源：http://qb.gzmigu.cn

C#:   $"Hello, {name}!"
来源：http://dz.huixinmuqiang.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://bf.hnjuh.cn

Py:   "第一行\n第二行"
来源：http://vt.muxihuayi.cn

PHP:  "第一行\n第二行"
来源：http://qb.huixinmuqiang.cn

JS:   "第一行\n第二行"
来源：http://bv.gzmigu.cn

TS:   "第一行\n第二行"
来源：http://rk.nszjky.cn

Java: "第一行\n第二行"
来源：http://up.szxytkj.cn

Go:   "第一行\n第二行"
来源：http://kg.jctech888.com.cn

Ruby: "第一行\n第二行"
来源：http://nl.jianghongdianzi.cn

C#:   "第一行\n第二行"
来源：http://pi.colortex.cn

[A14] 注释写法
来源：http://fs.yuntaijiaju.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://lx.gzmigu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ds.muxihuayi.cn

JS:   // 单行；/* 多行 */
来源：http://rv.nicolike.cn

TS:   // 单行；/* 多行 */
来源：http://tc.huixinmuqiang.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://za.yuexingan06.cn

Go:   // 单行；/* 多行 */
来源：http://ey.huixiangedu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://oy.yuntaijiaju.cn

C#:   // 单行；/* 多行 */
来源：http://dq.szxytkj.cn

[A15] 空值判断与默认值
来源：http://ua.jianghongdianzi.cn

Py:   value = data or "默认值"
来源：http://vc.yuexingan06.cn

PHP:  $value = $data ?? "默认值";
来源：http://xp.colortex.cn

JS:   const value = data ?? "默认值";
来源：http://ok.shtwfgs.cn

TS:   const value = data ?? "默认值";
来源：http://jl.muxihuayi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ir.shxzukj.cn

Go:   if data == "" { data = "默认值" }
来源：http://eo.yuexingan06.cn

Ruby: value = data || "默认值"
来源：http://ka.muxihuayi.cn

C#:   var value = data ?? "默认值";
来源：http://jh.9csxet.cn

[A16] 真假值判断规则
来源：http://uu.nicolike.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zc.shxzukj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ay.panjiajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gs.nszjky.cn

TS:   if (!x) {}
来源：http://ji.nszjky.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ci.gzmigu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vm.nicolike.cn

Ruby: unless x            # nil 与 false 为假
来源：http://tq.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pr.521024.cn

[A17] 位运算
来源：http://jt.nszjky.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uv.shxzukj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xy.chemitech.net.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pd.9csxet.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uf.shxzukj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jt.wgjwhj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fy.jianghongdianzi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://co.chemitech.net.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wh.bookmarksfly.cn

[A18] 字符与 ASCII 码互转
来源：http://kr.chemitech.net.cn

Py:   ord("A"); chr(65)
来源：http://ed.jctech888.com.cn

PHP:  ord("A"); chr(65)
来源：http://xk.bjjhwx.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mv.szsharing.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ci.hahajie.cn

Java: (int) 'A'; (char) 65
来源：http://wl.wgjwhj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vq.huanxung.cn

Ruby: "A".ord; 65.chr
来源：http://hc.bookmarksfly.cn

C#:   (int)'A'; (char)65
来源：http://pp.jctech888.com.cn

[A19] 交换两个变量
来源：http://nh.9csxet.cn

Py:   a, b = b, a
来源：http://er.lnxyls.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tg.lnxyls.cn

JS:   [a, b] = [b, a];
来源：http://xl.huanxung.cn

TS:   [a, b] = [b, a];
来源：http://sr.newstarts.cn

Java: int t = a; a = b; b = t;
来源：http://lu.gzmigu.cn

Go:   a, b = b, a
来源：http://wh.newstarts.cn

Ruby: a, b = b, a
来源：http://xz.chemitech.net.cn

C#:   (a, b) = (b, a);
来源：http://kl.yuntaijiaju.cn

[A20] 读取标准输入
来源：http://ba.bjjhwx.cn

Py:   name = input("请输入：")
来源：http://yy.nszjky.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qp.9csxet.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kn.colortex.cn

TS:   // Node.js：readline 模块
来源：http://qh.9csxet.cn

Java: new Scanner(System.in).nextLine()
来源：http://xl.huanxung.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lf.huixiangedu.cn

Ruby: gets.chomp
来源：http://cn.szxytkj.cn

C#:   Console.ReadLine();
来源：http://az.szsharing.cn

[A21] 保留指定小数位输出
来源：http://hg.szxytkj.cn

Py:   f"{3.14159:.2f}"
来源：http://tx.huanxung.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wj.jianghongdianzi.cn

JS:   (3.14159).toFixed(2)
来源：http://to.yuexingan06.cn

TS:   (3.14159).toFixed(2)
来源：http://ge.szxytkj.cn

Java: String.format("%.2f", 3.14159)
来源：http://ci.huixinmuqiang.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vr.szsharing.cn

Ruby: format("%.2f", 3.14159)
来源：http://ue.yuntaijiaju.cn

C#:   3.14159.ToString("F2")
来源：http://xq.panjiajie.cn

[A22] 获取字符串长度
来源：http://jj.bjjhwx.cn

Py:   len(s)
来源：http://by.yuntaijiaju.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kx.hahajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nk.shxzukj.cn

TS:   s.length
来源：http://ft.bjjhwx.cn

Java: s.length()
来源：http://wu.jctech888.com.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://si.newstarts.cn

Ruby: s.length
来源：http://ku.wgjwhj.cn

C#:   s.Length
来源：http://td.shxzskj.cn

[A23] 大小写转换
来源：http://ia.yuexingan06.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wl.szsharing.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mr.panjiajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://iv.huanxung.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tz.9csxet.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ka.gzmigu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://am.haigaiapp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lr.hahajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ie.nszjky.cn

[A24] 去除首尾空白
来源：http://am.haigaiapp.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ti.gzmigu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ei.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kb.huixinmuqiang.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ev.yuntaijiaju.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vj.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://sv.yuexingan06.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ru.huanxung.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qp.wgjwhj.cn

[A25] 字符串比较
来源：http://eo.shtwfgs.cn

Py:   s1 == s2; s1 != s2
来源：http://ds.yuntaijiaju.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gu.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lc.jctech888.com.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pw.muxihuayi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vz.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zi.gzmigu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ss.bjjhwx.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://te.szsharing.cn

[A26] 类型转换总览
来源：http://mb.jianghongdianzi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yu.hnjuh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kq.chemitech.net.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://en.hnjuh.cn

TS:   Number() String() Boolean() x as number
来源：http://br.yuexingan06.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pz.lnxyls.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://he.muxihuayi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pa.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hr.hahajie.cn

================================================================================
来源：http://ix.hnjuh.cn

B. 流程控制
来源：http://gc.wgjwhj.cn

================================================================================
来源：http://dp.panjiajie.cn

[B01] 条件判断 if / else
来源：http://ha.shxzukj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dd.bookmarksfly.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://of.chemitech.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zm.jctech888.com.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fd.yuexingan06.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ui.panjiajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.huanxung.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jt.szsharing.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sf.nszjky.cn

[B02] 多分支 else if / elif
来源：http://ex.haigaiapp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pf.wgjwhj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rt.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kj.muxihuayi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ao.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://km.jianghongdianzi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://os.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cp.wgjwhj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hc.bookmarksfly.cn

[B03] switch / match / case
来源：http://ab.jianghongdianzi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://se.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://om.9csxet.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gu.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qd.jctech888.com.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yr.jctech888.com.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hl.shtwfgs.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vc.szsharing.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qu.colortex.cn

[B04] for 计数循环
来源：http://ok.szxytkj.cn

Py:   for i in range(10): print(i)
来源：http://zb.yuntaijiaju.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rr.lnxyls.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ha.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cc.9csxet.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gr.bjjhwx.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fa.chemitech.net.cn

Ruby: 10.times { |i| puts i }
来源：http://yu.newstarts.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nt.hnjuh.cn

[B05] 遍历数组 / 列表
来源：http://bv.lnxyls.cn

Py:   for item in arr: print(item)
来源：http://fq.lnxyls.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://up.huanxung.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vm.9csxet.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kh.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ch.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wp.muxihuayi.cn

Ruby: arr.each { |item| puts item }
来源：http://lv.bookmarksfly.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yd.huixiangedu.cn

[B06] 遍历字典 / 对象
来源：http://da.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rm.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zt.9csxet.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cu.bjjhwx.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pq.nicolike.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cp.gzmigu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yq.hnjuh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fl.panjiajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mb.9csxet.cn

[B07] while 循环
来源：http://bb.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://jm.panjiajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ss.huanxung.cn

JS:   while (i < 10) { i++; }
来源：http://cf.jctech888.com.cn

TS:   while (i < 10) { i++; }
来源：http://rn.yuntaijiaju.cn

Java: while (i < 10) { i++; }
来源：http://rm.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fq.521024.cn

Ruby: while i < 10; i += 1; end
来源：http://dm.huixinmuqiang.cn

C#:   while (i < 10) { i++; }
来源：http://dd.hahajie.cn

[B08] do-while（至少执行一次）
来源：http://dw.chemitech.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://ko.asd995.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ca.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://sr.bookmarksfly.cn

TS:   do { i++; } while (i < 10);
来源：http://st.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://mx.huixinmuqiang.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fa.muxihuayi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://js.huixinmuqiang.cn

C#:   do { i++; } while (i < 10);
来源：http://jw.521024.cn

[B09] break 与 continue
来源：http://aj.jianghongdianzi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nk.huixinmuqiang.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mm.jctech888.com.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://am.yuntaijiaju.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rf.haigaiapp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ph.yuexingan06.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dr.asd995.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pg.shtwfgs.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://io.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://kk.wgjwhj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fi.hahajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sj.panjiajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lf.chemitech.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zh.shxzskj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zq.bookmarksfly.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kv.hnjuh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zf.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.szsharing.cn

[B11] 生成数字序列 / 区间
来源：http://vb.9csxet.cn

Py:   list(range(0, 10, 2))
来源：http://tj.haigaiapp.cn

PHP:  range(0, 10, 2);
来源：http://mf.nicolike.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fp.lnxyls.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mm.shxzukj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://em.szsharing.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vl.muxihuayi.cn

Ruby: (0...10).step(2).to_a
来源：http://gk.shtwfgs.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://aq.chemitech.net.cn

[B12] 跳出多层循环
来源：http://jm.shxzukj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rp.lnxyls.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hw.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://js.yuexingan06.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tw.newstarts.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nu.jctech888.com.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ub.chemitech.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fi.chemitech.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cu.shtwfgs.cn

[B13] 判断是否为数字
来源：http://zo.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://uz.shtwfgs.cn

PHP:  is_numeric($x)
来源：http://po.szsharing.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ba.newstarts.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ew.jianghongdianzi.cn

Java: x instanceof Number
来源：http://ly.yuexingan06.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yo.9csxet.cn

Ruby: x.is_a?(Numeric)
来源：http://jd.panjiajie.cn

C#:   x is int or double or decimal
来源：http://sj.gzmigu.cn

[B14] 判断值是否在集合内
来源：http://nf.huixiangedu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pl.hnjuh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ev.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://fi.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://al.muxihuayi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lu.hnjuh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hv.bookmarksfly.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ko.huanxung.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pf.chemitech.net.cn

[B15] 布尔运算与取反
来源：http://ya.wgjwhj.cn

Py:   a and b or not c
来源：http://rm.szsharing.cn

PHP:  $a && $b || !$c
来源：http://sj.jctech888.com.cn

JS:   a && b || !c
来源：http://ev.gzmigu.cn

TS:   a && b || !c
来源：http://ke.yuexingan06.cn

Java: a && b || !c
来源：http://vw.nicolike.cn

Go:   a && b || !c
来源：http://to.jctech888.com.cn

Ruby: a && b || !c
来源：http://rf.szsharing.cn

C#:   a && b || !c
来源：http://hp.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cw.wgjwhj.cn

Py:   if not data: return
来源：http://hg.muxihuayi.cn

PHP:  if (!$data) { return; }
来源：http://xq.szxytkj.cn

JS:   if (!data) return;
来源：http://rd.nicolike.cn

TS:   if (!data) return;
来源：http://eo.yuexingan06.cn

Java: if (data == null) return;
来源：http://vt.bjjhwx.cn

Go:   if data == nil { return }
来源：http://xm.yuntaijiaju.cn

Ruby: return if data.nil?
来源：http://fi.newstarts.cn

C#:   if (data == null) return;
来源：http://qr.yuntaijiaju.cn

================================================================================
来源：http://rb.hahajie.cn

C. 函数与作用域
来源：http://ch.nicolike.cn

================================================================================
来源：http://qc.muxihuayi.cn

[C01] 定义函数
来源：http://xc.newstarts.cn

Py:   def add(a, b): return a + b
来源：http://sv.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gj.muxihuayi.cn

JS:   function add(a, b) { return a + b; }
来源：http://wf.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ni.bjjhwx.cn


<!-- 参考信息 -->