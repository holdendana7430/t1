代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://zm.szxytkj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://bb.newstarts.cn

[A12] 字符串插值 / 格式化
来源：http://sp.shxzukj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nv.asd995.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ms.asd995.cn

JS:   `Hello, ${name}!`
来源：http://ab.huanxung.cn

TS:   `Hello, ${name}!`
来源：http://bq.szxytkj.cn

Java: "Hello, %s!".formatted(name)
来源：http://mt.szxytkj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xg.szxytkj.cn

Ruby: "Hello, #{name}!"
来源：http://qc.nicolike.cn

C#:   $"Hello, {name}!"
来源：http://qq.szsharing.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://gd.bookmarksfly.cn

Py:   "第一行\n第二行"
来源：http://sl.shxzskj.cn

PHP:  "第一行\n第二行"
来源：http://yy.chemitech.net.cn

JS:   "第一行\n第二行"
来源：http://qq.shtwfgs.cn

TS:   "第一行\n第二行"
来源：http://tk.yuexingan06.cn

Java: "第一行\n第二行"
来源：http://id.newstarts.cn

Go:   "第一行\n第二行"
来源：http://xp.newstarts.cn

Ruby: "第一行\n第二行"
来源：http://tx.hnjuh.cn

C#:   "第一行\n第二行"
来源：http://zq.hnjuh.cn

[A14] 注释写法
来源：http://yf.colortex.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://bs.szsharing.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://mw.jianghongdianzi.cn

JS:   // 单行；/* 多行 */
来源：http://kw.shtwfgs.cn

TS:   // 单行；/* 多行 */
来源：http://ut.chemitech.net.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jz.szsharing.cn

Go:   // 单行；/* 多行 */
来源：http://xa.shxzskj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://cr.wgjwhj.cn

C#:   // 单行；/* 多行 */
来源：http://nl.muxihuayi.cn

[A15] 空值判断与默认值
来源：http://kd.bjjhwx.cn

Py:   value = data or "默认值"
来源：http://fx.shxzukj.cn

PHP:  $value = $data ?? "默认值";
来源：http://yu.yuexingan06.cn

JS:   const value = data ?? "默认值";
来源：http://gi.9csxet.cn

TS:   const value = data ?? "默认值";
来源：http://jx.shxzskj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://it.haigaiapp.cn

Go:   if data == "" { data = "默认值" }
来源：http://lq.huixiangedu.cn

Ruby: value = data || "默认值"
来源：http://jx.huanxung.cn

C#:   var value = data ?? "默认值";
来源：http://pc.yuntaijiaju.cn

[A16] 真假值判断规则
来源：http://wt.colortex.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ua.nicolike.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vn.bookmarksfly.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fo.szsharing.cn

TS:   if (!x) {}
来源：http://at.lnxyls.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vx.nicolike.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://og.szsharing.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ee.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cm.shxzukj.cn

[A17] 位运算
来源：http://fo.jianghongdianzi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bv.haigaiapp.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ir.shxzskj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rs.huixinmuqiang.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cr.nszjky.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ou.muxihuayi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xx.muxihuayi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pm.szxytkj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jk.9csxet.cn

[A18] 字符与 ASCII 码互转
来源：http://tz.bookmarksfly.cn

Py:   ord("A"); chr(65)
来源：http://rp.hahajie.cn

PHP:  ord("A"); chr(65)
来源：http://zi.wgjwhj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bp.chemitech.net.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mb.haigaiapp.cn

Java: (int) 'A'; (char) 65
来源：http://jr.jctech888.com.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rm.muxihuayi.cn

Ruby: "A".ord; 65.chr
来源：http://co.huixinmuqiang.cn

C#:   (int)'A'; (char)65
来源：http://zi.bjjhwx.cn

[A19] 交换两个变量
来源：http://az.wgjwhj.cn

Py:   a, b = b, a
来源：http://ec.bookmarksfly.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qa.asd995.cn

JS:   [a, b] = [b, a];
来源：http://tl.bjjhwx.cn

TS:   [a, b] = [b, a];
来源：http://xg.lnxyls.cn

Java: int t = a; a = b; b = t;
来源：http://bl.asd995.cn

Go:   a, b = b, a
来源：http://wb.gzmigu.cn

Ruby: a, b = b, a
来源：http://pv.bookmarksfly.cn

C#:   (a, b) = (b, a);
来源：http://bq.huixinmuqiang.cn

[A20] 读取标准输入
来源：http://vk.huixinmuqiang.cn

Py:   name = input("请输入：")
来源：http://yz.shxzskj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://by.asd995.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jd.shtwfgs.cn

TS:   // Node.js：readline 模块
来源：http://bp.jianghongdianzi.cn

Java: new Scanner(System.in).nextLine()
来源：http://wq.panjiajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ju.nszjky.cn

Ruby: gets.chomp
来源：http://hu.bjjhwx.cn

C#:   Console.ReadLine();
来源：http://ua.521024.cn

[A21] 保留指定小数位输出
来源：http://ck.jianghongdianzi.cn

Py:   f"{3.14159:.2f}"
来源：http://rc.szxytkj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ek.hahajie.cn

JS:   (3.14159).toFixed(2)
来源：http://an.9csxet.cn

TS:   (3.14159).toFixed(2)
来源：http://jf.panjiajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://dp.muxihuayi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hj.chemitech.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://ug.szxytkj.cn

C#:   3.14159.ToString("F2")
来源：http://ah.nszjky.cn

[A22] 获取字符串长度
来源：http://ys.panjiajie.cn

Py:   len(s)
来源：http://bw.yuexingan06.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xr.newstarts.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://og.szsharing.cn

TS:   s.length
来源：http://wx.colortex.cn

Java: s.length()
来源：http://er.asd995.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tr.jianghongdianzi.cn

Ruby: s.length
来源：http://kf.lnxyls.cn

C#:   s.Length
来源：http://gh.chemitech.net.cn

[A23] 大小写转换
来源：http://zn.yuexingan06.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://er.gzmigu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jb.9csxet.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gl.bjjhwx.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ak.jianghongdianzi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rk.asd995.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://iz.shtwfgs.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bk.shtwfgs.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hd.521024.cn

[A24] 去除首尾空白
来源：http://ag.shxzskj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nw.colortex.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xe.huixiangedu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rq.colortex.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kh.yuntaijiaju.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xa.lnxyls.cn

Go:   strings.TrimSpace(s)
来源：http://wd.jianghongdianzi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fm.huixinmuqiang.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hg.521024.cn

[A25] 字符串比较
来源：http://la.szsharing.cn

Py:   s1 == s2; s1 != s2
来源：http://ki.gzmigu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dg.haigaiapp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jq.shxzskj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://op.bjjhwx.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cp.haigaiapp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pu.nszjky.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://kp.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uu.wgjwhj.cn

[A26] 类型转换总览
来源：http://qs.shtwfgs.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://oy.huanxung.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gn.yuexingan06.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pv.shxzukj.cn

TS:   Number() String() Boolean() x as number
来源：http://xu.hnjuh.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://eu.newstarts.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wj.9csxet.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vf.chemitech.net.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yu.9csxet.cn

================================================================================
来源：http://fc.haigaiapp.cn

B. 流程控制
来源：http://bz.muxihuayi.cn

================================================================================
来源：http://vo.szsharing.cn

[B01] 条件判断 if / else
来源：http://tm.bookmarksfly.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xd.huixinmuqiang.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qc.shtwfgs.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yt.shxzukj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tj.huixinmuqiang.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ue.nicolike.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ml.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ay.muxihuayi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jp.bjjhwx.cn

[B02] 多分支 else if / elif
来源：http://xp.jianghongdianzi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zo.huixiangedu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://in.huixiangedu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vu.jctech888.com.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iq.nicolike.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yc.9csxet.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://su.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sn.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qe.shxzukj.cn

[B03] switch / match / case
来源：http://un.panjiajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zh.jianghongdianzi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kf.huanxung.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ag.yuexingan06.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iv.shxzskj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://po.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ob.bjjhwx.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jm.bookmarksfly.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sd.9csxet.cn

[B04] for 计数循环
来源：http://mo.nszjky.cn

Py:   for i in range(10): print(i)
来源：http://hx.newstarts.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://aa.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qu.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://at.newstarts.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nh.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qi.yuexingan06.cn

Ruby: 10.times { |i| puts i }
来源：http://tn.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sd.nicolike.cn

[B05] 遍历数组 / 列表
来源：http://aq.hnjuh.cn

Py:   for item in arr: print(item)
来源：http://kq.yuntaijiaju.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rv.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://go.bookmarksfly.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ua.9csxet.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://us.521024.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lk.wgjwhj.cn

Ruby: arr.each { |item| puts item }
来源：http://br.huixinmuqiang.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yx.colortex.cn

[B06] 遍历字典 / 对象
来源：http://jw.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fl.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jw.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wv.newstarts.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fn.bookmarksfly.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pz.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zo.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xy.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://av.wgjwhj.cn

[B07] while 循环
来源：http://zt.newstarts.cn

Py:   while i < 10: i += 1
来源：http://yk.chemitech.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wd.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://wn.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://fz.haigaiapp.cn

Java: while (i < 10) { i++; }
来源：http://dg.haigaiapp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pb.muxihuayi.cn

Ruby: while i < 10; i += 1; end
来源：http://le.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://we.9csxet.cn

[B08] do-while（至少执行一次）
来源：http://vj.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://ix.lnxyls.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mg.szsharing.cn

JS:   do { i++; } while (i < 10);
来源：http://ok.jctech888.com.cn

TS:   do { i++; } while (i < 10);
来源：http://vd.bookmarksfly.cn

Java: do { i++; } while (i < 10);
来源：http://tj.yuexingan06.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sx.colortex.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xo.shxzukj.cn

C#:   do { i++; } while (i < 10);
来源：http://hu.huixiangedu.cn

[B09] break 与 continue
来源：http://zo.haigaiapp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wp.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wc.jctech888.com.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ng.nicolike.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tk.9csxet.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lx.lnxyls.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://me.bookmarksfly.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sa.newstarts.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qc.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://en.newstarts.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://um.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mz.shtwfgs.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sq.bookmarksfly.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ha.chemitech.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://am.yuntaijiaju.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jv.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://av.szxytkj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uj.shxzskj.cn

[B11] 生成数字序列 / 区间
来源：http://cz.shxzskj.cn

Py:   list(range(0, 10, 2))
来源：http://un.jctech888.com.cn

PHP:  range(0, 10, 2);
来源：http://md.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wk.newstarts.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ho.jianghongdianzi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hr.lnxyls.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jf.521024.cn

Ruby: (0...10).step(2).to_a
来源：http://zi.chemitech.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tu.bjjhwx.cn

[B12] 跳出多层循环
来源：http://up.muxihuayi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pv.panjiajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vh.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uh.colortex.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://eb.szsharing.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vn.bookmarksfly.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zj.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oa.9csxet.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fo.chemitech.net.cn

[B13] 判断是否为数字
来源：http://ua.lnxyls.cn

Py:   isinstance(x, (int, float))
来源：http://fn.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://uf.gzmigu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vv.521024.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://es.jctech888.com.cn

Java: x instanceof Number
来源：http://lt.huanxung.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tt.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://jc.huixiangedu.cn

C#:   x is int or double or decimal
来源：http://yl.yuntaijiaju.cn

[B14] 判断值是否在集合内
来源：http://jo.hahajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yn.hnjuh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gh.huanxung.cn

JS:   [1, 2, 3].includes(x)
来源：http://bq.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://yj.haigaiapp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ye.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yg.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mi.nszjky.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bt.jianghongdianzi.cn

[B15] 布尔运算与取反
来源：http://wc.521024.cn

Py:   a and b or not c
来源：http://rg.newstarts.cn

PHP:  $a && $b || !$c
来源：http://ib.haigaiapp.cn

JS:   a && b || !c
来源：http://tq.yuntaijiaju.cn

TS:   a && b || !c
来源：http://fo.huixinmuqiang.cn

Java: a && b || !c
来源：http://wn.yuntaijiaju.cn

Go:   a && b || !c
来源：http://hs.shxzukj.cn

Ruby: a && b || !c
来源：http://pi.yuexingan06.cn

C#:   a && b || !c
来源：http://uj.bjjhwx.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bs.521024.cn

Py:   if not data: return
来源：http://sp.nicolike.cn

PHP:  if (!$data) { return; }
来源：http://fr.huixiangedu.cn

JS:   if (!data) return;
来源：http://ow.jctech888.com.cn

TS:   if (!data) return;
来源：http://xp.muxihuayi.cn

Java: if (data == null) return;
来源：http://dj.gzmigu.cn

Go:   if data == nil { return }
来源：http://ol.szxytkj.cn

Ruby: return if data.nil?
来源：http://dd.huixiangedu.cn

C#:   if (data == null) return;
来源：http://pb.szxytkj.cn

================================================================================
来源：http://ru.bookmarksfly.cn

C. 函数与作用域
来源：http://yd.szsharing.cn

================================================================================
来源：http://vd.szsharing.cn

[C01] 定义函数
来源：http://on.jianghongdianzi.cn

Py:   def add(a, b): return a + b
来源：http://tw.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cq.szxytkj.cn

JS:   function add(a, b) { return a + b; }
来源：http://yp.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sx.huixiangedu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mx.asd995.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pk.colortex.cn

Ruby: def add(a, b); a + b; end
来源：http://wh.gzmigu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bc.hahajie.cn

[C02] 默认参数
来源：http://hg.newstarts.cn

Py:   def greet(name="World"): return name
来源：http://xd.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ad.panjiajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://hh.hahajie.cn


<!-- 参考信息 -->