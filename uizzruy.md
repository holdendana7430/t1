代发 wailian999

Java: "第一行\n第二行"
来源：http://gf.lnxyls.cn

Go:   "第一行\n第二行"
来源：http://xm.jianghongdianzi.cn

Ruby: "第一行\n第二行"
来源：http://pe.huixiangedu.cn

C#:   "第一行\n第二行"
来源：http://bx.lnxyls.cn

[A14] 注释写法
来源：http://jl.huixinmuqiang.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://qh.9csxet.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xo.9csxet.cn

JS:   // 单行；/* 多行 */
来源：http://ly.jianghongdianzi.cn

TS:   // 单行；/* 多行 */
来源：http://yk.9csxet.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yd.nicolike.cn

Go:   // 单行；/* 多行 */
来源：http://ry.nicolike.cn

Ruby: # 单行；=begin 多行 =end
来源：http://nq.hahajie.cn

C#:   // 单行；/* 多行 */
来源：http://yh.bookmarksfly.cn

[A15] 空值判断与默认值
来源：http://li.shxzskj.cn

Py:   value = data or "默认值"
来源：http://jw.521024.cn

PHP:  $value = $data ?? "默认值";
来源：http://nh.bookmarksfly.cn

JS:   const value = data ?? "默认值";
来源：http://kd.hahajie.cn

TS:   const value = data ?? "默认值";
来源：http://bz.shxzskj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ha.bookmarksfly.cn

Go:   if data == "" { data = "默认值" }
来源：http://ik.hnjuh.cn

Ruby: value = data || "默认值"
来源：http://ui.shtwfgs.cn

C#:   var value = data ?? "默认值";
来源：http://dr.hahajie.cn

[A16] 真假值判断规则
来源：http://ps.chemitech.net.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xj.jianghongdianzi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bd.shxzskj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ex.521024.cn

TS:   if (!x) {}
来源：http://kt.nszjky.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pr.gzmigu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ba.huixinmuqiang.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lt.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wx.szsharing.cn

[A17] 位运算
来源：http://md.jctech888.com.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gh.bjjhwx.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://on.nszjky.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qj.panjiajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dp.huixinmuqiang.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ke.hahajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ji.colortex.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wh.asd995.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xr.nszjky.cn

[A18] 字符与 ASCII 码互转
来源：http://pu.muxihuayi.cn

Py:   ord("A"); chr(65)
来源：http://qp.lnxyls.cn

PHP:  ord("A"); chr(65)
来源：http://sy.huixiangedu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fm.wgjwhj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wa.newstarts.cn

Java: (int) 'A'; (char) 65
来源：http://bn.shxzskj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gh.shxzskj.cn

Ruby: "A".ord; 65.chr
来源：http://zi.nicolike.cn

C#:   (int)'A'; (char)65
来源：http://wi.nicolike.cn

[A19] 交换两个变量
来源：http://pc.newstarts.cn

Py:   a, b = b, a
来源：http://lj.huixinmuqiang.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fe.nszjky.cn

JS:   [a, b] = [b, a];
来源：http://nx.huanxung.cn

TS:   [a, b] = [b, a];
来源：http://dm.haigaiapp.cn

Java: int t = a; a = b; b = t;
来源：http://ht.shxzukj.cn

Go:   a, b = b, a
来源：http://gx.wgjwhj.cn

Ruby: a, b = b, a
来源：http://lx.szxytkj.cn

C#:   (a, b) = (b, a);
来源：http://yp.jctech888.com.cn

[A20] 读取标准输入
来源：http://ek.huanxung.cn

Py:   name = input("请输入：")
来源：http://qq.newstarts.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ts.bjjhwx.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cd.521024.cn

TS:   // Node.js：readline 模块
来源：http://kk.haigaiapp.cn

Java: new Scanner(System.in).nextLine()
来源：http://pa.yuntaijiaju.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gp.9csxet.cn

Ruby: gets.chomp
来源：http://oa.gzmigu.cn

C#:   Console.ReadLine();
来源：http://cc.chemitech.net.cn

[A21] 保留指定小数位输出
来源：http://zu.shtwfgs.cn

Py:   f"{3.14159:.2f}"
来源：http://qj.huanxung.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qj.521024.cn

JS:   (3.14159).toFixed(2)
来源：http://gh.gzmigu.cn

TS:   (3.14159).toFixed(2)
来源：http://cf.jianghongdianzi.cn

Java: String.format("%.2f", 3.14159)
来源：http://tm.huanxung.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ay.huixiangedu.cn

Ruby: format("%.2f", 3.14159)
来源：http://in.huixinmuqiang.cn

C#:   3.14159.ToString("F2")
来源：http://di.szxytkj.cn

[A22] 获取字符串长度
来源：http://nv.huixinmuqiang.cn

Py:   len(s)
来源：http://vt.panjiajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hv.szxytkj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ji.asd995.cn

TS:   s.length
来源：http://zx.chemitech.net.cn

Java: s.length()
来源：http://ka.9csxet.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lu.huixiangedu.cn

Ruby: s.length
来源：http://cx.colortex.cn

C#:   s.Length
来源：http://wq.panjiajie.cn

[A23] 大小写转换
来源：http://jv.bookmarksfly.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kd.nszjky.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wl.haigaiapp.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ro.yuexingan06.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zc.lnxyls.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ni.nszjky.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dq.bjjhwx.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dc.bookmarksfly.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zo.szxytkj.cn

[A24] 去除首尾空白
来源：http://qp.huixinmuqiang.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lb.panjiajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://aq.asd995.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nh.521024.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sz.shtwfgs.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ym.muxihuayi.cn

Go:   strings.TrimSpace(s)
来源：http://nm.chemitech.net.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://oe.shxzukj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qh.huanxung.cn

[A25] 字符串比较
来源：http://mo.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://qk.huanxung.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ot.wgjwhj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://be.lnxyls.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://eb.colortex.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bu.lnxyls.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mb.shtwfgs.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tn.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rl.szsharing.cn

[A26] 类型转换总览
来源：http://cl.szsharing.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fn.huixinmuqiang.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xm.shtwfgs.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ii.wgjwhj.cn

TS:   Number() String() Boolean() x as number
来源：http://qh.panjiajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yk.asd995.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bu.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qt.huixinmuqiang.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hu.gzmigu.cn

================================================================================
来源：http://ys.521024.cn

B. 流程控制
来源：http://vs.panjiajie.cn

================================================================================
来源：http://er.jianghongdianzi.cn

[B01] 条件判断 if / else
来源：http://do.haigaiapp.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mr.gzmigu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fg.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hc.jctech888.com.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sl.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zk.muxihuayi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sk.jctech888.com.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ap.yuexingan06.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ii.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://gh.hnjuh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://me.yuexingan06.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cr.szsharing.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ui.wgjwhj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jb.shtwfgs.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pf.huixiangedu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rh.muxihuayi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://oj.asd995.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wk.hnjuh.cn

[B03] switch / match / case
来源：http://ls.lnxyls.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sc.panjiajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wj.huanxung.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jn.asd995.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vl.huixinmuqiang.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sb.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ig.shxzukj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dr.haigaiapp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://si.panjiajie.cn

[B04] for 计数循环
来源：http://up.lnxyls.cn

Py:   for i in range(10): print(i)
来源：http://xp.haigaiapp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zf.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xt.hnjuh.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cr.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fp.colortex.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vx.nszjky.cn

Ruby: 10.times { |i| puts i }
来源：http://mz.wgjwhj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zy.wgjwhj.cn

[B05] 遍历数组 / 列表
来源：http://gs.nszjky.cn

Py:   for item in arr: print(item)
来源：http://jg.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hs.nszjky.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wq.yuexingan06.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ix.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://st.9csxet.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nl.bookmarksfly.cn

Ruby: arr.each { |item| puts item }
来源：http://dx.jianghongdianzi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xe.huixiangedu.cn

[B06] 遍历字典 / 对象
来源：http://ld.panjiajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ah.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rq.bookmarksfly.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://if.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://es.szxytkj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hc.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mx.bookmarksfly.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ve.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gc.gzmigu.cn

[B07] while 循环
来源：http://bi.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://nt.panjiajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://om.panjiajie.cn

JS:   while (i < 10) { i++; }
来源：http://zo.shxzukj.cn

TS:   while (i < 10) { i++; }
来源：http://dz.haigaiapp.cn

Java: while (i < 10) { i++; }
来源：http://ki.shxzukj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kg.shxzskj.cn

Ruby: while i < 10; i += 1; end
来源：http://wt.nszjky.cn

C#:   while (i < 10) { i++; }
来源：http://jj.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://ey.muxihuayi.cn

Py:   # 无 do-while：用 while True + break
来源：http://wu.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ux.hahajie.cn

JS:   do { i++; } while (i < 10);
来源：http://zs.521024.cn

TS:   do { i++; } while (i < 10);
来源：http://hg.muxihuayi.cn

Java: do { i++; } while (i < 10);
来源：http://yu.bookmarksfly.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mv.haigaiapp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://re.shtwfgs.cn

C#:   do { i++; } while (i < 10);
来源：http://tu.gzmigu.cn

[B09] break 与 continue
来源：http://td.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://je.hahajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gm.9csxet.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sh.newstarts.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zk.wgjwhj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ef.szxytkj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vp.huanxung.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gb.newstarts.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kt.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://ul.hahajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rj.jianghongdianzi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ip.shxzukj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kp.huixiangedu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lc.shxzskj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yn.colortex.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gx.panjiajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bo.yuntaijiaju.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://um.shxzskj.cn

[B11] 生成数字序列 / 区间
来源：http://gg.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://wz.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://qd.hnjuh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lj.bjjhwx.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ft.asd995.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fs.haigaiapp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xm.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://sb.hahajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://az.huanxung.cn

[B12] 跳出多层循环
来源：http://un.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nh.chemitech.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tu.wgjwhj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dk.wgjwhj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gy.nszjky.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ph.shxzskj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hv.huanxung.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rd.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rh.bjjhwx.cn

[B13] 判断是否为数字
来源：http://gi.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://mt.huixiangedu.cn

PHP:  is_numeric($x)
来源：http://zz.panjiajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bu.hahajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kz.nicolike.cn

Java: x instanceof Number
来源：http://fq.huixiangedu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vm.chemitech.net.cn

Ruby: x.is_a?(Numeric)
来源：http://sj.szxytkj.cn

C#:   x is int or double or decimal
来源：http://be.newstarts.cn

[B14] 判断值是否在集合内
来源：http://ry.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://km.shxzukj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bf.jctech888.com.cn

JS:   [1, 2, 3].includes(x)
来源：http://ud.bjjhwx.cn

TS:   [1, 2, 3].includes(x)
来源：http://ok.asd995.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://db.bjjhwx.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://af.nicolike.cn

Ruby: [1, 2, 3].include?(x)
来源：http://il.panjiajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yh.huanxung.cn

[B15] 布尔运算与取反
来源：http://od.shxzukj.cn

Py:   a and b or not c
来源：http://lf.newstarts.cn

PHP:  $a && $b || !$c
来源：http://qw.521024.cn

JS:   a && b || !c
来源：http://vs.huanxung.cn

TS:   a && b || !c
来源：http://hy.yuexingan06.cn

Java: a && b || !c
来源：http://ds.huixiangedu.cn

Go:   a && b || !c
来源：http://ys.huixinmuqiang.cn

Ruby: a && b || !c
来源：http://ia.hnjuh.cn

C#:   a && b || !c
来源：http://fr.521024.cn

[B16] 卫语句：不满足条件提前返回
来源：http://oa.shtwfgs.cn

Py:   if not data: return
来源：http://ax.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://ut.shxzskj.cn

JS:   if (!data) return;
来源：http://mz.yuexingan06.cn

TS:   if (!data) return;
来源：http://aj.shtwfgs.cn

Java: if (data == null) return;
来源：http://yb.nszjky.cn

Go:   if data == nil { return }
来源：http://wn.colortex.cn

Ruby: return if data.nil?
来源：http://bn.nszjky.cn

C#:   if (data == null) return;
来源：http://rr.nicolike.cn

================================================================================
来源：http://nj.hnjuh.cn

C. 函数与作用域
来源：http://ad.colortex.cn

================================================================================
来源：http://hl.szxytkj.cn

[C01] 定义函数
来源：http://nv.shxzukj.cn

Py:   def add(a, b): return a + b
来源：http://dy.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rz.wgjwhj.cn

JS:   function add(a, b) { return a + b; }
来源：http://aj.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ib.jianghongdianzi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pd.hnjuh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fd.yuntaijiaju.cn

Ruby: def add(a, b); a + b; end
来源：http://zt.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zk.chemitech.net.cn

[C02] 默认参数
来源：http://tc.chemitech.net.cn

Py:   def greet(name="World"): return name
来源：http://xc.hnjuh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gj.wgjwhj.cn

JS:   function greet(name = "World") { return name; }
来源：http://xs.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yn.shxzskj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rd.hnjuh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pz.jctech888.com.cn

Ruby: def greet(name = "World") = name
来源：http://dk.shxzskj.cn

C#:   string Greet(string name = "World") => name;
来源：http://tw.shxzskj.cn

[C03] 可变参数
来源：http://tq.jianghongdianzi.cn

Py:   def total(*args): return sum(args)
来源：http://em.bjjhwx.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pz.jianghongdianzi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bq.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bn.newstarts.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ms.huixiangedu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wk.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zs.521024.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wj.haigaiapp.cn

[C04] 命名参数 / 关键字参数
来源：http://hv.lnxyls.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ko.521024.cn


<!-- 参考信息 -->