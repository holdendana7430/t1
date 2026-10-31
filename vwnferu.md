代发 wailian999

Java: "第一行\n第二行"
来源：http://he.gzmigu.cn

Go:   "第一行\n第二行"
来源：http://yg.shxzukj.cn

Ruby: "第一行\n第二行"
来源：http://rb.panjiajie.cn

C#:   "第一行\n第二行"
来源：http://ux.szxytkj.cn

[A14] 注释写法
来源：http://xv.yuexingan06.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://cn.hnjuh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hj.muxihuayi.cn

JS:   // 单行；/* 多行 */
来源：http://zs.szxytkj.cn

TS:   // 单行；/* 多行 */
来源：http://eh.lnxyls.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pq.jctech888.com.cn

Go:   // 单行；/* 多行 */
来源：http://ih.hnjuh.cn

Ruby: # 单行；=begin 多行 =end
来源：http://yk.huixiangedu.cn

C#:   // 单行；/* 多行 */
来源：http://qh.hahajie.cn

[A15] 空值判断与默认值
来源：http://wu.colortex.cn

Py:   value = data or "默认值"
来源：http://ea.huixiangedu.cn

PHP:  $value = $data ?? "默认值";
来源：http://yb.shtwfgs.cn

JS:   const value = data ?? "默认值";
来源：http://zc.9csxet.cn

TS:   const value = data ?? "默认值";
来源：http://pq.huixiangedu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hc.jianghongdianzi.cn

Go:   if data == "" { data = "默认值" }
来源：http://rn.jctech888.com.cn

Ruby: value = data || "默认值"
来源：http://er.nicolike.cn

C#:   var value = data ?? "默认值";
来源：http://bb.muxihuayi.cn

[A16] 真假值判断规则
来源：http://kc.jctech888.com.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ci.newstarts.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hl.bookmarksfly.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ey.lnxyls.cn

TS:   if (!x) {}
来源：http://bj.colortex.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ah.jianghongdianzi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bc.gzmigu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zp.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bf.yuexingan06.cn

[A17] 位运算
来源：http://uq.muxihuayi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ub.shtwfgs.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ut.bookmarksfly.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ie.jianghongdianzi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mm.bookmarksfly.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hg.nicolike.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ax.bookmarksfly.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iu.szsharing.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cw.jianghongdianzi.cn

[A18] 字符与 ASCII 码互转
来源：http://ef.lnxyls.cn

Py:   ord("A"); chr(65)
来源：http://us.hnjuh.cn

PHP:  ord("A"); chr(65)
来源：http://ko.asd995.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jc.shxzskj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xv.panjiajie.cn

Java: (int) 'A'; (char) 65
来源：http://gi.9csxet.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jt.colortex.cn

Ruby: "A".ord; 65.chr
来源：http://lr.yuntaijiaju.cn

C#:   (int)'A'; (char)65
来源：http://rn.hnjuh.cn

[A19] 交换两个变量
来源：http://du.colortex.cn

Py:   a, b = b, a
来源：http://rp.nszjky.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jn.shtwfgs.cn

JS:   [a, b] = [b, a];
来源：http://qz.yuexingan06.cn

TS:   [a, b] = [b, a];
来源：http://sd.panjiajie.cn

Java: int t = a; a = b; b = t;
来源：http://ee.shxzukj.cn

Go:   a, b = b, a
来源：http://nk.bookmarksfly.cn

Ruby: a, b = b, a
来源：http://nv.wgjwhj.cn

C#:   (a, b) = (b, a);
来源：http://ci.nicolike.cn

[A20] 读取标准输入
来源：http://wt.yuntaijiaju.cn

Py:   name = input("请输入：")
来源：http://eb.yuntaijiaju.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://od.9csxet.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://se.haigaiapp.cn

TS:   // Node.js：readline 模块
来源：http://hs.521024.cn

Java: new Scanner(System.in).nextLine()
来源：http://hn.huanxung.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://eo.lnxyls.cn

Ruby: gets.chomp
来源：http://lb.nicolike.cn

C#:   Console.ReadLine();
来源：http://ud.gzmigu.cn

[A21] 保留指定小数位输出
来源：http://ht.bookmarksfly.cn

Py:   f"{3.14159:.2f}"
来源：http://xa.szsharing.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ai.jctech888.com.cn

JS:   (3.14159).toFixed(2)
来源：http://tg.yuexingan06.cn

TS:   (3.14159).toFixed(2)
来源：http://xc.huixiangedu.cn

Java: String.format("%.2f", 3.14159)
来源：http://hq.wgjwhj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mz.yuntaijiaju.cn

Ruby: format("%.2f", 3.14159)
来源：http://ry.bookmarksfly.cn

C#:   3.14159.ToString("F2")
来源：http://wr.9csxet.cn

[A22] 获取字符串长度
来源：http://ig.jctech888.com.cn

Py:   len(s)
来源：http://sc.yuexingan06.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sh.lnxyls.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fa.bjjhwx.cn

TS:   s.length
来源：http://el.muxihuayi.cn

Java: s.length()
来源：http://zn.shxzukj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nh.hahajie.cn

Ruby: s.length
来源：http://yu.asd995.cn

C#:   s.Length
来源：http://pj.haigaiapp.cn

[A23] 大小写转换
来源：http://ju.asd995.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://cs.yuntaijiaju.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ku.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ry.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://aj.asd995.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://eh.gzmigu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xr.yuntaijiaju.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://by.jctech888.com.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://kp.bjjhwx.cn

[A24] 去除首尾空白
来源：http://xh.521024.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gt.wgjwhj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bx.szsharing.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ht.chemitech.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vd.hnjuh.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bg.wgjwhj.cn

Go:   strings.TrimSpace(s)
来源：http://md.bjjhwx.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mo.muxihuayi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xl.muxihuayi.cn

[A25] 字符串比较
来源：http://ik.jctech888.com.cn

Py:   s1 == s2; s1 != s2
来源：http://me.jctech888.com.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hr.yuntaijiaju.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dv.hahajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pa.nszjky.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vb.hnjuh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://us.huixiangedu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ly.huixinmuqiang.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sm.panjiajie.cn

[A26] 类型转换总览
来源：http://lf.jianghongdianzi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gp.haigaiapp.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://km.asd995.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ae.bookmarksfly.cn

TS:   Number() String() Boolean() x as number
来源：http://au.bookmarksfly.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uc.muxihuayi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://de.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://od.muxihuayi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://oi.gzmigu.cn

================================================================================
来源：http://rs.gzmigu.cn

B. 流程控制
来源：http://vi.huanxung.cn

================================================================================
来源：http://px.newstarts.cn

[B01] 条件判断 if / else
来源：http://rg.yuntaijiaju.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ha.hahajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://oj.shxzskj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rv.chemitech.net.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ns.szxytkj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://up.bjjhwx.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://if.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kx.huanxung.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gw.9csxet.cn

[B02] 多分支 else if / elif
来源：http://jc.colortex.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kt.lnxyls.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nx.muxihuayi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sg.nszjky.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nm.yuexingan06.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://of.colortex.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sg.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ls.panjiajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kx.bjjhwx.cn

[B03] switch / match / case
来源：http://po.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wf.szsharing.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ec.yuexingan06.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xr.yuntaijiaju.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dq.bjjhwx.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ri.newstarts.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nf.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ce.haigaiapp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ko.nicolike.cn

[B04] for 计数循环
来源：http://ye.bookmarksfly.cn

Py:   for i in range(10): print(i)
来源：http://xk.panjiajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://eb.nszjky.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://at.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zn.521024.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zl.shxzskj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uh.hahajie.cn

Ruby: 10.times { |i| puts i }
来源：http://kz.chemitech.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://is.hnjuh.cn

[B05] 遍历数组 / 列表
来源：http://xe.nszjky.cn

Py:   for item in arr: print(item)
来源：http://um.asd995.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cq.nszjky.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fu.shtwfgs.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ze.bjjhwx.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://eh.hahajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yl.muxihuayi.cn

Ruby: arr.each { |item| puts item }
来源：http://ql.jianghongdianzi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cg.colortex.cn

[B06] 遍历字典 / 对象
来源：http://ij.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ce.huixinmuqiang.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qh.huixinmuqiang.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yi.nszjky.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cp.colortex.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sm.gzmigu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oh.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bb.shtwfgs.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://eo.9csxet.cn

[B07] while 循环
来源：http://to.521024.cn

Py:   while i < 10: i += 1
来源：http://iq.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ss.521024.cn

JS:   while (i < 10) { i++; }
来源：http://la.yuntaijiaju.cn

TS:   while (i < 10) { i++; }
来源：http://sd.huixiangedu.cn

Java: while (i < 10) { i++; }
来源：http://di.huanxung.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ug.lnxyls.cn

Ruby: while i < 10; i += 1; end
来源：http://vg.hnjuh.cn

C#:   while (i < 10) { i++; }
来源：http://tt.bookmarksfly.cn

[B08] do-while（至少执行一次）
来源：http://bz.bookmarksfly.cn

Py:   # 无 do-while：用 while True + break
来源：http://hb.jianghongdianzi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://br.huixiangedu.cn

JS:   do { i++; } while (i < 10);
来源：http://id.shtwfgs.cn

TS:   do { i++; } while (i < 10);
来源：http://my.chemitech.net.cn

Java: do { i++; } while (i < 10);
来源：http://ln.asd995.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vd.panjiajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ut.nicolike.cn

C#:   do { i++; } while (i < 10);
来源：http://qt.panjiajie.cn

[B09] break 与 continue
来源：http://rw.jianghongdianzi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xq.nszjky.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nu.yuntaijiaju.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://up.hnjuh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hq.jctech888.com.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eg.jctech888.com.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ds.521024.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fz.wgjwhj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lp.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://xq.panjiajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bu.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vz.nszjky.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jx.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dy.huixinmuqiang.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rh.szxytkj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dp.colortex.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jm.haigaiapp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jn.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://vu.nszjky.cn

Py:   list(range(0, 10, 2))
来源：http://vw.521024.cn

PHP:  range(0, 10, 2);
来源：http://yb.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nt.9csxet.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aj.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fg.nszjky.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ip.nszjky.cn

Ruby: (0...10).step(2).to_a
来源：http://ar.nicolike.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hp.yuntaijiaju.cn

[B12] 跳出多层循环
来源：http://xk.9csxet.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yc.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wj.lnxyls.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jc.huanxung.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ua.colortex.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kx.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qu.shtwfgs.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jf.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uq.chemitech.net.cn

[B13] 判断是否为数字
来源：http://ch.jctech888.com.cn

Py:   isinstance(x, (int, float))
来源：http://wp.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://ao.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iv.hnjuh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rh.9csxet.cn

Java: x instanceof Number
来源：http://pz.huanxung.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bm.9csxet.cn

Ruby: x.is_a?(Numeric)
来源：http://zr.shxzukj.cn

C#:   x is int or double or decimal
来源：http://jh.shtwfgs.cn

[B14] 判断值是否在集合内
来源：http://kq.nicolike.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hu.jianghongdianzi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kl.yuexingan06.cn

JS:   [1, 2, 3].includes(x)
来源：http://wq.colortex.cn

TS:   [1, 2, 3].includes(x)
来源：http://pa.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://op.bjjhwx.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pq.huixiangedu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zs.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vn.yuexingan06.cn

[B15] 布尔运算与取反
来源：http://fm.bjjhwx.cn

Py:   a and b or not c
来源：http://hh.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://ws.hahajie.cn

JS:   a && b || !c
来源：http://zy.nszjky.cn

TS:   a && b || !c
来源：http://qb.jianghongdianzi.cn

Java: a && b || !c
来源：http://rv.newstarts.cn

Go:   a && b || !c
来源：http://bt.szxytkj.cn

Ruby: a && b || !c
来源：http://mn.hnjuh.cn

C#:   a && b || !c
来源：http://rk.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jj.szsharing.cn

Py:   if not data: return
来源：http://yi.asd995.cn

PHP:  if (!$data) { return; }
来源：http://jh.muxihuayi.cn

JS:   if (!data) return;
来源：http://pz.chemitech.net.cn

TS:   if (!data) return;
来源：http://so.huixiangedu.cn

Java: if (data == null) return;
来源：http://al.huixinmuqiang.cn

Go:   if data == nil { return }
来源：http://of.gzmigu.cn

Ruby: return if data.nil?
来源：http://pg.9csxet.cn

C#:   if (data == null) return;
来源：http://qh.huixiangedu.cn

================================================================================
来源：http://no.muxihuayi.cn

C. 函数与作用域
来源：http://ak.huanxung.cn

================================================================================
来源：http://pp.shxzskj.cn

[C01] 定义函数
来源：http://um.shxzukj.cn

Py:   def add(a, b): return a + b
来源：http://ms.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ca.chemitech.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://wu.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rk.shtwfgs.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sp.9csxet.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tk.colortex.cn

Ruby: def add(a, b); a + b; end
来源：http://yc.lnxyls.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ak.wgjwhj.cn

[C02] 默认参数
来源：http://rk.521024.cn

Py:   def greet(name="World"): return name
来源：http://vp.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rl.jctech888.com.cn

JS:   function greet(name = "World") { return name; }
来源：http://fh.szxytkj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zh.muxihuayi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ko.haigaiapp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ox.jctech888.com.cn

Ruby: def greet(name = "World") = name
来源：http://dd.huixiangedu.cn

C#:   string Greet(string name = "World") => name;
来源：http://kt.szxytkj.cn

[C03] 可变参数
来源：http://iy.nszjky.cn

Py:   def total(*args): return sum(args)
来源：http://ai.521024.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nh.shxzukj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sy.szxytkj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xo.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ry.huixinmuqiang.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qi.yuexingan06.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tv.asd995.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rd.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://cj.panjiajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wf.panjiajie.cn


<!-- 参考信息 -->