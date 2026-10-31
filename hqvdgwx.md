代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://dv.hahajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://an.wgjwhj.cn

Go:   // 单行；/* 多行 */
来源：http://ea.hnjuh.cn

Ruby: # 单行；=begin 多行 =end
来源：http://yf.jctech888.com.cn

C#:   // 单行；/* 多行 */
来源：http://jp.colortex.cn

[A15] 空值判断与默认值
来源：http://ec.chemitech.net.cn

Py:   value = data or "默认值"
来源：http://qx.huixiangedu.cn

PHP:  $value = $data ?? "默认值";
来源：http://tq.asd995.cn

JS:   const value = data ?? "默认值";
来源：http://xn.panjiajie.cn

TS:   const value = data ?? "默认值";
来源：http://ef.yuexingan06.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wz.bjjhwx.cn

Go:   if data == "" { data = "默认值" }
来源：http://ma.huanxung.cn

Ruby: value = data || "默认值"
来源：http://eg.jctech888.com.cn

C#:   var value = data ?? "默认值";
来源：http://ma.newstarts.cn

[A16] 真假值判断规则
来源：http://yt.muxihuayi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ii.wgjwhj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mr.huanxung.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vc.chemitech.net.cn

TS:   if (!x) {}
来源：http://ep.yuntaijiaju.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gx.521024.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zd.wgjwhj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vw.szsharing.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vh.jctech888.com.cn

[A17] 位运算
来源：http://nn.szxytkj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bu.521024.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qq.jianghongdianzi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wb.gzmigu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://se.panjiajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yt.shtwfgs.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pr.asd995.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rn.haigaiapp.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tg.gzmigu.cn

[A18] 字符与 ASCII 码互转
来源：http://fj.muxihuayi.cn

Py:   ord("A"); chr(65)
来源：http://io.panjiajie.cn

PHP:  ord("A"); chr(65)
来源：http://bg.shxzskj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ec.bjjhwx.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gc.huanxung.cn

Java: (int) 'A'; (char) 65
来源：http://sh.szxytkj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fj.yuexingan06.cn

Ruby: "A".ord; 65.chr
来源：http://da.yuexingan06.cn

C#:   (int)'A'; (char)65
来源：http://qw.jianghongdianzi.cn

[A19] 交换两个变量
来源：http://jx.shtwfgs.cn

Py:   a, b = b, a
来源：http://tt.hahajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://os.jctech888.com.cn

JS:   [a, b] = [b, a];
来源：http://tg.yuexingan06.cn

TS:   [a, b] = [b, a];
来源：http://jk.9csxet.cn

Java: int t = a; a = b; b = t;
来源：http://qp.bjjhwx.cn

Go:   a, b = b, a
来源：http://ks.muxihuayi.cn

Ruby: a, b = b, a
来源：http://kf.hnjuh.cn

C#:   (a, b) = (b, a);
来源：http://xj.yuntaijiaju.cn

[A20] 读取标准输入
来源：http://xx.bookmarksfly.cn

Py:   name = input("请输入：")
来源：http://ub.hahajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qu.wgjwhj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ga.nszjky.cn

TS:   // Node.js：readline 模块
来源：http://xk.jctech888.com.cn

Java: new Scanner(System.in).nextLine()
来源：http://sr.muxihuayi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jr.colortex.cn

Ruby: gets.chomp
来源：http://ey.nszjky.cn

C#:   Console.ReadLine();
来源：http://hu.haigaiapp.cn

[A21] 保留指定小数位输出
来源：http://mk.bookmarksfly.cn

Py:   f"{3.14159:.2f}"
来源：http://te.haigaiapp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://re.panjiajie.cn

JS:   (3.14159).toFixed(2)
来源：http://tp.huixiangedu.cn

TS:   (3.14159).toFixed(2)
来源：http://jm.szsharing.cn

Java: String.format("%.2f", 3.14159)
来源：http://wz.hnjuh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xy.muxihuayi.cn

Ruby: format("%.2f", 3.14159)
来源：http://we.521024.cn

C#:   3.14159.ToString("F2")
来源：http://oy.nicolike.cn

[A22] 获取字符串长度
来源：http://wg.9csxet.cn

Py:   len(s)
来源：http://vr.chemitech.net.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://oo.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gx.521024.cn

TS:   s.length
来源：http://je.shxzskj.cn

Java: s.length()
来源：http://dy.521024.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pj.bjjhwx.cn

Ruby: s.length
来源：http://qx.hnjuh.cn

C#:   s.Length
来源：http://yp.chemitech.net.cn

[A23] 大小写转换
来源：http://bf.panjiajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vw.hnjuh.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ei.muxihuayi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ca.lnxyls.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://uv.shxzskj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://db.colortex.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pw.bjjhwx.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fz.jianghongdianzi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qq.szxytkj.cn

[A24] 去除首尾空白
来源：http://qj.yuexingan06.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sp.colortex.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wx.szsharing.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gb.haigaiapp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://me.huixinmuqiang.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sp.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://sh.9csxet.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rj.lnxyls.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ka.521024.cn

[A25] 字符串比较
来源：http://bs.szxytkj.cn

Py:   s1 == s2; s1 != s2
来源：http://pz.huixinmuqiang.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zf.shtwfgs.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qq.szsharing.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vy.asd995.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sr.jianghongdianzi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lf.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://eo.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xe.huixinmuqiang.cn

[A26] 类型转换总览
来源：http://wp.yuexingan06.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://md.muxihuayi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://si.huixinmuqiang.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zs.bookmarksfly.cn

TS:   Number() String() Boolean() x as number
来源：http://kt.szsharing.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jo.hahajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ss.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://py.nicolike.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xn.panjiajie.cn

================================================================================
来源：http://df.bookmarksfly.cn

B. 流程控制
来源：http://pv.huixinmuqiang.cn

================================================================================
来源：http://vi.nicolike.cn

[B01] 条件判断 if / else
来源：http://qj.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zz.shtwfgs.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ja.yuntaijiaju.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jx.newstarts.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kd.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bt.huixiangedu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qa.shtwfgs.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://si.huanxung.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kh.muxihuayi.cn

[B02] 多分支 else if / elif
来源：http://sg.huanxung.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mn.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bo.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bq.shtwfgs.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ag.yuexingan06.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://os.szxytkj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ox.gzmigu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://og.shxzskj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kv.9csxet.cn

[B03] switch / match / case
来源：http://pp.hnjuh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yj.panjiajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://so.shxzukj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hd.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://np.9csxet.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://po.bookmarksfly.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dr.huixinmuqiang.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pf.bookmarksfly.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jn.newstarts.cn

[B04] for 计数循环
来源：http://ig.bookmarksfly.cn

Py:   for i in range(10): print(i)
来源：http://rg.wgjwhj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wr.muxihuayi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ti.muxihuayi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cg.huanxung.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jy.chemitech.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ry.haigaiapp.cn

Ruby: 10.times { |i| puts i }
来源：http://mp.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yb.hahajie.cn

[B05] 遍历数组 / 列表
来源：http://sw.muxihuayi.cn

Py:   for item in arr: print(item)
来源：http://tc.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ar.jianghongdianzi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ay.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://of.haigaiapp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nu.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rr.bookmarksfly.cn

Ruby: arr.each { |item| puts item }
来源：http://kt.chemitech.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ly.yuntaijiaju.cn

[B06] 遍历字典 / 对象
来源：http://at.asd995.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lq.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qf.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ha.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pw.chemitech.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gi.9csxet.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xb.bjjhwx.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sd.shxzskj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pg.9csxet.cn

[B07] while 循环
来源：http://vl.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://ex.shxzskj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rc.nicolike.cn

JS:   while (i < 10) { i++; }
来源：http://sh.yuexingan06.cn

TS:   while (i < 10) { i++; }
来源：http://aa.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://xl.yuexingan06.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sv.bjjhwx.cn

Ruby: while i < 10; i += 1; end
来源：http://gg.szxytkj.cn

C#:   while (i < 10) { i++; }
来源：http://ha.asd995.cn

[B08] do-while（至少执行一次）
来源：http://sx.nicolike.cn

Py:   # 无 do-while：用 while True + break
来源：http://pf.lnxyls.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kq.hnjuh.cn

JS:   do { i++; } while (i < 10);
来源：http://zy.huixiangedu.cn

TS:   do { i++; } while (i < 10);
来源：http://cc.bookmarksfly.cn

Java: do { i++; } while (i < 10);
来源：http://uf.asd995.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ny.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fn.521024.cn

C#:   do { i++; } while (i < 10);
来源：http://cb.huixiangedu.cn

[B09] break 与 continue
来源：http://zq.panjiajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wo.panjiajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uh.jianghongdianzi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wf.bookmarksfly.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fe.colortex.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tk.9csxet.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zp.huanxung.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wp.hahajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yl.muxihuayi.cn

[B10] 遍历同时拿索引
来源：http://my.chemitech.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://an.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://by.jianghongdianzi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cf.gzmigu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://un.wgjwhj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qe.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://eg.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ww.yuntaijiaju.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hp.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://mc.shtwfgs.cn

Py:   list(range(0, 10, 2))
来源：http://pn.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://pp.9csxet.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xw.bjjhwx.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fn.shxzukj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wm.jctech888.com.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qz.newstarts.cn

Ruby: (0...10).step(2).to_a
来源：http://dq.shxzskj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wg.hahajie.cn

[B12] 跳出多层循环
来源：http://da.szsharing.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://oy.bjjhwx.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://op.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ni.newstarts.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://oj.szsharing.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ke.huixinmuqiang.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://av.shtwfgs.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ma.chemitech.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jl.wgjwhj.cn

[B13] 判断是否为数字
来源：http://jb.chemitech.net.cn

Py:   isinstance(x, (int, float))
来源：http://ft.szsharing.cn

PHP:  is_numeric($x)
来源：http://mj.gzmigu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nm.hahajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qz.nicolike.cn

Java: x instanceof Number
来源：http://uo.hahajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xf.asd995.cn

Ruby: x.is_a?(Numeric)
来源：http://os.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://df.asd995.cn

[B14] 判断值是否在集合内
来源：http://qs.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ro.huixinmuqiang.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ct.colortex.cn

JS:   [1, 2, 3].includes(x)
来源：http://lq.gzmigu.cn

TS:   [1, 2, 3].includes(x)
来源：http://cp.nszjky.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://er.hahajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cg.asd995.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qv.bookmarksfly.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ud.gzmigu.cn

[B15] 布尔运算与取反
来源：http://cy.colortex.cn

Py:   a and b or not c
来源：http://ik.huanxung.cn

PHP:  $a && $b || !$c
来源：http://nu.yuexingan06.cn

JS:   a && b || !c
来源：http://mz.muxihuayi.cn

TS:   a && b || !c
来源：http://bh.shtwfgs.cn

Java: a && b || !c
来源：http://bq.yuntaijiaju.cn

Go:   a && b || !c
来源：http://so.9csxet.cn

Ruby: a && b || !c
来源：http://ob.bjjhwx.cn

C#:   a && b || !c
来源：http://jw.shtwfgs.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ax.521024.cn

Py:   if not data: return
来源：http://yj.nicolike.cn

PHP:  if (!$data) { return; }
来源：http://dp.nicolike.cn

JS:   if (!data) return;
来源：http://ii.muxihuayi.cn

TS:   if (!data) return;
来源：http://xb.hahajie.cn

Java: if (data == null) return;
来源：http://rl.9csxet.cn

Go:   if data == nil { return }
来源：http://la.panjiajie.cn

Ruby: return if data.nil?
来源：http://ec.jctech888.com.cn

C#:   if (data == null) return;
来源：http://yo.jctech888.com.cn

================================================================================
来源：http://wn.newstarts.cn

C. 函数与作用域
来源：http://vy.shtwfgs.cn

================================================================================
来源：http://yo.yuexingan06.cn

[C01] 定义函数
来源：http://na.szsharing.cn

Py:   def add(a, b): return a + b
来源：http://ct.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wt.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://oi.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mv.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://uc.colortex.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ny.hahajie.cn

Ruby: def add(a, b); a + b; end
来源：http://vh.huixiangedu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ks.asd995.cn

[C02] 默认参数
来源：http://uo.muxihuayi.cn

Py:   def greet(name="World"): return name
来源：http://hc.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://sn.szxytkj.cn

JS:   function greet(name = "World") { return name; }
来源：http://wn.gzmigu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dt.shxzukj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://it.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ii.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://iz.hahajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://ol.wgjwhj.cn

[C03] 可变参数
来源：http://xi.yuntaijiaju.cn

Py:   def total(*args): return sum(args)
来源：http://al.huixinmuqiang.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://in.shxzskj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://go.huixinmuqiang.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uu.huixiangedu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ge.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wp.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://of.szxytkj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://se.wgjwhj.cn

[C04] 命名参数 / 关键字参数
来源：http://bk.bjjhwx.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mr.szsharing.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tk.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zi.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ad.lnxyls.cn

Java: // 无：用 Builder 模式或 record
来源：http://ot.szsharing.cn

Go:   // 无：用配置结构体参数
来源：http://av.jianghongdianzi.cn

Ruby: f(a: 1, b: 2)
来源：http://la.yuntaijiaju.cn

C#:   f(a: 1, b: 2)
来源：http://xi.szxytkj.cn

[C05] 返回多个值
来源：http://bn.shtwfgs.cn


<!-- 参考信息 -->