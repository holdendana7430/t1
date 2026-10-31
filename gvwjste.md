代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fa.9csxet.cn

Ruby: "Hello, #{name}!"
来源：http://an.hnjuh.cn

C#:   $"Hello, {name}!"
来源：http://lr.chemitech.net.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ve.jctech888.com.cn

Py:   "第一行\n第二行"
来源：http://fb.newstarts.cn

PHP:  "第一行\n第二行"
来源：http://mv.bookmarksfly.cn

JS:   "第一行\n第二行"
来源：http://vj.colortex.cn

TS:   "第一行\n第二行"
来源：http://ck.asd995.cn

Java: "第一行\n第二行"
来源：http://xv.wgjwhj.cn

Go:   "第一行\n第二行"
来源：http://py.panjiajie.cn

Ruby: "第一行\n第二行"
来源：http://ug.hnjuh.cn

C#:   "第一行\n第二行"
来源：http://hn.muxihuayi.cn

[A14] 注释写法
来源：http://fc.haigaiapp.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ij.huixinmuqiang.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://rd.shtwfgs.cn

JS:   // 单行；/* 多行 */
来源：http://pb.nszjky.cn

TS:   // 单行；/* 多行 */
来源：http://sb.huixinmuqiang.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kp.jianghongdianzi.cn

Go:   // 单行；/* 多行 */
来源：http://pr.wgjwhj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://on.panjiajie.cn

C#:   // 单行；/* 多行 */
来源：http://sx.huanxung.cn

[A15] 空值判断与默认值
来源：http://mq.haigaiapp.cn

Py:   value = data or "默认值"
来源：http://da.nicolike.cn

PHP:  $value = $data ?? "默认值";
来源：http://bi.panjiajie.cn

JS:   const value = data ?? "默认值";
来源：http://wn.nicolike.cn

TS:   const value = data ?? "默认值";
来源：http://iv.yuntaijiaju.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://if.gzmigu.cn

Go:   if data == "" { data = "默认值" }
来源：http://ck.bjjhwx.cn

Ruby: value = data || "默认值"
来源：http://tl.shxzukj.cn

C#:   var value = data ?? "默认值";
来源：http://ti.shxzskj.cn

[A16] 真假值判断规则
来源：http://qp.bjjhwx.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ti.newstarts.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://iu.haigaiapp.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ln.9csxet.cn

TS:   if (!x) {}
来源：http://rm.hnjuh.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ul.bjjhwx.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kx.hahajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ax.asd995.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tj.hnjuh.cn

[A17] 位运算
来源：http://fv.huixinmuqiang.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zv.haigaiapp.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qr.bjjhwx.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sl.wgjwhj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://er.9csxet.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wg.521024.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qo.huixinmuqiang.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hj.nicolike.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.shxzukj.cn

[A18] 字符与 ASCII 码互转
来源：http://op.szsharing.cn

Py:   ord("A"); chr(65)
来源：http://hv.huanxung.cn

PHP:  ord("A"); chr(65)
来源：http://ym.shxzskj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zj.chemitech.net.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fu.szxytkj.cn

Java: (int) 'A'; (char) 65
来源：http://jq.szxytkj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jd.asd995.cn

Ruby: "A".ord; 65.chr
来源：http://fg.huixiangedu.cn

C#:   (int)'A'; (char)65
来源：http://nn.panjiajie.cn

[A19] 交换两个变量
来源：http://rr.newstarts.cn

Py:   a, b = b, a
来源：http://dl.shtwfgs.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://mc.shxzskj.cn

JS:   [a, b] = [b, a];
来源：http://qe.nicolike.cn

TS:   [a, b] = [b, a];
来源：http://he.szsharing.cn

Java: int t = a; a = b; b = t;
来源：http://ks.nszjky.cn

Go:   a, b = b, a
来源：http://er.shxzskj.cn

Ruby: a, b = b, a
来源：http://od.jianghongdianzi.cn

C#:   (a, b) = (b, a);
来源：http://xv.asd995.cn

[A20] 读取标准输入
来源：http://ly.muxihuayi.cn

Py:   name = input("请输入：")
来源：http://mj.huixinmuqiang.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ck.gzmigu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pz.huixiangedu.cn

TS:   // Node.js：readline 模块
来源：http://rt.huanxung.cn

Java: new Scanner(System.in).nextLine()
来源：http://no.shxzskj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qb.muxihuayi.cn

Ruby: gets.chomp
来源：http://iw.bjjhwx.cn

C#:   Console.ReadLine();
来源：http://gx.jianghongdianzi.cn

[A21] 保留指定小数位输出
来源：http://yf.huanxung.cn

Py:   f"{3.14159:.2f}"
来源：http://hw.nszjky.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bm.nszjky.cn

JS:   (3.14159).toFixed(2)
来源：http://st.chemitech.net.cn

TS:   (3.14159).toFixed(2)
来源：http://sd.szxytkj.cn

Java: String.format("%.2f", 3.14159)
来源：http://qc.shxzukj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ts.huixinmuqiang.cn

Ruby: format("%.2f", 3.14159)
来源：http://rj.bjjhwx.cn

C#:   3.14159.ToString("F2")
来源：http://wf.9csxet.cn

[A22] 获取字符串长度
来源：http://bw.nicolike.cn

Py:   len(s)
来源：http://ia.huanxung.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kj.newstarts.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rw.nszjky.cn

TS:   s.length
来源：http://yi.wgjwhj.cn

Java: s.length()
来源：http://hz.muxihuayi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://us.panjiajie.cn

Ruby: s.length
来源：http://kn.jianghongdianzi.cn

C#:   s.Length
来源：http://hb.newstarts.cn

[A23] 大小写转换
来源：http://yq.nszjky.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wh.9csxet.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vg.jctech888.com.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kg.bjjhwx.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qr.yuexingan06.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sy.colortex.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mp.huixiangedu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zv.huanxung.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rm.panjiajie.cn

[A24] 去除首尾空白
来源：http://de.colortex.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ep.shtwfgs.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fp.hahajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lh.hnjuh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://en.nicolike.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cu.nicolike.cn

Go:   strings.TrimSpace(s)
来源：http://vh.lnxyls.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://er.wgjwhj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kz.lnxyls.cn

[A25] 字符串比较
来源：http://tx.jctech888.com.cn

Py:   s1 == s2; s1 != s2
来源：http://ms.szxytkj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xg.hahajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vv.chemitech.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yg.hnjuh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rb.huixiangedu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lf.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gn.asd995.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nn.nszjky.cn

[A26] 类型转换总览
来源：http://jq.jianghongdianzi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nk.521024.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mg.huixinmuqiang.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qv.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://rv.szsharing.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://op.panjiajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mr.huanxung.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bd.panjiajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://go.shxzukj.cn

================================================================================
来源：http://am.huanxung.cn

B. 流程控制
来源：http://rt.hnjuh.cn

================================================================================
来源：http://vv.jianghongdianzi.cn

[B01] 条件判断 if / else
来源：http://zh.asd995.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wm.szxytkj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cb.shxzukj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://io.hahajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zv.lnxyls.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://yj.szxytkj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fe.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ur.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nm.hnjuh.cn

[B02] 多分支 else if / elif
来源：http://qh.jianghongdianzi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yj.bookmarksfly.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cr.huixinmuqiang.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zh.shxzukj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ij.9csxet.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zx.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xr.newstarts.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ao.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ij.hnjuh.cn

[B03] switch / match / case
来源：http://db.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xk.hnjuh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kd.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lp.wgjwhj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rz.nicolike.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pi.szxytkj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ic.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fm.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ap.jctech888.com.cn

[B04] for 计数循环
来源：http://tz.hahajie.cn

Py:   for i in range(10): print(i)
来源：http://pj.shxzskj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jh.panjiajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wn.9csxet.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mq.jianghongdianzi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ej.haigaiapp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cu.wgjwhj.cn

Ruby: 10.times { |i| puts i }
来源：http://hq.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://iw.nszjky.cn

[B05] 遍历数组 / 列表
来源：http://qh.lnxyls.cn

Py:   for item in arr: print(item)
来源：http://hi.yuexingan06.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://je.shxzukj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ko.yuntaijiaju.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fy.lnxyls.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ub.gzmigu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yx.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://ow.szsharing.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://op.jctech888.com.cn

[B06] 遍历字典 / 对象
来源：http://jr.gzmigu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zk.nicolike.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ln.szxytkj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qs.nszjky.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aw.jctech888.com.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kq.huixiangedu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nl.jctech888.com.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yp.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pw.jctech888.com.cn

[B07] while 循环
来源：http://de.yuntaijiaju.cn

Py:   while i < 10: i += 1
来源：http://st.jianghongdianzi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lp.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://pk.jctech888.com.cn

TS:   while (i < 10) { i++; }
来源：http://ui.huanxung.cn

Java: while (i < 10) { i++; }
来源：http://mm.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ro.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://xc.haigaiapp.cn

C#:   while (i < 10) { i++; }
来源：http://jp.colortex.cn

[B08] do-while（至少执行一次）
来源：http://zz.nszjky.cn

Py:   # 无 do-while：用 while True + break
来源：http://ry.9csxet.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mc.shxzukj.cn

JS:   do { i++; } while (i < 10);
来源：http://ra.muxihuayi.cn

TS:   do { i++; } while (i < 10);
来源：http://po.nicolike.cn

Java: do { i++; } while (i < 10);
来源：http://yd.bjjhwx.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sh.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://sj.jianghongdianzi.cn

C#:   do { i++; } while (i < 10);
来源：http://ai.jianghongdianzi.cn

[B09] break 与 continue
来源：http://wo.hnjuh.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://or.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://to.shxzskj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kk.nszjky.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uf.bookmarksfly.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xc.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ay.asd995.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kg.huanxung.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hg.521024.cn

[B10] 遍历同时拿索引
来源：http://xl.521024.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vd.nszjky.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ja.nicolike.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cf.gzmigu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://do.huanxung.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yw.bookmarksfly.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qv.szsharing.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qt.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://es.jianghongdianzi.cn

[B11] 生成数字序列 / 区间
来源：http://or.panjiajie.cn

Py:   list(range(0, 10, 2))
来源：http://ey.newstarts.cn

PHP:  range(0, 10, 2);
来源：http://tc.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tm.szsharing.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oa.newstarts.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hy.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://se.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://ms.szsharing.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zf.hnjuh.cn

[B12] 跳出多层循环
来源：http://ol.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jj.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://os.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ok.nicolike.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gg.hnjuh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pa.newstarts.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cu.chemitech.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pm.szsharing.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ao.bjjhwx.cn

[B13] 判断是否为数字
来源：http://xy.bjjhwx.cn

Py:   isinstance(x, (int, float))
来源：http://is.bookmarksfly.cn

PHP:  is_numeric($x)
来源：http://tn.521024.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://md.bookmarksfly.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jd.chemitech.net.cn

Java: x instanceof Number
来源：http://im.huixinmuqiang.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://js.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://nd.nszjky.cn

C#:   x is int or double or decimal
来源：http://bu.newstarts.cn

[B14] 判断值是否在集合内
来源：http://tg.yuexingan06.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bw.nicolike.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xi.yuexingan06.cn

JS:   [1, 2, 3].includes(x)
来源：http://ox.shtwfgs.cn

TS:   [1, 2, 3].includes(x)
来源：http://sy.yuntaijiaju.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://tr.haigaiapp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sg.lnxyls.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lh.nszjky.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yl.9csxet.cn

[B15] 布尔运算与取反
来源：http://sk.muxihuayi.cn

Py:   a and b or not c
来源：http://wh.nicolike.cn

PHP:  $a && $b || !$c
来源：http://gb.haigaiapp.cn

JS:   a && b || !c
来源：http://fw.asd995.cn

TS:   a && b || !c
来源：http://kv.gzmigu.cn

Java: a && b || !c
来源：http://jj.huixinmuqiang.cn

Go:   a && b || !c
来源：http://vq.nszjky.cn

Ruby: a && b || !c
来源：http://hm.panjiajie.cn

C#:   a && b || !c
来源：http://mh.szxytkj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fq.huanxung.cn

Py:   if not data: return
来源：http://ss.bjjhwx.cn

PHP:  if (!$data) { return; }
来源：http://qd.yuexingan06.cn

JS:   if (!data) return;
来源：http://gt.panjiajie.cn

TS:   if (!data) return;
来源：http://rv.huixinmuqiang.cn

Java: if (data == null) return;
来源：http://tu.huixiangedu.cn

Go:   if data == nil { return }
来源：http://ro.haigaiapp.cn

Ruby: return if data.nil?
来源：http://nh.wgjwhj.cn

C#:   if (data == null) return;
来源：http://eq.hnjuh.cn

================================================================================
来源：http://fk.wgjwhj.cn

C. 函数与作用域
来源：http://oi.panjiajie.cn

================================================================================
来源：http://rm.nicolike.cn

[C01] 定义函数
来源：http://vi.hnjuh.cn

Py:   def add(a, b): return a + b
来源：http://aw.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pq.gzmigu.cn

JS:   function add(a, b) { return a + b; }
来源：http://fv.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jz.szsharing.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hw.newstarts.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qm.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://hc.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dw.colortex.cn

[C02] 默认参数
来源：http://sg.bjjhwx.cn

Py:   def greet(name="World"): return name
来源：http://zv.huixiangedu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://co.jctech888.com.cn

JS:   function greet(name = "World") { return name; }
来源：http://mu.haigaiapp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ht.huanxung.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mt.bookmarksfly.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rf.521024.cn

Ruby: def greet(name = "World") = name
来源：http://ux.521024.cn

C#:   string Greet(string name = "World") => name;
来源：http://tw.yuntaijiaju.cn

[C03] 可变参数
来源：http://lk.9csxet.cn

Py:   def total(*args): return sum(args)
来源：http://ht.wgjwhj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lz.jctech888.com.cn


<!-- 参考信息 -->