代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jv.yuntaijiaju.cn

Ruby: "Hello, #{name}!"
来源：http://ld.haigaiapp.cn

C#:   $"Hello, {name}!"
来源：http://we.szxytkj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ly.huanxung.cn

Py:   "第一行\n第二行"
来源：http://wb.shxzskj.cn

PHP:  "第一行\n第二行"
来源：http://wz.521024.cn

JS:   "第一行\n第二行"
来源：http://bl.asd995.cn

TS:   "第一行\n第二行"
来源：http://fm.chemitech.net.cn

Java: "第一行\n第二行"
来源：http://zt.gzmigu.cn

Go:   "第一行\n第二行"
来源：http://me.nicolike.cn

Ruby: "第一行\n第二行"
来源：http://qe.nszjky.cn

C#:   "第一行\n第二行"
来源：http://pu.huixinmuqiang.cn

[A14] 注释写法
来源：http://do.lnxyls.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ii.jctech888.com.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://yk.asd995.cn

JS:   // 单行；/* 多行 */
来源：http://xh.shtwfgs.cn

TS:   // 单行；/* 多行 */
来源：http://tl.shxzskj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://oo.jianghongdianzi.cn

Go:   // 单行；/* 多行 */
来源：http://pz.nszjky.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vx.huixiangedu.cn

C#:   // 单行；/* 多行 */
来源：http://gl.shxzukj.cn

[A15] 空值判断与默认值
来源：http://mh.colortex.cn

Py:   value = data or "默认值"
来源：http://nl.yuexingan06.cn

PHP:  $value = $data ?? "默认值";
来源：http://dx.szxytkj.cn

JS:   const value = data ?? "默认值";
来源：http://ce.lnxyls.cn

TS:   const value = data ?? "默认值";
来源：http://bs.szxytkj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://iz.521024.cn

Go:   if data == "" { data = "默认值" }
来源：http://dj.shtwfgs.cn

Ruby: value = data || "默认值"
来源：http://cw.colortex.cn

C#:   var value = data ?? "默认值";
来源：http://au.bookmarksfly.cn

[A16] 真假值判断规则
来源：http://sq.yuntaijiaju.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gn.szsharing.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nx.huanxung.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tb.huixiangedu.cn

TS:   if (!x) {}
来源：http://ka.bjjhwx.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cv.bjjhwx.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yu.nicolike.cn

Ruby: unless x            # nil 与 false 为假
来源：http://pb.colortex.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tz.huanxung.cn

[A17] 位运算
来源：http://bc.wgjwhj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rl.yuntaijiaju.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cx.521024.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rh.shxzukj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cx.huixiangedu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://it.nszjky.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gh.szsharing.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zv.huixiangedu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xh.szsharing.cn

[A18] 字符与 ASCII 码互转
来源：http://cu.521024.cn

Py:   ord("A"); chr(65)
来源：http://fz.huanxung.cn

PHP:  ord("A"); chr(65)
来源：http://ft.szsharing.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ji.colortex.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mq.hnjuh.cn

Java: (int) 'A'; (char) 65
来源：http://bo.shxzukj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wp.jianghongdianzi.cn

Ruby: "A".ord; 65.chr
来源：http://xl.bookmarksfly.cn

C#:   (int)'A'; (char)65
来源：http://xo.yuexingan06.cn

[A19] 交换两个变量
来源：http://ri.gzmigu.cn

Py:   a, b = b, a
来源：http://wx.gzmigu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://iu.521024.cn

JS:   [a, b] = [b, a];
来源：http://ko.colortex.cn

TS:   [a, b] = [b, a];
来源：http://ar.huanxung.cn

Java: int t = a; a = b; b = t;
来源：http://az.nicolike.cn

Go:   a, b = b, a
来源：http://il.shxzukj.cn

Ruby: a, b = b, a
来源：http://ty.shxzskj.cn

C#:   (a, b) = (b, a);
来源：http://bw.wgjwhj.cn

[A20] 读取标准输入
来源：http://bh.lnxyls.cn

Py:   name = input("请输入：")
来源：http://mn.szxytkj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://tb.muxihuayi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ql.yuexingan06.cn

TS:   // Node.js：readline 模块
来源：http://vb.szxytkj.cn

Java: new Scanner(System.in).nextLine()
来源：http://jd.szsharing.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qj.lnxyls.cn

Ruby: gets.chomp
来源：http://vp.jianghongdianzi.cn

C#:   Console.ReadLine();
来源：http://gy.chemitech.net.cn

[A21] 保留指定小数位输出
来源：http://xn.huixiangedu.cn

Py:   f"{3.14159:.2f}"
来源：http://wd.521024.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://le.newstarts.cn

JS:   (3.14159).toFixed(2)
来源：http://xw.hahajie.cn

TS:   (3.14159).toFixed(2)
来源：http://dc.newstarts.cn

Java: String.format("%.2f", 3.14159)
来源：http://fv.gzmigu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://af.muxihuayi.cn

Ruby: format("%.2f", 3.14159)
来源：http://wn.asd995.cn

C#:   3.14159.ToString("F2")
来源：http://sw.haigaiapp.cn

[A22] 获取字符串长度
来源：http://qi.bjjhwx.cn

Py:   len(s)
来源：http://qg.yuexingan06.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tu.shtwfgs.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mc.shtwfgs.cn

TS:   s.length
来源：http://tr.jianghongdianzi.cn

Java: s.length()
来源：http://ku.gzmigu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ma.colortex.cn

Ruby: s.length
来源：http://qx.wgjwhj.cn

C#:   s.Length
来源：http://pt.huanxung.cn

[A23] 大小写转换
来源：http://ax.bjjhwx.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ea.nicolike.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zw.huixinmuqiang.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://so.jianghongdianzi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nm.chemitech.net.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qk.huanxung.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bv.szsharing.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dj.nszjky.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cd.hnjuh.cn

[A24] 去除首尾空白
来源：http://ay.szsharing.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gw.bjjhwx.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://to.nszjky.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ei.newstarts.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ad.haigaiapp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ao.newstarts.cn

Go:   strings.TrimSpace(s)
来源：http://lk.jctech888.com.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bf.muxihuayi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gt.huixiangedu.cn

[A25] 字符串比较
来源：http://jx.szxytkj.cn

Py:   s1 == s2; s1 != s2
来源：http://xp.panjiajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ho.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ry.panjiajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ol.gzmigu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ff.wgjwhj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dv.szxytkj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pw.jianghongdianzi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uh.szxytkj.cn

[A26] 类型转换总览
来源：http://oc.colortex.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ud.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sp.nicolike.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nk.hnjuh.cn

TS:   Number() String() Boolean() x as number
来源：http://fl.lnxyls.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wc.yuntaijiaju.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ce.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://at.colortex.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dw.wgjwhj.cn

================================================================================
来源：http://rs.gzmigu.cn

B. 流程控制
来源：http://xo.asd995.cn

================================================================================
来源：http://th.shxzukj.cn

[B01] 条件判断 if / else
来源：http://zo.yuexingan06.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fn.panjiajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lq.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vc.9csxet.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rs.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://kh.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yn.9csxet.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yz.szsharing.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fs.szsharing.cn

[B02] 多分支 else if / elif
来源：http://fu.huixinmuqiang.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wp.jctech888.com.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gs.hnjuh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://we.haigaiapp.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jo.9csxet.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bm.wgjwhj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vp.hahajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zf.yuntaijiaju.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hl.shtwfgs.cn

[B03] switch / match / case
来源：http://ly.nicolike.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fe.huixiangedu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ic.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dc.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fi.lnxyls.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lt.wgjwhj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ba.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rw.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ae.colortex.cn

[B04] for 计数循环
来源：http://cq.shxzukj.cn

Py:   for i in range(10): print(i)
来源：http://kq.newstarts.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nh.bjjhwx.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vu.huixinmuqiang.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://st.haigaiapp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jp.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uc.haigaiapp.cn

Ruby: 10.times { |i| puts i }
来源：http://kb.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hn.muxihuayi.cn

[B05] 遍历数组 / 列表
来源：http://el.gzmigu.cn

Py:   for item in arr: print(item)
来源：http://wq.huixinmuqiang.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vo.newstarts.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://cj.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qn.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://uh.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yj.huanxung.cn

Ruby: arr.each { |item| puts item }
来源：http://is.szxytkj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xc.nszjky.cn

[B06] 遍历字典 / 对象
来源：http://ij.szxytkj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ot.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://je.shxzukj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://et.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mp.521024.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jq.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mm.bjjhwx.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ut.521024.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ml.shtwfgs.cn

[B07] while 循环
来源：http://jh.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://df.muxihuayi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mg.shtwfgs.cn

JS:   while (i < 10) { i++; }
来源：http://ew.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://sa.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://ey.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jr.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://hf.haigaiapp.cn

C#:   while (i < 10) { i++; }
来源：http://ki.haigaiapp.cn

[B08] do-while（至少执行一次）
来源：http://wk.haigaiapp.cn

Py:   # 无 do-while：用 while True + break
来源：http://tb.jctech888.com.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dh.huixinmuqiang.cn

JS:   do { i++; } while (i < 10);
来源：http://te.yuntaijiaju.cn

TS:   do { i++; } while (i < 10);
来源：http://oo.huixinmuqiang.cn

Java: do { i++; } while (i < 10);
来源：http://qb.hahajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://uo.yuexingan06.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tb.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://jk.shxzukj.cn

[B09] break 与 continue
来源：http://yw.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yj.szsharing.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nw.huixiangedu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jx.chemitech.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mq.yuexingan06.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vc.9csxet.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://it.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vg.szxytkj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jm.asd995.cn

[B10] 遍历同时拿索引
来源：http://iw.nszjky.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rq.9csxet.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://eu.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zx.shxzskj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ud.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ld.colortex.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jv.gzmigu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://su.panjiajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xj.muxihuayi.cn

[B11] 生成数字序列 / 区间
来源：http://fc.wgjwhj.cn

Py:   list(range(0, 10, 2))
来源：http://ib.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://lu.wgjwhj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://le.hahajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mh.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yv.shtwfgs.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bl.bjjhwx.cn

Ruby: (0...10).step(2).to_a
来源：http://na.jianghongdianzi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tn.gzmigu.cn

[B12] 跳出多层循环
来源：http://xf.chemitech.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ro.bjjhwx.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fy.bookmarksfly.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xh.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zw.colortex.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pm.lnxyls.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ey.bookmarksfly.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mr.chemitech.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gs.shxzskj.cn

[B13] 判断是否为数字
来源：http://lo.szsharing.cn

Py:   isinstance(x, (int, float))
来源：http://ne.bookmarksfly.cn

PHP:  is_numeric($x)
来源：http://nf.colortex.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://op.bookmarksfly.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xh.haigaiapp.cn

Java: x instanceof Number
来源：http://sh.gzmigu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ka.9csxet.cn

Ruby: x.is_a?(Numeric)
来源：http://ph.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://ca.lnxyls.cn

[B14] 判断值是否在集合内
来源：http://rv.shxzukj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://be.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://br.hnjuh.cn

JS:   [1, 2, 3].includes(x)
来源：http://hv.yuntaijiaju.cn

TS:   [1, 2, 3].includes(x)
来源：http://ka.jianghongdianzi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://md.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dg.lnxyls.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ts.bookmarksfly.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hv.newstarts.cn

[B15] 布尔运算与取反
来源：http://fa.bookmarksfly.cn

Py:   a and b or not c
来源：http://xi.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://we.lnxyls.cn

JS:   a && b || !c
来源：http://sl.asd995.cn

TS:   a && b || !c
来源：http://pq.jianghongdianzi.cn

Java: a && b || !c
来源：http://ja.huixiangedu.cn

Go:   a && b || !c
来源：http://ly.haigaiapp.cn

Ruby: a && b || !c
来源：http://ig.chemitech.net.cn

C#:   a && b || !c
来源：http://km.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zk.panjiajie.cn

Py:   if not data: return
来源：http://uo.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://dn.huixinmuqiang.cn

JS:   if (!data) return;
来源：http://dg.shxzukj.cn

TS:   if (!data) return;
来源：http://wb.jctech888.com.cn

Java: if (data == null) return;
来源：http://nj.asd995.cn

Go:   if data == nil { return }
来源：http://vu.shxzskj.cn

Ruby: return if data.nil?
来源：http://yg.newstarts.cn

C#:   if (data == null) return;
来源：http://yl.huixiangedu.cn

================================================================================
来源：http://pm.wgjwhj.cn

C. 函数与作用域
来源：http://tg.huixiangedu.cn

================================================================================
来源：http://xd.muxihuayi.cn

[C01] 定义函数
来源：http://bi.jianghongdianzi.cn

Py:   def add(a, b): return a + b
来源：http://aj.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lr.wgjwhj.cn

JS:   function add(a, b) { return a + b; }
来源：http://ue.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sn.shxzskj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://oe.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ha.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://rl.huixinmuqiang.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gv.9csxet.cn

[C02] 默认参数
来源：http://ui.shtwfgs.cn

Py:   def greet(name="World"): return name
来源：http://wv.wgjwhj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cj.bookmarksfly.cn

JS:   function greet(name = "World") { return name; }
来源：http://ne.shxzukj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ot.yuexingan06.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://et.colortex.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qi.wgjwhj.cn

Ruby: def greet(name = "World") = name
来源：http://bn.yuexingan06.cn

C#:   string Greet(string name = "World") => name;
来源：http://oe.hahajie.cn

[C03] 可变参数
来源：http://pd.muxihuayi.cn

Py:   def total(*args): return sum(args)
来源：http://cu.bookmarksfly.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ii.newstarts.cn


<!-- 参考信息 -->