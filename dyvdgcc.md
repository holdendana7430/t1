代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cd.jctech888.com.cn

Ruby: "Hello, #{name}!"
来源：http://mn.szsharing.cn

C#:   $"Hello, {name}!"
来源：http://wr.hnjuh.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://lj.yuntaijiaju.cn

Py:   "第一行\n第二行"
来源：http://ka.muxihuayi.cn

PHP:  "第一行\n第二行"
来源：http://ms.521024.cn

JS:   "第一行\n第二行"
来源：http://ib.newstarts.cn

TS:   "第一行\n第二行"
来源：http://wi.muxihuayi.cn

Java: "第一行\n第二行"
来源：http://lf.shxzukj.cn

Go:   "第一行\n第二行"
来源：http://yb.lnxyls.cn

Ruby: "第一行\n第二行"
来源：http://nd.shtwfgs.cn

C#:   "第一行\n第二行"
来源：http://gk.jctech888.com.cn

[A14] 注释写法
来源：http://hy.panjiajie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://tf.jianghongdianzi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ut.gzmigu.cn

JS:   // 单行；/* 多行 */
来源：http://qp.bookmarksfly.cn

TS:   // 单行；/* 多行 */
来源：http://nw.huixinmuqiang.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kl.gzmigu.cn

Go:   // 单行；/* 多行 */
来源：http://su.gzmigu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://il.shtwfgs.cn

C#:   // 单行；/* 多行 */
来源：http://lk.hnjuh.cn

[A15] 空值判断与默认值
来源：http://hy.bookmarksfly.cn

Py:   value = data or "默认值"
来源：http://df.nszjky.cn

PHP:  $value = $data ?? "默认值";
来源：http://uh.gzmigu.cn

JS:   const value = data ?? "默认值";
来源：http://rg.huixinmuqiang.cn

TS:   const value = data ?? "默认值";
来源：http://kg.wgjwhj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yz.shxzskj.cn

Go:   if data == "" { data = "默认值" }
来源：http://hy.hnjuh.cn

Ruby: value = data || "默认值"
来源：http://vc.yuntaijiaju.cn

C#:   var value = data ?? "默认值";
来源：http://rd.nicolike.cn

[A16] 真假值判断规则
来源：http://yj.nicolike.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rp.yuexingan06.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bu.yuntaijiaju.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ej.huixinmuqiang.cn

TS:   if (!x) {}
来源：http://aw.shtwfgs.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wm.gzmigu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://es.yuexingan06.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xg.huanxung.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xz.jianghongdianzi.cn

[A17] 位运算
来源：http://vd.newstarts.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ji.wgjwhj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hk.szxytkj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qr.yuexingan06.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zm.szxytkj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qu.shxzskj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cz.lnxyls.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nf.nicolike.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ws.chemitech.net.cn

[A18] 字符与 ASCII 码互转
来源：http://sw.shxzukj.cn

Py:   ord("A"); chr(65)
来源：http://nv.521024.cn

PHP:  ord("A"); chr(65)
来源：http://vd.nszjky.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jj.szxytkj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lk.lnxyls.cn

Java: (int) 'A'; (char) 65
来源：http://am.huixinmuqiang.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qz.bjjhwx.cn

Ruby: "A".ord; 65.chr
来源：http://or.huanxung.cn

C#:   (int)'A'; (char)65
来源：http://si.shtwfgs.cn

[A19] 交换两个变量
来源：http://sa.szxytkj.cn

Py:   a, b = b, a
来源：http://js.521024.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qn.colortex.cn

JS:   [a, b] = [b, a];
来源：http://qo.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://ag.hnjuh.cn

Java: int t = a; a = b; b = t;
来源：http://ym.lnxyls.cn

Go:   a, b = b, a
来源：http://qf.521024.cn

Ruby: a, b = b, a
来源：http://jc.newstarts.cn

C#:   (a, b) = (b, a);
来源：http://dw.hahajie.cn

[A20] 读取标准输入
来源：http://dx.szxytkj.cn

Py:   name = input("请输入：")
来源：http://rf.haigaiapp.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://uo.wgjwhj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gb.wgjwhj.cn

TS:   // Node.js：readline 模块
来源：http://rp.nszjky.cn

Java: new Scanner(System.in).nextLine()
来源：http://ce.jctech888.com.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gj.muxihuayi.cn

Ruby: gets.chomp
来源：http://cv.bookmarksfly.cn

C#:   Console.ReadLine();
来源：http://sg.huanxung.cn

[A21] 保留指定小数位输出
来源：http://hd.szxytkj.cn

Py:   f"{3.14159:.2f}"
来源：http://tm.panjiajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dt.nszjky.cn

JS:   (3.14159).toFixed(2)
来源：http://cv.haigaiapp.cn

TS:   (3.14159).toFixed(2)
来源：http://ik.jctech888.com.cn

Java: String.format("%.2f", 3.14159)
来源：http://pi.colortex.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fo.huixinmuqiang.cn

Ruby: format("%.2f", 3.14159)
来源：http://xv.gzmigu.cn

C#:   3.14159.ToString("F2")
来源：http://aw.colortex.cn

[A22] 获取字符串长度
来源：http://nt.hnjuh.cn

Py:   len(s)
来源：http://rl.hahajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mv.hnjuh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ou.yuexingan06.cn

TS:   s.length
来源：http://ux.panjiajie.cn

Java: s.length()
来源：http://hz.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fq.colortex.cn

Ruby: s.length
来源：http://na.wgjwhj.cn

C#:   s.Length
来源：http://mi.shxzukj.cn

[A23] 大小写转换
来源：http://en.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://bx.lnxyls.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://et.newstarts.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pl.shtwfgs.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://id.shxzukj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://iq.yuntaijiaju.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://oy.521024.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ol.bjjhwx.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zj.szxytkj.cn

[A24] 去除首尾空白
来源：http://uk.hnjuh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kp.shxzukj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ql.shxzukj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yb.huixiangedu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yu.nicolike.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gx.yuntaijiaju.cn

Go:   strings.TrimSpace(s)
来源：http://hy.shxzukj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hk.yuntaijiaju.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://du.haigaiapp.cn

[A25] 字符串比较
来源：http://kd.asd995.cn

Py:   s1 == s2; s1 != s2
来源：http://vy.9csxet.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lr.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xv.newstarts.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ue.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kh.huixiangedu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nb.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://sl.bookmarksfly.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hg.gzmigu.cn

[A26] 类型转换总览
来源：http://or.9csxet.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fh.bjjhwx.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jr.shxzukj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uz.haigaiapp.cn

TS:   Number() String() Boolean() x as number
来源：http://sy.jctech888.com.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yf.wgjwhj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://up.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cm.521024.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kx.colortex.cn

================================================================================
来源：http://nx.szxytkj.cn

B. 流程控制
来源：http://mv.9csxet.cn

================================================================================
来源：http://om.jianghongdianzi.cn

[B01] 条件判断 if / else
来源：http://rg.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ts.521024.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ig.wgjwhj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pz.asd995.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ph.colortex.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://to.colortex.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dx.szxytkj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bw.521024.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cj.bookmarksfly.cn

[B02] 多分支 else if / elif
来源：http://ax.panjiajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ds.hnjuh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://eh.shxzukj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://px.hnjuh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fl.hahajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kl.colortex.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gs.bookmarksfly.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://et.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lw.newstarts.cn

[B03] switch / match / case
来源：http://ox.panjiajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xq.521024.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ah.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pu.bjjhwx.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kz.9csxet.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://oc.szsharing.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nd.asd995.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ux.szsharing.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ts.hnjuh.cn

[B04] for 计数循环
来源：http://kb.lnxyls.cn

Py:   for i in range(10): print(i)
来源：http://ts.yuntaijiaju.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://li.bjjhwx.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yv.huanxung.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ui.lnxyls.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wf.newstarts.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ge.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://lp.shtwfgs.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pa.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://xx.wgjwhj.cn

Py:   for item in arr: print(item)
来源：http://vf.chemitech.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sk.muxihuayi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://th.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kc.lnxyls.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://or.muxihuayi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mi.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://pv.lnxyls.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ps.huanxung.cn

[B06] 遍历字典 / 对象
来源：http://dx.9csxet.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bo.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qc.chemitech.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ub.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ye.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://or.hahajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ux.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mw.huixinmuqiang.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dr.jctech888.com.cn

[B07] while 循环
来源：http://aj.colortex.cn

Py:   while i < 10: i += 1
来源：http://rs.shtwfgs.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lz.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://le.wgjwhj.cn

TS:   while (i < 10) { i++; }
来源：http://iw.colortex.cn

Java: while (i < 10) { i++; }
来源：http://do.newstarts.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kb.shxzskj.cn

Ruby: while i < 10; i += 1; end
来源：http://rr.haigaiapp.cn

C#:   while (i < 10) { i++; }
来源：http://db.colortex.cn

[B08] do-while（至少执行一次）
来源：http://yy.nszjky.cn

Py:   # 无 do-while：用 while True + break
来源：http://to.huixiangedu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qr.chemitech.net.cn

JS:   do { i++; } while (i < 10);
来源：http://ja.nicolike.cn

TS:   do { i++; } while (i < 10);
来源：http://zw.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://tr.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ue.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ne.yuntaijiaju.cn

C#:   do { i++; } while (i < 10);
来源：http://ev.chemitech.net.cn

[B09] break 与 continue
来源：http://yk.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ao.jctech888.com.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pr.bookmarksfly.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zh.huixinmuqiang.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jx.9csxet.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cn.panjiajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ly.hahajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sf.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://au.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://tk.shxzskj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vp.huixiangedu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cf.yuexingan06.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ba.huixiangedu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pi.9csxet.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ex.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ai.bjjhwx.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uj.jctech888.com.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bj.hnjuh.cn

[B11] 生成数字序列 / 区间
来源：http://xr.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://ma.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://sm.asd995.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dq.shxzskj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gp.wgjwhj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://md.yuntaijiaju.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xi.panjiajie.cn

Ruby: (0...10).step(2).to_a
来源：http://qr.jianghongdianzi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://eb.nszjky.cn

[B12] 跳出多层循环
来源：http://bs.jctech888.com.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qr.chemitech.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nh.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ou.panjiajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pc.shxzskj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://iv.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pt.yuntaijiaju.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://os.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ta.muxihuayi.cn

[B13] 判断是否为数字
来源：http://hj.521024.cn

Py:   isinstance(x, (int, float))
来源：http://ed.huanxung.cn

PHP:  is_numeric($x)
来源：http://xf.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qo.yuntaijiaju.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ir.nicolike.cn

Java: x instanceof Number
来源：http://yi.gzmigu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yg.shxzukj.cn

Ruby: x.is_a?(Numeric)
来源：http://ug.colortex.cn

C#:   x is int or double or decimal
来源：http://mp.bjjhwx.cn

[B14] 判断值是否在集合内
来源：http://fy.wgjwhj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yz.wgjwhj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yp.shtwfgs.cn

JS:   [1, 2, 3].includes(x)
来源：http://ut.huanxung.cn

TS:   [1, 2, 3].includes(x)
来源：http://mx.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kd.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ob.gzmigu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jh.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qn.lnxyls.cn

[B15] 布尔运算与取反
来源：http://oa.gzmigu.cn

Py:   a and b or not c
来源：http://jc.newstarts.cn

PHP:  $a && $b || !$c
来源：http://cc.asd995.cn

JS:   a && b || !c
来源：http://gi.jianghongdianzi.cn

TS:   a && b || !c
来源：http://ls.9csxet.cn

Java: a && b || !c
来源：http://tw.huanxung.cn

Go:   a && b || !c
来源：http://cv.haigaiapp.cn

Ruby: a && b || !c
来源：http://ug.wgjwhj.cn

C#:   a && b || !c
来源：http://vu.jctech888.com.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xx.lnxyls.cn

Py:   if not data: return
来源：http://eo.muxihuayi.cn

PHP:  if (!$data) { return; }
来源：http://wq.jianghongdianzi.cn

JS:   if (!data) return;
来源：http://xj.newstarts.cn

TS:   if (!data) return;
来源：http://qw.huixiangedu.cn

Java: if (data == null) return;
来源：http://tu.chemitech.net.cn

Go:   if data == nil { return }
来源：http://lf.shtwfgs.cn

Ruby: return if data.nil?
来源：http://aj.bjjhwx.cn

C#:   if (data == null) return;
来源：http://rn.bookmarksfly.cn

================================================================================
来源：http://ko.shxzskj.cn

C. 函数与作用域
来源：http://ka.shtwfgs.cn

================================================================================
来源：http://xg.colortex.cn

[C01] 定义函数
来源：http://xa.muxihuayi.cn

Py:   def add(a, b): return a + b
来源：http://ah.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tt.yuntaijiaju.cn

JS:   function add(a, b) { return a + b; }
来源：http://bi.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dp.bjjhwx.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sc.asd995.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ib.szxytkj.cn

Ruby: def add(a, b); a + b; end
来源：http://bj.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kz.jianghongdianzi.cn

[C02] 默认参数
来源：http://tu.panjiajie.cn

Py:   def greet(name="World"): return name
来源：http://dp.shxzukj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://en.gzmigu.cn

JS:   function greet(name = "World") { return name; }
来源：http://fn.9csxet.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wf.shtwfgs.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ql.chemitech.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gu.chemitech.net.cn

Ruby: def greet(name = "World") = name
来源：http://nv.lnxyls.cn

C#:   string Greet(string name = "World") => name;
来源：http://cj.szsharing.cn

[C03] 可变参数
来源：http://hi.yuntaijiaju.cn

Py:   def total(*args): return sum(args)
来源：http://em.bjjhwx.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oi.szsharing.cn


<!-- 参考信息 -->