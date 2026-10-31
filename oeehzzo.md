代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xv.hahajie.cn

Ruby: "Hello, #{name}!"
来源：http://zy.wgjwhj.cn

C#:   $"Hello, {name}!"
来源：http://ip.hnjuh.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ni.colortex.cn

Py:   "第一行\n第二行"
来源：http://mz.shtwfgs.cn

PHP:  "第一行\n第二行"
来源：http://jm.521024.cn

JS:   "第一行\n第二行"
来源：http://du.bookmarksfly.cn

TS:   "第一行\n第二行"
来源：http://od.huixinmuqiang.cn

Java: "第一行\n第二行"
来源：http://jl.shtwfgs.cn

Go:   "第一行\n第二行"
来源：http://zm.colortex.cn

Ruby: "第一行\n第二行"
来源：http://sz.asd995.cn

C#:   "第一行\n第二行"
来源：http://to.wgjwhj.cn

[A14] 注释写法
来源：http://gf.lnxyls.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://xl.panjiajie.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://mw.colortex.cn

JS:   // 单行；/* 多行 */
来源：http://ue.huixinmuqiang.cn

TS:   // 单行；/* 多行 */
来源：http://av.szsharing.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fe.newstarts.cn

Go:   // 单行；/* 多行 */
来源：http://gi.huixiangedu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://mg.panjiajie.cn

C#:   // 单行；/* 多行 */
来源：http://gc.gzmigu.cn

[A15] 空值判断与默认值
来源：http://fn.bookmarksfly.cn

Py:   value = data or "默认值"
来源：http://gz.yuntaijiaju.cn

PHP:  $value = $data ?? "默认值";
来源：http://xl.szsharing.cn

JS:   const value = data ?? "默认值";
来源：http://bb.jctech888.com.cn

TS:   const value = data ?? "默认值";
来源：http://fx.yuexingan06.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pb.nszjky.cn

Go:   if data == "" { data = "默认值" }
来源：http://an.jctech888.com.cn

Ruby: value = data || "默认值"
来源：http://hu.panjiajie.cn

C#:   var value = data ?? "默认值";
来源：http://xw.colortex.cn

[A16] 真假值判断规则
来源：http://jh.jianghongdianzi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bx.panjiajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bo.huanxung.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ei.gzmigu.cn

TS:   if (!x) {}
来源：http://js.colortex.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tv.asd995.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jj.9csxet.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gz.asd995.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pc.huanxung.cn

[A17] 位运算
来源：http://vn.haigaiapp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dt.szxytkj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cu.521024.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vj.wgjwhj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pa.shtwfgs.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bz.huixinmuqiang.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ne.gzmigu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jn.hahajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vz.huixiangedu.cn

[A18] 字符与 ASCII 码互转
来源：http://as.muxihuayi.cn

Py:   ord("A"); chr(65)
来源：http://rl.shxzukj.cn

PHP:  ord("A"); chr(65)
来源：http://yj.panjiajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yo.gzmigu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bo.shxzukj.cn

Java: (int) 'A'; (char) 65
来源：http://lt.haigaiapp.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dc.hahajie.cn

Ruby: "A".ord; 65.chr
来源：http://dg.huixinmuqiang.cn

C#:   (int)'A'; (char)65
来源：http://mn.gzmigu.cn

[A19] 交换两个变量
来源：http://do.asd995.cn

Py:   a, b = b, a
来源：http://xh.wgjwhj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://mi.shxzskj.cn

JS:   [a, b] = [b, a];
来源：http://un.szsharing.cn

TS:   [a, b] = [b, a];
来源：http://mo.szxytkj.cn

Java: int t = a; a = b; b = t;
来源：http://jo.yuntaijiaju.cn

Go:   a, b = b, a
来源：http://xd.gzmigu.cn

Ruby: a, b = b, a
来源：http://pq.bookmarksfly.cn

C#:   (a, b) = (b, a);
来源：http://zl.huanxung.cn

[A20] 读取标准输入
来源：http://ew.jctech888.com.cn

Py:   name = input("请输入：")
来源：http://su.yuexingan06.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://go.lnxyls.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zj.bookmarksfly.cn

TS:   // Node.js：readline 模块
来源：http://wh.asd995.cn

Java: new Scanner(System.in).nextLine()
来源：http://tu.hnjuh.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tp.521024.cn

Ruby: gets.chomp
来源：http://qa.gzmigu.cn

C#:   Console.ReadLine();
来源：http://gz.gzmigu.cn

[A21] 保留指定小数位输出
来源：http://el.haigaiapp.cn

Py:   f"{3.14159:.2f}"
来源：http://ji.szxytkj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://iv.gzmigu.cn

JS:   (3.14159).toFixed(2)
来源：http://gh.hnjuh.cn

TS:   (3.14159).toFixed(2)
来源：http://hj.szxytkj.cn

Java: String.format("%.2f", 3.14159)
来源：http://mt.nszjky.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dj.szxytkj.cn

Ruby: format("%.2f", 3.14159)
来源：http://yl.wgjwhj.cn

C#:   3.14159.ToString("F2")
来源：http://mt.nicolike.cn

[A22] 获取字符串长度
来源：http://br.nicolike.cn

Py:   len(s)
来源：http://ag.asd995.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://na.jctech888.com.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wu.huixinmuqiang.cn

TS:   s.length
来源：http://lm.yuntaijiaju.cn

Java: s.length()
来源：http://ex.colortex.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ud.panjiajie.cn

Ruby: s.length
来源：http://ao.huanxung.cn

C#:   s.Length
来源：http://eo.wgjwhj.cn

[A23] 大小写转换
来源：http://ab.haigaiapp.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nb.shxzukj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dp.shtwfgs.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ok.jctech888.com.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.lnxyls.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ia.lnxyls.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lf.gzmigu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nc.gzmigu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jc.panjiajie.cn

[A24] 去除首尾空白
来源：http://iw.shtwfgs.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://id.shxzskj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dj.hnjuh.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qz.gzmigu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sa.gzmigu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rf.szsharing.cn

Go:   strings.TrimSpace(s)
来源：http://yk.jianghongdianzi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://af.shtwfgs.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ex.shxzskj.cn

[A25] 字符串比较
来源：http://ja.panjiajie.cn

Py:   s1 == s2; s1 != s2
来源：http://ly.panjiajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pz.colortex.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zi.newstarts.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wo.9csxet.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zh.bookmarksfly.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ds.9csxet.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gh.szsharing.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yc.521024.cn

[A26] 类型转换总览
来源：http://ka.colortex.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://km.wgjwhj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vk.asd995.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vn.shtwfgs.cn

TS:   Number() String() Boolean() x as number
来源：http://qe.shxzukj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zf.wgjwhj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lc.colortex.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pl.yuexingan06.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yp.bookmarksfly.cn

================================================================================
来源：http://kl.hahajie.cn

B. 流程控制
来源：http://oe.shxzskj.cn

================================================================================
来源：http://bq.9csxet.cn

[B01] 条件判断 if / else
来源：http://um.jianghongdianzi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ia.chemitech.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ax.panjiajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yr.huixinmuqiang.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qy.shtwfgs.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ck.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nh.9csxet.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kc.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mc.chemitech.net.cn

[B02] 多分支 else if / elif
来源：http://la.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ii.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gn.szsharing.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ku.gzmigu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sb.haigaiapp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xm.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zl.nicolike.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xc.shxzskj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lx.newstarts.cn

[B03] switch / match / case
来源：http://bb.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://oa.muxihuayi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dp.muxihuayi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xa.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ll.lnxyls.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://oe.haigaiapp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dc.nicolike.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lr.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://aw.hahajie.cn

[B04] for 计数循环
来源：http://ld.521024.cn

Py:   for i in range(10): print(i)
来源：http://lu.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hj.asd995.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pu.szxytkj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://im.jctech888.com.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ww.yuexingan06.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ro.jctech888.com.cn

Ruby: 10.times { |i| puts i }
来源：http://uy.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jo.jianghongdianzi.cn

[B05] 遍历数组 / 列表
来源：http://ol.colortex.cn

Py:   for item in arr: print(item)
来源：http://yc.chemitech.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://so.colortex.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gv.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zp.shxzukj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kf.huixiangedu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wq.colortex.cn

Ruby: arr.each { |item| puts item }
来源：http://dm.szxytkj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ir.huixiangedu.cn

[B06] 遍历字典 / 对象
来源：http://ze.yuntaijiaju.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cw.shtwfgs.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cq.bookmarksfly.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vo.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dc.newstarts.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://eu.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xq.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xj.asd995.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nh.asd995.cn

[B07] while 循环
来源：http://ix.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://ka.shtwfgs.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pc.szxytkj.cn

JS:   while (i < 10) { i++; }
来源：http://sx.chemitech.net.cn

TS:   while (i < 10) { i++; }
来源：http://oh.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://we.huanxung.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ch.haigaiapp.cn

Ruby: while i < 10; i += 1; end
来源：http://fi.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://lc.nszjky.cn

[B08] do-while（至少执行一次）
来源：http://ds.wgjwhj.cn

Py:   # 无 do-while：用 while True + break
来源：http://tv.jianghongdianzi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://se.chemitech.net.cn

JS:   do { i++; } while (i < 10);
来源：http://wu.szxytkj.cn

TS:   do { i++; } while (i < 10);
来源：http://cw.shxzskj.cn

Java: do { i++; } while (i < 10);
来源：http://bd.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vh.asd995.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ex.yuexingan06.cn

C#:   do { i++; } while (i < 10);
来源：http://rh.nicolike.cn

[B09] break 与 continue
来源：http://ip.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kh.shxzskj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cd.huixiangedu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fd.huixinmuqiang.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gv.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ig.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://iw.521024.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pg.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bp.nszjky.cn

[B10] 遍历同时拿索引
来源：http://ld.chemitech.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gh.szxytkj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ue.szsharing.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cn.9csxet.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mw.szxytkj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kl.huixinmuqiang.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dp.chemitech.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bx.szsharing.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hv.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://fu.lnxyls.cn

Py:   list(range(0, 10, 2))
来源：http://pv.nicolike.cn

PHP:  range(0, 10, 2);
来源：http://tl.szxytkj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jf.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yr.asd995.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hx.huanxung.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xd.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://qu.szsharing.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pa.asd995.cn

[B12] 跳出多层循环
来源：http://cj.shxzskj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fj.yuntaijiaju.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mb.bjjhwx.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oi.hnjuh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sg.shtwfgs.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hh.jianghongdianzi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://du.chemitech.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gy.hnjuh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uv.jctech888.com.cn

[B13] 判断是否为数字
来源：http://lj.szsharing.cn

Py:   isinstance(x, (int, float))
来源：http://fj.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://tu.panjiajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hp.shxzukj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lw.muxihuayi.cn

Java: x instanceof Number
来源：http://vt.jianghongdianzi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ih.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://eq.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://aa.hnjuh.cn

[B14] 判断值是否在集合内
来源：http://ao.asd995.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jq.shxzukj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lz.yuntaijiaju.cn

JS:   [1, 2, 3].includes(x)
来源：http://so.szxytkj.cn

TS:   [1, 2, 3].includes(x)
来源：http://ap.bookmarksfly.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gx.hnjuh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dq.nszjky.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bo.szxytkj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mw.521024.cn

[B15] 布尔运算与取反
来源：http://ig.nicolike.cn

Py:   a and b or not c
来源：http://mi.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://gq.nszjky.cn

JS:   a && b || !c
来源：http://yx.colortex.cn

TS:   a && b || !c
来源：http://cn.szxytkj.cn

Java: a && b || !c
来源：http://go.szxytkj.cn

Go:   a && b || !c
来源：http://ft.jctech888.com.cn

Ruby: a && b || !c
来源：http://jr.gzmigu.cn

C#:   a && b || !c
来源：http://rq.nicolike.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fu.shxzskj.cn

Py:   if not data: return
来源：http://nn.huixiangedu.cn

PHP:  if (!$data) { return; }
来源：http://mt.nszjky.cn

JS:   if (!data) return;
来源：http://yp.jctech888.com.cn

TS:   if (!data) return;
来源：http://mb.yuexingan06.cn

Java: if (data == null) return;
来源：http://sl.panjiajie.cn

Go:   if data == nil { return }
来源：http://hc.jctech888.com.cn

Ruby: return if data.nil?
来源：http://tb.hnjuh.cn

C#:   if (data == null) return;
来源：http://iv.newstarts.cn

================================================================================
来源：http://gu.panjiajie.cn

C. 函数与作用域
来源：http://cq.muxihuayi.cn

================================================================================
来源：http://qy.hahajie.cn

[C01] 定义函数
来源：http://fo.huixiangedu.cn

Py:   def add(a, b): return a + b
来源：http://pq.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fh.colortex.cn

JS:   function add(a, b) { return a + b; }
来源：http://pq.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oh.szsharing.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gr.nicolike.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wz.huixinmuqiang.cn

Ruby: def add(a, b); a + b; end
来源：http://oj.yuntaijiaju.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lc.gzmigu.cn

[C02] 默认参数
来源：http://tz.huixiangedu.cn

Py:   def greet(name="World"): return name
来源：http://gc.521024.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gc.huanxung.cn

JS:   function greet(name = "World") { return name; }
来源：http://fe.huixiangedu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qa.szxytkj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://az.asd995.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tc.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://wz.bjjhwx.cn

C#:   string Greet(string name = "World") => name;
来源：http://rz.jianghongdianzi.cn

[C03] 可变参数
来源：http://ys.9csxet.cn

Py:   def total(*args): return sum(args)
来源：http://ds.shxzskj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vg.haigaiapp.cn


<!-- 参考信息 -->