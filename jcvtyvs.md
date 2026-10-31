代发 wailian999

Java: "第一行\n第二行"
来源：http://fo.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://lk.haigaiapp.cn

Ruby: "第一行\n第二行"
来源：http://mt.bookmarksfly.cn

C#:   "第一行\n第二行"
来源：http://ql.shxzukj.cn

[A14] 注释写法
来源：http://cz.nicolike.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pq.colortex.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://py.shxzukj.cn

JS:   // 单行；/* 多行 */
来源：http://ac.bookmarksfly.cn

TS:   // 单行；/* 多行 */
来源：http://ij.asd995.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wk.huixiangedu.cn

Go:   // 单行；/* 多行 */
来源：http://lm.huixiangedu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://jr.huixiangedu.cn

C#:   // 单行；/* 多行 */
来源：http://dq.hnjuh.cn

[A15] 空值判断与默认值
来源：http://lb.haigaiapp.cn

Py:   value = data or "默认值"
来源：http://bq.szsharing.cn

PHP:  $value = $data ?? "默认值";
来源：http://cb.nicolike.cn

JS:   const value = data ?? "默认值";
来源：http://qt.bjjhwx.cn

TS:   const value = data ?? "默认值";
来源：http://pn.521024.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qr.gzmigu.cn

Go:   if data == "" { data = "默认值" }
来源：http://ci.gzmigu.cn

Ruby: value = data || "默认值"
来源：http://av.jianghongdianzi.cn

C#:   var value = data ?? "默认值";
来源：http://ze.asd995.cn

[A16] 真假值判断规则
来源：http://xh.nicolike.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vx.huixiangedu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dv.hnjuh.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://no.colortex.cn

TS:   if (!x) {}
来源：http://mb.panjiajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tz.asd995.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xy.jctech888.com.cn

Ruby: unless x            # nil 与 false 为假
来源：http://cc.panjiajie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vy.9csxet.cn

[A17] 位运算
来源：http://vp.hahajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://it.jctech888.com.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uq.huixinmuqiang.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sq.haigaiapp.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zw.521024.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pc.9csxet.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://of.yuntaijiaju.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tt.huixinmuqiang.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cp.shtwfgs.cn

[A18] 字符与 ASCII 码互转
来源：http://al.jctech888.com.cn

Py:   ord("A"); chr(65)
来源：http://nt.nicolike.cn

PHP:  ord("A"); chr(65)
来源：http://jw.huanxung.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wj.szsharing.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qt.muxihuayi.cn

Java: (int) 'A'; (char) 65
来源：http://gb.jianghongdianzi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gt.shxzukj.cn

Ruby: "A".ord; 65.chr
来源：http://me.haigaiapp.cn

C#:   (int)'A'; (char)65
来源：http://qk.szsharing.cn

[A19] 交换两个变量
来源：http://sx.shxzskj.cn

Py:   a, b = b, a
来源：http://pz.chemitech.net.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://wf.huixiangedu.cn

JS:   [a, b] = [b, a];
来源：http://ug.gzmigu.cn

TS:   [a, b] = [b, a];
来源：http://bx.521024.cn

Java: int t = a; a = b; b = t;
来源：http://rb.colortex.cn

Go:   a, b = b, a
来源：http://ca.jianghongdianzi.cn

Ruby: a, b = b, a
来源：http://em.huixinmuqiang.cn

C#:   (a, b) = (b, a);
来源：http://dx.haigaiapp.cn

[A20] 读取标准输入
来源：http://md.haigaiapp.cn

Py:   name = input("请输入：")
来源：http://ru.panjiajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://mm.9csxet.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xc.yuntaijiaju.cn

TS:   // Node.js：readline 模块
来源：http://ib.jianghongdianzi.cn

Java: new Scanner(System.in).nextLine()
来源：http://we.asd995.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bd.jctech888.com.cn

Ruby: gets.chomp
来源：http://zn.bookmarksfly.cn

C#:   Console.ReadLine();
来源：http://se.panjiajie.cn

[A21] 保留指定小数位输出
来源：http://ju.9csxet.cn

Py:   f"{3.14159:.2f}"
来源：http://so.shxzukj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zu.bookmarksfly.cn

JS:   (3.14159).toFixed(2)
来源：http://cu.shxzukj.cn

TS:   (3.14159).toFixed(2)
来源：http://cd.haigaiapp.cn

Java: String.format("%.2f", 3.14159)
来源：http://iv.colortex.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ex.hahajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://kn.chemitech.net.cn

C#:   3.14159.ToString("F2")
来源：http://fe.shxzukj.cn

[A22] 获取字符串长度
来源：http://la.newstarts.cn

Py:   len(s)
来源：http://nq.521024.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ws.szxytkj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ic.colortex.cn

TS:   s.length
来源：http://ca.jianghongdianzi.cn

Java: s.length()
来源：http://uj.bookmarksfly.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jn.521024.cn

Ruby: s.length
来源：http://wn.hnjuh.cn

C#:   s.Length
来源：http://mj.panjiajie.cn

[A23] 大小写转换
来源：http://gy.haigaiapp.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://yf.shtwfgs.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jm.huixinmuqiang.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xs.huixiangedu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qe.wgjwhj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vo.shxzukj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zr.nicolike.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qa.szxytkj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qy.shtwfgs.cn

[A24] 去除首尾空白
来源：http://hi.bjjhwx.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ex.newstarts.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cp.huixinmuqiang.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fb.jctech888.com.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://at.colortex.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://er.gzmigu.cn

Go:   strings.TrimSpace(s)
来源：http://ex.521024.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://eo.colortex.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://id.521024.cn

[A25] 字符串比较
来源：http://no.521024.cn

Py:   s1 == s2; s1 != s2
来源：http://sl.521024.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xl.hahajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ja.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yz.9csxet.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ho.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://en.muxihuayi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fp.9csxet.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mi.szxytkj.cn

[A26] 类型转换总览
来源：http://fs.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://np.nicolike.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uq.gzmigu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xw.hnjuh.cn

TS:   Number() String() Boolean() x as number
来源：http://zh.gzmigu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zt.muxihuayi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tn.jianghongdianzi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://xb.9csxet.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://km.muxihuayi.cn

================================================================================
来源：http://hi.hnjuh.cn

B. 流程控制
来源：http://oc.shtwfgs.cn

================================================================================
来源：http://fi.muxihuayi.cn

[B01] 条件判断 if / else
来源：http://av.shxzskj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rt.wgjwhj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://eg.huanxung.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nt.newstarts.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lb.nicolike.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gk.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gi.huixiangedu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fc.yuexingan06.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bw.521024.cn

[B02] 多分支 else if / elif
来源：http://jv.chemitech.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sr.szsharing.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xt.jianghongdianzi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://no.jctech888.com.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vr.bjjhwx.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lq.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nh.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dg.huanxung.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fe.jianghongdianzi.cn

[B03] switch / match / case
来源：http://in.wgjwhj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bv.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bb.szsharing.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xe.chemitech.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jw.colortex.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hn.bookmarksfly.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://um.szxytkj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://me.hnjuh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sw.asd995.cn

[B04] for 计数循环
来源：http://id.asd995.cn

Py:   for i in range(10): print(i)
来源：http://tm.gzmigu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ao.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ud.lnxyls.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://si.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kk.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ru.jctech888.com.cn

Ruby: 10.times { |i| puts i }
来源：http://rq.gzmigu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tz.jianghongdianzi.cn

[B05] 遍历数组 / 列表
来源：http://tv.muxihuayi.cn

Py:   for item in arr: print(item)
来源：http://ab.asd995.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dd.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lw.huixinmuqiang.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://oh.chemitech.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://om.hnjuh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://la.newstarts.cn

Ruby: arr.each { |item| puts item }
来源：http://iu.bjjhwx.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fx.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://yg.bjjhwx.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ht.szsharing.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://of.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sv.521024.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fd.panjiajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://se.nszjky.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jj.yuntaijiaju.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lr.shxzskj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bj.nicolike.cn

[B07] while 循环
来源：http://rr.hahajie.cn

Py:   while i < 10: i += 1
来源：http://tk.bookmarksfly.cn

PHP:  while ($i < 10) { $i++; }
来源：http://df.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://aa.9csxet.cn

TS:   while (i < 10) { i++; }
来源：http://xu.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://qh.huanxung.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jy.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://ss.colortex.cn

C#:   while (i < 10) { i++; }
来源：http://br.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://kr.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://tf.haigaiapp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xy.jctech888.com.cn

JS:   do { i++; } while (i < 10);
来源：http://gk.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://xk.nicolike.cn

Java: do { i++; } while (i < 10);
来源：http://bx.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ar.jianghongdianzi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wq.panjiajie.cn

C#:   do { i++; } while (i < 10);
来源：http://kh.asd995.cn

[B09] break 与 continue
来源：http://bi.yuntaijiaju.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://it.panjiajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kl.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ly.yuexingan06.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ak.szsharing.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gv.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ax.shxzukj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kb.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pa.szxytkj.cn

[B10] 遍历同时拿索引
来源：http://ow.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rg.yuntaijiaju.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sl.bjjhwx.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ka.colortex.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ev.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ih.bookmarksfly.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xk.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xt.yuexingan06.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vh.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://rq.jctech888.com.cn

Py:   list(range(0, 10, 2))
来源：http://gt.newstarts.cn

PHP:  range(0, 10, 2);
来源：http://mx.shtwfgs.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qc.bookmarksfly.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ii.colortex.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ts.bjjhwx.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kc.nszjky.cn

Ruby: (0...10).step(2).to_a
来源：http://oe.yuntaijiaju.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ks.chemitech.net.cn

[B12] 跳出多层循环
来源：http://bi.colortex.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ln.asd995.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://li.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vq.shtwfgs.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gu.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jk.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dd.chemitech.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ae.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bv.huixiangedu.cn

[B13] 判断是否为数字
来源：http://bb.lnxyls.cn

Py:   isinstance(x, (int, float))
来源：http://xz.jianghongdianzi.cn

PHP:  is_numeric($x)
来源：http://un.panjiajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://im.hnjuh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ry.jctech888.com.cn

Java: x instanceof Number
来源：http://hu.szxytkj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yp.colortex.cn

Ruby: x.is_a?(Numeric)
来源：http://bv.wgjwhj.cn

C#:   x is int or double or decimal
来源：http://ub.szsharing.cn

[B14] 判断值是否在集合内
来源：http://st.chemitech.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yp.521024.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://up.szxytkj.cn

JS:   [1, 2, 3].includes(x)
来源：http://qk.wgjwhj.cn

TS:   [1, 2, 3].includes(x)
来源：http://ym.lnxyls.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ru.huixiangedu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bd.bookmarksfly.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zd.huixiangedu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yu.jianghongdianzi.cn

[B15] 布尔运算与取反
来源：http://db.shxzskj.cn

Py:   a and b or not c
来源：http://wk.bookmarksfly.cn

PHP:  $a && $b || !$c
来源：http://pz.asd995.cn

JS:   a && b || !c
来源：http://ru.huixinmuqiang.cn

TS:   a && b || !c
来源：http://og.bookmarksfly.cn

Java: a && b || !c
来源：http://fs.huixinmuqiang.cn

Go:   a && b || !c
来源：http://jo.muxihuayi.cn

Ruby: a && b || !c
来源：http://oo.huanxung.cn

C#:   a && b || !c
来源：http://mh.newstarts.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wt.yuntaijiaju.cn

Py:   if not data: return
来源：http://zs.lnxyls.cn

PHP:  if (!$data) { return; }
来源：http://iy.shxzukj.cn

JS:   if (!data) return;
来源：http://md.wgjwhj.cn

TS:   if (!data) return;
来源：http://os.yuntaijiaju.cn

Java: if (data == null) return;
来源：http://hh.newstarts.cn

Go:   if data == nil { return }
来源：http://ar.huixinmuqiang.cn

Ruby: return if data.nil?
来源：http://ap.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://fw.huixiangedu.cn

================================================================================
来源：http://wt.yuntaijiaju.cn

C. 函数与作用域
来源：http://wx.gzmigu.cn

================================================================================
来源：http://lo.panjiajie.cn

[C01] 定义函数
来源：http://hs.bookmarksfly.cn

Py:   def add(a, b): return a + b
来源：http://fw.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rx.muxihuayi.cn

JS:   function add(a, b) { return a + b; }
来源：http://je.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fp.jianghongdianzi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ey.nszjky.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lp.521024.cn

Ruby: def add(a, b); a + b; end
来源：http://cv.wgjwhj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pa.muxihuayi.cn

[C02] 默认参数
来源：http://gp.muxihuayi.cn

Py:   def greet(name="World"): return name
来源：http://bm.shtwfgs.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rp.bookmarksfly.cn

JS:   function greet(name = "World") { return name; }
来源：http://dn.huanxung.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ue.asd995.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ku.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zm.521024.cn

Ruby: def greet(name = "World") = name
来源：http://cn.bjjhwx.cn

C#:   string Greet(string name = "World") => name;
来源：http://bw.hahajie.cn

[C03] 可变参数
来源：http://xb.shtwfgs.cn

Py:   def total(*args): return sum(args)
来源：http://vl.asd995.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rs.nszjky.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yq.hahajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sa.panjiajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vd.huixiangedu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dd.haigaiapp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ga.hnjuh.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zx.hahajie.cn

[C04] 命名参数 / 关键字参数
来源：http://dq.shxzukj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fj.huixinmuqiang.cn


<!-- 参考信息 -->