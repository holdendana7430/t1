代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://pm.colortex.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://sz.nszjky.cn

Go:   // 单行；/* 多行 */
来源：http://oi.szxytkj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://lg.asd995.cn

C#:   // 单行；/* 多行 */
来源：http://nm.bookmarksfly.cn

[A15] 空值判断与默认值
来源：http://kg.colortex.cn

Py:   value = data or "默认值"
来源：http://nk.bjjhwx.cn

PHP:  $value = $data ?? "默认值";
来源：http://zk.shxzskj.cn

JS:   const value = data ?? "默认值";
来源：http://tx.shxzukj.cn

TS:   const value = data ?? "默认值";
来源：http://ce.gzmigu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jp.panjiajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://tf.521024.cn

Ruby: value = data || "默认值"
来源：http://ou.szxytkj.cn

C#:   var value = data ?? "默认值";
来源：http://hn.yuntaijiaju.cn

[A16] 真假值判断规则
来源：http://su.huixiangedu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kv.newstarts.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://sa.9csxet.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uj.wgjwhj.cn

TS:   if (!x) {}
来源：http://qu.nszjky.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mc.wgjwhj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zu.nicolike.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ra.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://al.asd995.cn

[A17] 位运算
来源：http://uh.hahajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ku.hnjuh.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gr.szxytkj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ks.panjiajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://de.huixiangedu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tk.szxytkj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ue.szxytkj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://df.panjiajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jl.shxzskj.cn

[A18] 字符与 ASCII 码互转
来源：http://uc.bjjhwx.cn

Py:   ord("A"); chr(65)
来源：http://es.chemitech.net.cn

PHP:  ord("A"); chr(65)
来源：http://kr.lnxyls.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mm.gzmigu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tf.newstarts.cn

Java: (int) 'A'; (char) 65
来源：http://zr.yuntaijiaju.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vy.szsharing.cn

Ruby: "A".ord; 65.chr
来源：http://eb.muxihuayi.cn

C#:   (int)'A'; (char)65
来源：http://uk.huixiangedu.cn

[A19] 交换两个变量
来源：http://mg.gzmigu.cn

Py:   a, b = b, a
来源：http://vh.gzmigu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://js.shtwfgs.cn

JS:   [a, b] = [b, a];
来源：http://te.colortex.cn

TS:   [a, b] = [b, a];
来源：http://lk.jianghongdianzi.cn

Java: int t = a; a = b; b = t;
来源：http://cv.yuexingan06.cn

Go:   a, b = b, a
来源：http://if.9csxet.cn

Ruby: a, b = b, a
来源：http://hp.hnjuh.cn

C#:   (a, b) = (b, a);
来源：http://oq.huixiangedu.cn

[A20] 读取标准输入
来源：http://yl.nicolike.cn

Py:   name = input("请输入：")
来源：http://sr.bjjhwx.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://be.huanxung.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://os.hnjuh.cn

TS:   // Node.js：readline 模块
来源：http://io.asd995.cn

Java: new Scanner(System.in).nextLine()
来源：http://qz.yuntaijiaju.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pa.521024.cn

Ruby: gets.chomp
来源：http://lp.haigaiapp.cn

C#:   Console.ReadLine();
来源：http://hu.nicolike.cn

[A21] 保留指定小数位输出
来源：http://ce.panjiajie.cn

Py:   f"{3.14159:.2f}"
来源：http://dq.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qf.bjjhwx.cn

JS:   (3.14159).toFixed(2)
来源：http://zp.bjjhwx.cn

TS:   (3.14159).toFixed(2)
来源：http://mt.nicolike.cn

Java: String.format("%.2f", 3.14159)
来源：http://dw.521024.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vm.yuntaijiaju.cn

Ruby: format("%.2f", 3.14159)
来源：http://la.wgjwhj.cn

C#:   3.14159.ToString("F2")
来源：http://vy.yuntaijiaju.cn

[A22] 获取字符串长度
来源：http://zp.521024.cn

Py:   len(s)
来源：http://mi.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yd.bjjhwx.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ut.bjjhwx.cn

TS:   s.length
来源：http://nv.gzmigu.cn

Java: s.length()
来源：http://ll.hahajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tf.szxytkj.cn

Ruby: s.length
来源：http://oh.panjiajie.cn

C#:   s.Length
来源：http://ua.asd995.cn

[A23] 大小写转换
来源：http://dm.szxytkj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zp.colortex.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lx.jianghongdianzi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yp.szsharing.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yq.szsharing.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cw.521024.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fo.nicolike.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://px.wgjwhj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zr.szxytkj.cn

[A24] 去除首尾空白
来源：http://dk.nszjky.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://js.gzmigu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ic.muxihuayi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fw.nszjky.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ot.shxzskj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vn.jianghongdianzi.cn

Go:   strings.TrimSpace(s)
来源：http://gd.haigaiapp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://go.lnxyls.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zt.newstarts.cn

[A25] 字符串比较
来源：http://uy.shxzukj.cn

Py:   s1 == s2; s1 != s2
来源：http://uw.huanxung.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ue.huixiangedu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lf.521024.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bb.gzmigu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ga.yuntaijiaju.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ya.bjjhwx.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mx.521024.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nh.9csxet.cn

[A26] 类型转换总览
来源：http://qu.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uy.asd995.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://en.szxytkj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ow.yuntaijiaju.cn

TS:   Number() String() Boolean() x as number
来源：http://xr.gzmigu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gb.hnjuh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qv.nszjky.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mo.yuexingan06.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://oy.nicolike.cn

================================================================================
来源：http://xc.shxzukj.cn

B. 流程控制
来源：http://fh.hnjuh.cn

================================================================================
来源：http://ny.jianghongdianzi.cn

[B01] 条件判断 if / else
来源：http://js.muxihuayi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vc.wgjwhj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://oe.haigaiapp.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ec.newstarts.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sn.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ah.nicolike.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ze.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hi.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://oa.huixinmuqiang.cn

[B02] 多分支 else if / elif
来源：http://dk.huixinmuqiang.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bd.szsharing.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uk.newstarts.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ck.hahajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://no.shtwfgs.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fe.shtwfgs.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://eh.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rr.gzmigu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aq.colortex.cn

[B03] switch / match / case
来源：http://ch.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ut.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fx.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dy.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sw.shtwfgs.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ri.hnjuh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://eb.shxzukj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gs.521024.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ou.panjiajie.cn

[B04] for 计数循环
来源：http://mj.panjiajie.cn

Py:   for i in range(10): print(i)
来源：http://xh.lnxyls.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bf.jctech888.com.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ky.lnxyls.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zy.huixinmuqiang.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lu.hahajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zg.szsharing.cn

Ruby: 10.times { |i| puts i }
来源：http://wy.shxzskj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ib.wgjwhj.cn

[B05] 遍历数组 / 列表
来源：http://jk.szxytkj.cn

Py:   for item in arr: print(item)
来源：http://uf.haigaiapp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fe.yuntaijiaju.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://in.gzmigu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ko.chemitech.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://of.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zg.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://aa.yuexingan06.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oj.haigaiapp.cn

[B06] 遍历字典 / 对象
来源：http://wh.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ey.colortex.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sb.hnjuh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wy.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iu.bookmarksfly.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tr.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rz.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gl.muxihuayi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xo.gzmigu.cn

[B07] while 循环
来源：http://ba.hnjuh.cn

Py:   while i < 10: i += 1
来源：http://uw.szsharing.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gk.asd995.cn

JS:   while (i < 10) { i++; }
来源：http://bv.nicolike.cn

TS:   while (i < 10) { i++; }
来源：http://qi.shxzskj.cn

Java: while (i < 10) { i++; }
来源：http://yn.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zv.yuntaijiaju.cn

Ruby: while i < 10; i += 1; end
来源：http://ja.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://bb.chemitech.net.cn

[B08] do-while（至少执行一次）
来源：http://xw.szsharing.cn

Py:   # 无 do-while：用 while True + break
来源：http://oo.panjiajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xp.521024.cn

JS:   do { i++; } while (i < 10);
来源：http://nw.szsharing.cn

TS:   do { i++; } while (i < 10);
来源：http://na.haigaiapp.cn

Java: do { i++; } while (i < 10);
来源：http://yb.jianghongdianzi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://br.lnxyls.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ja.shxzukj.cn

C#:   do { i++; } while (i < 10);
来源：http://qq.shxzukj.cn

[B09] break 与 continue
来源：http://uv.panjiajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lg.shxzskj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ce.gzmigu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wb.huixinmuqiang.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zg.asd995.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ql.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xn.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bw.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://af.shtwfgs.cn

[B10] 遍历同时拿索引
来源：http://zr.shtwfgs.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nh.lnxyls.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://si.521024.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hu.shxzskj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sd.shtwfgs.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://na.asd995.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xt.muxihuayi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jl.panjiajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cs.huixiangedu.cn

[B11] 生成数字序列 / 区间
来源：http://px.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://rv.521024.cn

PHP:  range(0, 10, 2);
来源：http://qi.yuntaijiaju.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ag.huixiangedu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ak.asd995.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ju.yuexingan06.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cf.hahajie.cn

Ruby: (0...10).step(2).to_a
来源：http://xe.bjjhwx.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dp.nszjky.cn

[B12] 跳出多层循环
来源：http://fp.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://as.shxzskj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kl.huixiangedu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://eo.9csxet.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fk.asd995.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ll.newstarts.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ua.chemitech.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yi.nszjky.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mw.huixinmuqiang.cn

[B13] 判断是否为数字
来源：http://co.shxzskj.cn

Py:   isinstance(x, (int, float))
来源：http://yl.huixiangedu.cn

PHP:  is_numeric($x)
来源：http://hn.wgjwhj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bk.jctech888.com.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eg.lnxyls.cn

Java: x instanceof Number
来源：http://ds.shxzskj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://df.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://wq.huanxung.cn

C#:   x is int or double or decimal
来源：http://by.nszjky.cn

[B14] 判断值是否在集合内
来源：http://lj.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hl.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://um.yuntaijiaju.cn

JS:   [1, 2, 3].includes(x)
来源：http://fg.lnxyls.cn

TS:   [1, 2, 3].includes(x)
来源：http://fm.yuexingan06.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mw.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xb.huixiangedu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fa.colortex.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ao.lnxyls.cn

[B15] 布尔运算与取反
来源：http://ma.haigaiapp.cn

Py:   a and b or not c
来源：http://vy.shxzukj.cn

PHP:  $a && $b || !$c
来源：http://ke.panjiajie.cn

JS:   a && b || !c
来源：http://fl.hahajie.cn

TS:   a && b || !c
来源：http://ph.newstarts.cn

Java: a && b || !c
来源：http://kw.asd995.cn

Go:   a && b || !c
来源：http://fc.haigaiapp.cn

Ruby: a && b || !c
来源：http://gx.panjiajie.cn

C#:   a && b || !c
来源：http://rt.newstarts.cn

[B16] 卫语句：不满足条件提前返回
来源：http://td.huixinmuqiang.cn

Py:   if not data: return
来源：http://el.yuexingan06.cn

PHP:  if (!$data) { return; }
来源：http://ib.colortex.cn

JS:   if (!data) return;
来源：http://nc.shxzukj.cn

TS:   if (!data) return;
来源：http://hu.newstarts.cn

Java: if (data == null) return;
来源：http://mp.jianghongdianzi.cn

Go:   if data == nil { return }
来源：http://xi.nszjky.cn

Ruby: return if data.nil?
来源：http://wj.huanxung.cn

C#:   if (data == null) return;
来源：http://xn.shxzskj.cn

================================================================================
来源：http://wt.hnjuh.cn

C. 函数与作用域
来源：http://yh.nszjky.cn

================================================================================
来源：http://js.jctech888.com.cn

[C01] 定义函数
来源：http://rb.gzmigu.cn

Py:   def add(a, b): return a + b
来源：http://og.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wx.shxzukj.cn

JS:   function add(a, b) { return a + b; }
来源：http://ti.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mv.shxzukj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zc.gzmigu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qb.bookmarksfly.cn

Ruby: def add(a, b); a + b; end
来源：http://xd.gzmigu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cw.hahajie.cn

[C02] 默认参数
来源：http://kb.yuexingan06.cn

Py:   def greet(name="World"): return name
来源：http://fe.asd995.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xo.colortex.cn

JS:   function greet(name = "World") { return name; }
来源：http://uy.yuexingan06.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hm.hnjuh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dg.szxytkj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pf.gzmigu.cn

Ruby: def greet(name = "World") = name
来源：http://hk.szsharing.cn

C#:   string Greet(string name = "World") => name;
来源：http://yj.huixinmuqiang.cn

[C03] 可变参数
来源：http://mb.hnjuh.cn

Py:   def total(*args): return sum(args)
来源：http://rw.9csxet.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tp.gzmigu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zi.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ap.colortex.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jb.wgjwhj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://up.yuexingan06.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rs.huanxung.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hh.wgjwhj.cn

[C04] 命名参数 / 关键字参数
来源：http://vi.shxzskj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uq.muxihuayi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cv.shxzukj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jb.bookmarksfly.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sk.hahajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://ps.nszjky.cn

Go:   // 无：用配置结构体参数
来源：http://zx.colortex.cn

Ruby: f(a: 1, b: 2)
来源：http://bl.9csxet.cn

C#:   f(a: 1, b: 2)
来源：http://bv.bjjhwx.cn

[C05] 返回多个值
来源：http://me.wgjwhj.cn


<!-- 参考信息 -->