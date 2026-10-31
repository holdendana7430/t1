代发 wailian999

Java: "第一行\n第二行"
来源：http://pb.szsharing.cn

Go:   "第一行\n第二行"
来源：http://gd.huanxung.cn

Ruby: "第一行\n第二行"
来源：http://ic.nszjky.cn

C#:   "第一行\n第二行"
来源：http://oi.jianghongdianzi.cn

[A14] 注释写法
来源：http://ir.szsharing.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pd.huixiangedu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://zy.jctech888.com.cn

JS:   // 单行；/* 多行 */
来源：http://jh.hahajie.cn

TS:   // 单行；/* 多行 */
来源：http://tk.shtwfgs.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://db.panjiajie.cn

Go:   // 单行；/* 多行 */
来源：http://mb.huixiangedu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://zd.chemitech.net.cn

C#:   // 单行；/* 多行 */
来源：http://ia.colortex.cn

[A15] 空值判断与默认值
来源：http://es.bjjhwx.cn

Py:   value = data or "默认值"
来源：http://au.huixiangedu.cn

PHP:  $value = $data ?? "默认值";
来源：http://vt.newstarts.cn

JS:   const value = data ?? "默认值";
来源：http://ga.chemitech.net.cn

TS:   const value = data ?? "默认值";
来源：http://gv.newstarts.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qd.panjiajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://ha.szxytkj.cn

Ruby: value = data || "默认值"
来源：http://pr.panjiajie.cn

C#:   var value = data ?? "默认值";
来源：http://vr.szsharing.cn

[A16] 真假值判断规则
来源：http://fw.hahajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vr.asd995.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vl.521024.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://de.jianghongdianzi.cn

TS:   if (!x) {}
来源：http://vq.asd995.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://el.nszjky.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qa.newstarts.cn

Ruby: unless x            # nil 与 false 为假
来源：http://fg.nszjky.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bu.huixiangedu.cn

[A17] 位运算
来源：http://il.yuexingan06.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mn.szsharing.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://yo.gzmigu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xd.gzmigu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bp.szxytkj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kn.nszjky.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qe.9csxet.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lp.lnxyls.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://az.muxihuayi.cn

[A18] 字符与 ASCII 码互转
来源：http://av.gzmigu.cn

Py:   ord("A"); chr(65)
来源：http://tj.jctech888.com.cn

PHP:  ord("A"); chr(65)
来源：http://fm.haigaiapp.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ou.bjjhwx.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dz.jianghongdianzi.cn

Java: (int) 'A'; (char) 65
来源：http://sf.panjiajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ly.panjiajie.cn

Ruby: "A".ord; 65.chr
来源：http://ss.szsharing.cn

C#:   (int)'A'; (char)65
来源：http://ll.szxytkj.cn

[A19] 交换两个变量
来源：http://ry.muxihuayi.cn

Py:   a, b = b, a
来源：http://jm.yuexingan06.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ml.szsharing.cn

JS:   [a, b] = [b, a];
来源：http://vr.huixiangedu.cn

TS:   [a, b] = [b, a];
来源：http://eg.colortex.cn

Java: int t = a; a = b; b = t;
来源：http://nc.gzmigu.cn

Go:   a, b = b, a
来源：http://px.newstarts.cn

Ruby: a, b = b, a
来源：http://sd.muxihuayi.cn

C#:   (a, b) = (b, a);
来源：http://xe.huixiangedu.cn

[A20] 读取标准输入
来源：http://ew.jianghongdianzi.cn

Py:   name = input("请输入：")
来源：http://yk.huixiangedu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://jl.panjiajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dx.nicolike.cn

TS:   // Node.js：readline 模块
来源：http://cz.jctech888.com.cn

Java: new Scanner(System.in).nextLine()
来源：http://yd.nszjky.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yd.gzmigu.cn

Ruby: gets.chomp
来源：http://hn.nszjky.cn

C#:   Console.ReadLine();
来源：http://uf.yuexingan06.cn

[A21] 保留指定小数位输出
来源：http://gi.9csxet.cn

Py:   f"{3.14159:.2f}"
来源：http://zn.yuexingan06.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rw.521024.cn

JS:   (3.14159).toFixed(2)
来源：http://eb.bookmarksfly.cn

TS:   (3.14159).toFixed(2)
来源：http://rw.shxzukj.cn

Java: String.format("%.2f", 3.14159)
来源：http://fw.nicolike.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gg.haigaiapp.cn

Ruby: format("%.2f", 3.14159)
来源：http://pw.9csxet.cn

C#:   3.14159.ToString("F2")
来源：http://ej.gzmigu.cn

[A22] 获取字符串长度
来源：http://uc.shxzskj.cn

Py:   len(s)
来源：http://fa.521024.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yg.gzmigu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wg.huixinmuqiang.cn

TS:   s.length
来源：http://vg.asd995.cn

Java: s.length()
来源：http://ki.chemitech.net.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qv.colortex.cn

Ruby: s.length
来源：http://xo.huixinmuqiang.cn

C#:   s.Length
来源：http://ik.lnxyls.cn

[A23] 大小写转换
来源：http://cd.gzmigu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://we.shtwfgs.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fm.shtwfgs.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xl.panjiajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mm.nicolike.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nb.jianghongdianzi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rq.chemitech.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wg.521024.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ef.szxytkj.cn

[A24] 去除首尾空白
来源：http://zl.521024.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ug.huanxung.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qp.muxihuayi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fq.shxzukj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fj.newstarts.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tj.asd995.cn

Go:   strings.TrimSpace(s)
来源：http://kh.nszjky.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fk.newstarts.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kl.bookmarksfly.cn

[A25] 字符串比较
来源：http://nj.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://xe.bookmarksfly.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fr.521024.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nj.hahajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qo.lnxyls.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kc.huixinmuqiang.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ym.huixinmuqiang.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ba.9csxet.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ec.wgjwhj.cn

[A26] 类型转换总览
来源：http://va.huixinmuqiang.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tw.gzmigu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dk.yuexingan06.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kz.huanxung.cn

TS:   Number() String() Boolean() x as number
来源：http://ut.gzmigu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vf.szsharing.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cj.muxihuayi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ho.szxytkj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vz.jctech888.com.cn

================================================================================
来源：http://cw.lnxyls.cn

B. 流程控制
来源：http://qm.jctech888.com.cn

================================================================================
来源：http://zk.9csxet.cn

[B01] 条件判断 if / else
来源：http://ds.szxytkj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qs.szxytkj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vn.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vx.muxihuayi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vs.lnxyls.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hx.colortex.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ai.lnxyls.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rh.asd995.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pg.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://jt.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://th.newstarts.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zf.chemitech.net.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mp.hnjuh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uk.9csxet.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ti.muxihuayi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ax.shxzskj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zc.bookmarksfly.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://in.bjjhwx.cn

[B03] switch / match / case
来源：http://fg.yuexingan06.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lx.hnjuh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://op.yuexingan06.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qt.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yn.huixinmuqiang.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rs.huanxung.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ze.yuntaijiaju.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ry.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://to.jctech888.com.cn

[B04] for 计数循环
来源：http://pj.nicolike.cn

Py:   for i in range(10): print(i)
来源：http://io.yuexingan06.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yy.shxzskj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bc.szxytkj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hg.shxzskj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zb.hahajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oq.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://md.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vu.yuexingan06.cn

[B05] 遍历数组 / 列表
来源：http://bi.shxzskj.cn

Py:   for item in arr: print(item)
来源：http://ua.bookmarksfly.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bs.521024.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wu.bjjhwx.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zf.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zs.bjjhwx.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://io.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://ih.asd995.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sw.colortex.cn

[B06] 遍历字典 / 对象
来源：http://pp.hahajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://op.521024.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jx.hahajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fv.nicolike.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wi.hnjuh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ta.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jq.shxzskj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ws.panjiajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hu.hahajie.cn

[B07] while 循环
来源：http://oh.hnjuh.cn

Py:   while i < 10: i += 1
来源：http://bf.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lb.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://dw.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://ms.yuexingan06.cn

Java: while (i < 10) { i++; }
来源：http://zm.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sy.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://wo.9csxet.cn

C#:   while (i < 10) { i++; }
来源：http://ax.521024.cn

[B08] do-while（至少执行一次）
来源：http://ci.panjiajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://nc.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ys.szsharing.cn

JS:   do { i++; } while (i < 10);
来源：http://dd.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://qg.szsharing.cn

Java: do { i++; } while (i < 10);
来源：http://gg.haigaiapp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ai.szxytkj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://sy.wgjwhj.cn

C#:   do { i++; } while (i < 10);
来源：http://nt.wgjwhj.cn

[B09] break 与 continue
来源：http://rh.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ip.muxihuayi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ig.yuexingan06.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xo.colortex.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://by.shxzukj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dc.asd995.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xr.nszjky.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://df.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lr.lnxyls.cn

[B10] 遍历同时拿索引
来源：http://ek.yuexingan06.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ip.521024.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fk.shxzskj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pp.nicolike.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dg.shxzukj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ml.jianghongdianzi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vg.yuexingan06.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ak.gzmigu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://we.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://wt.shtwfgs.cn

Py:   list(range(0, 10, 2))
来源：http://ri.hnjuh.cn

PHP:  range(0, 10, 2);
来源：http://lh.gzmigu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ar.haigaiapp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fs.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sg.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hs.nszjky.cn

Ruby: (0...10).step(2).to_a
来源：http://yy.hahajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fe.wgjwhj.cn

[B12] 跳出多层循环
来源：http://bk.panjiajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xv.bookmarksfly.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yp.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fb.hnjuh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://es.newstarts.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ym.asd995.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hg.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://am.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gv.shxzukj.cn

[B13] 判断是否为数字
来源：http://xa.huanxung.cn

Py:   isinstance(x, (int, float))
来源：http://on.521024.cn

PHP:  is_numeric($x)
来源：http://cz.hnjuh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uh.huanxung.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yb.bjjhwx.cn

Java: x instanceof Number
来源：http://mq.huanxung.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vy.lnxyls.cn

Ruby: x.is_a?(Numeric)
来源：http://sh.shxzukj.cn

C#:   x is int or double or decimal
来源：http://jl.asd995.cn

[B14] 判断值是否在集合内
来源：http://hf.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qu.huixiangedu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://of.gzmigu.cn

JS:   [1, 2, 3].includes(x)
来源：http://fd.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://ac.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yp.szsharing.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://eb.yuexingan06.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hc.hahajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mq.hahajie.cn

[B15] 布尔运算与取反
来源：http://mh.521024.cn

Py:   a and b or not c
来源：http://pw.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://nc.jianghongdianzi.cn

JS:   a && b || !c
来源：http://uc.yuntaijiaju.cn

TS:   a && b || !c
来源：http://iw.hahajie.cn

Java: a && b || !c
来源：http://ta.asd995.cn

Go:   a && b || !c
来源：http://ek.9csxet.cn

Ruby: a && b || !c
来源：http://vd.nszjky.cn

C#:   a && b || !c
来源：http://wx.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zv.yuexingan06.cn

Py:   if not data: return
来源：http://ns.shtwfgs.cn

PHP:  if (!$data) { return; }
来源：http://qi.shxzukj.cn

JS:   if (!data) return;
来源：http://ap.asd995.cn

TS:   if (!data) return;
来源：http://yq.9csxet.cn

Java: if (data == null) return;
来源：http://em.bookmarksfly.cn

Go:   if data == nil { return }
来源：http://tm.hahajie.cn

Ruby: return if data.nil?
来源：http://rz.szsharing.cn

C#:   if (data == null) return;
来源：http://kj.muxihuayi.cn

================================================================================
来源：http://qc.hnjuh.cn

C. 函数与作用域
来源：http://qh.hahajie.cn

================================================================================
来源：http://pv.szxytkj.cn

[C01] 定义函数
来源：http://sv.hahajie.cn

Py:   def add(a, b): return a + b
来源：http://ea.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tt.gzmigu.cn

JS:   function add(a, b) { return a + b; }
来源：http://lz.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eu.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ai.bookmarksfly.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zd.shxzskj.cn

Ruby: def add(a, b); a + b; end
来源：http://dp.muxihuayi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://do.huixiangedu.cn

[C02] 默认参数
来源：http://to.yuexingan06.cn

Py:   def greet(name="World"): return name
来源：http://gd.hahajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://to.9csxet.cn

JS:   function greet(name = "World") { return name; }
来源：http://ak.wgjwhj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bb.bookmarksfly.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lf.szsharing.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vp.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://rw.panjiajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://lq.huanxung.cn

[C03] 可变参数
来源：http://rq.muxihuayi.cn

Py:   def total(*args): return sum(args)
来源：http://fe.yuexingan06.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rv.shxzukj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lm.asd995.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vs.huixinmuqiang.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fs.huixinmuqiang.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://eq.chemitech.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vs.yuntaijiaju.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vq.chemitech.net.cn

[C04] 命名参数 / 关键字参数
来源：http://vu.huixiangedu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://la.shxzskj.cn


<!-- 参考信息 -->