代发 wailian999

Py:   "第一行\n第二行"
来源：http://tf.lnxyls.cn

PHP:  "第一行\n第二行"
来源：http://am.lnxyls.cn

JS:   "第一行\n第二行"
来源：http://ej.hahajie.cn

TS:   "第一行\n第二行"
来源：http://tu.huixiangedu.cn

Java: "第一行\n第二行"
来源：http://jr.colortex.cn

Go:   "第一行\n第二行"
来源：http://vl.jctech888.com.cn

Ruby: "第一行\n第二行"
来源：http://ok.chemitech.net.cn

C#:   "第一行\n第二行"
来源：http://bi.yuntaijiaju.cn

[A14] 注释写法
来源：http://lv.haigaiapp.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gp.jianghongdianzi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ry.asd995.cn

JS:   // 单行；/* 多行 */
来源：http://mv.jianghongdianzi.cn

TS:   // 单行；/* 多行 */
来源：http://yg.yuexingan06.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pn.shtwfgs.cn

Go:   // 单行；/* 多行 */
来源：http://he.lnxyls.cn

Ruby: # 单行；=begin 多行 =end
来源：http://sf.jianghongdianzi.cn

C#:   // 单行；/* 多行 */
来源：http://as.colortex.cn

[A15] 空值判断与默认值
来源：http://dm.bjjhwx.cn

Py:   value = data or "默认值"
来源：http://pl.chemitech.net.cn

PHP:  $value = $data ?? "默认值";
来源：http://tp.9csxet.cn

JS:   const value = data ?? "默认值";
来源：http://ve.szxytkj.cn

TS:   const value = data ?? "默认值";
来源：http://kt.bookmarksfly.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://lt.shtwfgs.cn

Go:   if data == "" { data = "默认值" }
来源：http://aj.huanxung.cn

Ruby: value = data || "默认值"
来源：http://mt.yuexingan06.cn

C#:   var value = data ?? "默认值";
来源：http://qi.yuexingan06.cn

[A16] 真假值判断规则
来源：http://lz.haigaiapp.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ve.shxzukj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vs.shxzskj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cf.huanxung.cn

TS:   if (!x) {}
来源：http://rl.huanxung.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tr.shxzskj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wd.yuexingan06.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zf.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ci.huixiangedu.cn

[A17] 位运算
来源：http://wb.jctech888.com.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hh.wgjwhj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tn.521024.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dc.jianghongdianzi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zp.asd995.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fb.chemitech.net.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xx.shxzukj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oj.hahajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ao.jianghongdianzi.cn

[A18] 字符与 ASCII 码互转
来源：http://uf.panjiajie.cn

Py:   ord("A"); chr(65)
来源：http://fv.szsharing.cn

PHP:  ord("A"); chr(65)
来源：http://mo.panjiajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xg.asd995.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wx.bjjhwx.cn

Java: (int) 'A'; (char) 65
来源：http://mc.521024.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xw.asd995.cn

Ruby: "A".ord; 65.chr
来源：http://or.9csxet.cn

C#:   (int)'A'; (char)65
来源：http://cc.szsharing.cn

[A19] 交换两个变量
来源：http://xo.asd995.cn

Py:   a, b = b, a
来源：http://od.huanxung.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://wy.521024.cn

JS:   [a, b] = [b, a];
来源：http://ap.yuntaijiaju.cn

TS:   [a, b] = [b, a];
来源：http://gi.yuntaijiaju.cn

Java: int t = a; a = b; b = t;
来源：http://fs.lnxyls.cn

Go:   a, b = b, a
来源：http://us.hahajie.cn

Ruby: a, b = b, a
来源：http://xg.nicolike.cn

C#:   (a, b) = (b, a);
来源：http://vh.521024.cn

[A20] 读取标准输入
来源：http://xo.yuexingan06.cn

Py:   name = input("请输入：")
来源：http://hz.huixiangedu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://tr.haigaiapp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hi.panjiajie.cn

TS:   // Node.js：readline 模块
来源：http://ks.jctech888.com.cn

Java: new Scanner(System.in).nextLine()
来源：http://sa.hahajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fj.huixinmuqiang.cn

Ruby: gets.chomp
来源：http://hl.hahajie.cn

C#:   Console.ReadLine();
来源：http://ym.bjjhwx.cn

[A21] 保留指定小数位输出
来源：http://mx.hahajie.cn

Py:   f"{3.14159:.2f}"
来源：http://na.9csxet.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hu.shxzukj.cn

JS:   (3.14159).toFixed(2)
来源：http://je.hahajie.cn

TS:   (3.14159).toFixed(2)
来源：http://tr.lnxyls.cn

Java: String.format("%.2f", 3.14159)
来源：http://jo.jianghongdianzi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://da.bjjhwx.cn

Ruby: format("%.2f", 3.14159)
来源：http://gb.jctech888.com.cn

C#:   3.14159.ToString("F2")
来源：http://qg.muxihuayi.cn

[A22] 获取字符串长度
来源：http://yp.shxzukj.cn

Py:   len(s)
来源：http://dj.nicolike.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bg.nicolike.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hr.colortex.cn

TS:   s.length
来源：http://ln.yuexingan06.cn

Java: s.length()
来源：http://ft.shxzukj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fk.9csxet.cn

Ruby: s.length
来源：http://zh.wgjwhj.cn

C#:   s.Length
来源：http://yt.panjiajie.cn

[A23] 大小写转换
来源：http://wk.huanxung.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://uo.panjiajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ph.lnxyls.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gr.hahajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ms.newstarts.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ao.lnxyls.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zz.yuntaijiaju.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ke.nicolike.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xj.wgjwhj.cn

[A24] 去除首尾空白
来源：http://fe.nszjky.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vy.szxytkj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ho.nicolike.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zc.huixinmuqiang.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vm.bjjhwx.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://px.yuntaijiaju.cn

Go:   strings.TrimSpace(s)
来源：http://ju.asd995.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://oc.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cc.nicolike.cn

[A25] 字符串比较
来源：http://xz.asd995.cn

Py:   s1 == s2; s1 != s2
来源：http://uc.huixinmuqiang.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://th.yuntaijiaju.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ud.huanxung.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://by.521024.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vl.chemitech.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sq.panjiajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hu.jianghongdianzi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uz.9csxet.cn

[A26] 类型转换总览
来源：http://nb.panjiajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tw.huanxung.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vz.szxytkj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vd.colortex.cn

TS:   Number() String() Boolean() x as number
来源：http://hc.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ci.jianghongdianzi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yt.wgjwhj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ig.jctech888.com.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bv.shxzukj.cn

================================================================================
来源：http://jc.muxihuayi.cn

B. 流程控制
来源：http://bt.panjiajie.cn

================================================================================
来源：http://rf.nicolike.cn

[B01] 条件判断 if / else
来源：http://yp.lnxyls.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ag.lnxyls.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sv.bjjhwx.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jk.chemitech.net.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fc.wgjwhj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://au.jctech888.com.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ql.szsharing.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ob.huixinmuqiang.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tv.shxzskj.cn

[B02] 多分支 else if / elif
来源：http://yr.shxzskj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ak.szsharing.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pg.szsharing.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yt.gzmigu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uj.shtwfgs.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ch.jctech888.com.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mv.shtwfgs.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wo.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sn.shtwfgs.cn

[B03] switch / match / case
来源：http://ic.chemitech.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cu.nszjky.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mr.shtwfgs.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hv.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://er.newstarts.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cx.colortex.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xe.yuexingan06.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tt.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://km.shxzskj.cn

[B04] for 计数循环
来源：http://gj.colortex.cn

Py:   for i in range(10): print(i)
来源：http://bf.hnjuh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yl.lnxyls.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jk.szxytkj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pw.huanxung.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nt.jctech888.com.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://eo.huixinmuqiang.cn

Ruby: 10.times { |i| puts i }
来源：http://wr.huixiangedu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kk.jctech888.com.cn

[B05] 遍历数组 / 列表
来源：http://xg.jianghongdianzi.cn

Py:   for item in arr: print(item)
来源：http://xw.jctech888.com.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ti.lnxyls.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zq.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fk.szxytkj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ix.szsharing.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nj.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://ql.nszjky.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lt.huixinmuqiang.cn

[B06] 遍历字典 / 对象
来源：http://am.nszjky.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://na.gzmigu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://we.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://un.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nv.nicolike.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://by.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dm.szxytkj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qr.9csxet.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jc.jctech888.com.cn

[B07] while 循环
来源：http://ov.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://qf.asd995.cn

PHP:  while ($i < 10) { $i++; }
来源：http://js.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://qz.bookmarksfly.cn

TS:   while (i < 10) { i++; }
来源：http://ew.haigaiapp.cn

Java: while (i < 10) { i++; }
来源：http://zd.asd995.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://or.shtwfgs.cn

Ruby: while i < 10; i += 1; end
来源：http://cu.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://xo.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://lf.chemitech.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://te.hnjuh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://li.shxzukj.cn

JS:   do { i++; } while (i < 10);
来源：http://as.wgjwhj.cn

TS:   do { i++; } while (i < 10);
来源：http://no.huixiangedu.cn

Java: do { i++; } while (i < 10);
来源：http://cc.521024.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qb.newstarts.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kj.szxytkj.cn

C#:   do { i++; } while (i < 10);
来源：http://ur.nszjky.cn

[B09] break 与 continue
来源：http://sm.521024.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uc.hnjuh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hk.9csxet.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xy.colortex.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qn.9csxet.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zr.newstarts.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cp.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bq.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lt.shtwfgs.cn

[B10] 遍历同时拿索引
来源：http://bx.9csxet.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xn.nicolike.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gy.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ny.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vj.szxytkj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ik.jctech888.com.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mo.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cl.9csxet.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jp.bjjhwx.cn

[B11] 生成数字序列 / 区间
来源：http://ho.szxytkj.cn

Py:   list(range(0, 10, 2))
来源：http://ac.huixiangedu.cn

PHP:  range(0, 10, 2);
来源：http://pt.yuntaijiaju.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jq.szxytkj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://so.shxzskj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ie.shxzukj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://im.panjiajie.cn

Ruby: (0...10).step(2).to_a
来源：http://rr.jianghongdianzi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dv.muxihuayi.cn

[B12] 跳出多层循环
来源：http://si.bjjhwx.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lt.shxzukj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yr.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dy.haigaiapp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://el.panjiajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ur.panjiajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vn.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lg.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vj.szxytkj.cn

[B13] 判断是否为数字
来源：http://ku.hahajie.cn

Py:   isinstance(x, (int, float))
来源：http://bs.jianghongdianzi.cn

PHP:  is_numeric($x)
来源：http://me.wgjwhj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wq.hnjuh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sw.haigaiapp.cn

Java: x instanceof Number
来源：http://jt.colortex.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ws.9csxet.cn

Ruby: x.is_a?(Numeric)
来源：http://ii.nszjky.cn

C#:   x is int or double or decimal
来源：http://nn.gzmigu.cn

[B14] 判断值是否在集合内
来源：http://qx.wgjwhj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uh.hnjuh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yr.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://np.asd995.cn

TS:   [1, 2, 3].includes(x)
来源：http://in.hahajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ib.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://iq.szxytkj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fn.lnxyls.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wh.jianghongdianzi.cn

[B15] 布尔运算与取反
来源：http://az.muxihuayi.cn

Py:   a and b or not c
来源：http://bm.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://pd.shxzskj.cn

JS:   a && b || !c
来源：http://kh.jianghongdianzi.cn

TS:   a && b || !c
来源：http://ba.jctech888.com.cn

Java: a && b || !c
来源：http://mc.hahajie.cn

Go:   a && b || !c
来源：http://jo.muxihuayi.cn

Ruby: a && b || !c
来源：http://fb.shxzukj.cn

C#:   a && b || !c
来源：http://sv.jctech888.com.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ba.haigaiapp.cn

Py:   if not data: return
来源：http://jd.chemitech.net.cn

PHP:  if (!$data) { return; }
来源：http://sw.panjiajie.cn

JS:   if (!data) return;
来源：http://yn.haigaiapp.cn

TS:   if (!data) return;
来源：http://be.colortex.cn

Java: if (data == null) return;
来源：http://ha.haigaiapp.cn

Go:   if data == nil { return }
来源：http://qx.nicolike.cn

Ruby: return if data.nil?
来源：http://go.jianghongdianzi.cn

C#:   if (data == null) return;
来源：http://yc.yuntaijiaju.cn

================================================================================
来源：http://du.huixinmuqiang.cn

C. 函数与作用域
来源：http://jc.bookmarksfly.cn

================================================================================
来源：http://ra.jctech888.com.cn

[C01] 定义函数
来源：http://qh.panjiajie.cn

Py:   def add(a, b): return a + b
来源：http://ge.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nv.bjjhwx.cn

JS:   function add(a, b) { return a + b; }
来源：http://up.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ww.szxytkj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fw.9csxet.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wk.nszjky.cn

Ruby: def add(a, b); a + b; end
来源：http://ms.haigaiapp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://op.yuntaijiaju.cn

[C02] 默认参数
来源：http://ys.nicolike.cn

Py:   def greet(name="World"): return name
来源：http://dd.hnjuh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://sh.wgjwhj.cn

JS:   function greet(name = "World") { return name; }
来源：http://zg.shxzskj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ul.bookmarksfly.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gq.shxzskj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cw.shxzskj.cn

Ruby: def greet(name = "World") = name
来源：http://sq.hnjuh.cn

C#:   string Greet(string name = "World") => name;
来源：http://gy.hahajie.cn

[C03] 可变参数
来源：http://xf.nicolike.cn

Py:   def total(*args): return sum(args)
来源：http://hc.hahajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sp.yuntaijiaju.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fy.gzmigu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://op.haigaiapp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cv.szsharing.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vr.jianghongdianzi.cn


<!-- 参考信息 -->