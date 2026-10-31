代发 wailian999

[A14] 注释写法
来源：http://dz.hahajie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ed.9csxet.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://nt.newstarts.cn

JS:   // 单行；/* 多行 */
来源：http://qk.asd995.cn

TS:   // 单行；/* 多行 */
来源：http://dd.huixinmuqiang.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ow.jctech888.com.cn

Go:   // 单行；/* 多行 */
来源：http://kc.jianghongdianzi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://yy.hnjuh.cn

C#:   // 单行；/* 多行 */
来源：http://cs.bookmarksfly.cn

[A15] 空值判断与默认值
来源：http://ai.9csxet.cn

Py:   value = data or "默认值"
来源：http://lc.wgjwhj.cn

PHP:  $value = $data ?? "默认值";
来源：http://mp.nszjky.cn

JS:   const value = data ?? "默认值";
来源：http://re.gzmigu.cn

TS:   const value = data ?? "默认值";
来源：http://mj.colortex.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ns.nicolike.cn

Go:   if data == "" { data = "默认值" }
来源：http://wu.shxzskj.cn

Ruby: value = data || "默认值"
来源：http://ak.huixiangedu.cn

C#:   var value = data ?? "默认值";
来源：http://fh.jianghongdianzi.cn

[A16] 真假值判断规则
来源：http://ah.wgjwhj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mv.chemitech.net.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fi.nszjky.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yn.gzmigu.cn

TS:   if (!x) {}
来源：http://hm.panjiajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wt.9csxet.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kc.wgjwhj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://al.nszjky.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rc.huixiangedu.cn

[A17] 位运算
来源：http://xx.huixiangedu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oo.jctech888.com.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vq.lnxyls.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fc.yuexingan06.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tl.colortex.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qw.panjiajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kz.asd995.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xm.yuntaijiaju.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://js.wgjwhj.cn

[A18] 字符与 ASCII 码互转
来源：http://qj.hahajie.cn

Py:   ord("A"); chr(65)
来源：http://uc.jianghongdianzi.cn

PHP:  ord("A"); chr(65)
来源：http://uj.yuexingan06.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://de.huanxung.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cu.huanxung.cn

Java: (int) 'A'; (char) 65
来源：http://zk.shxzskj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fl.yuntaijiaju.cn

Ruby: "A".ord; 65.chr
来源：http://je.hahajie.cn

C#:   (int)'A'; (char)65
来源：http://jr.szxytkj.cn

[A19] 交换两个变量
来源：http://uk.bookmarksfly.cn

Py:   a, b = b, a
来源：http://fk.szxytkj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://xl.bookmarksfly.cn

JS:   [a, b] = [b, a];
来源：http://wo.szxytkj.cn

TS:   [a, b] = [b, a];
来源：http://ux.szxytkj.cn

Java: int t = a; a = b; b = t;
来源：http://xj.yuexingan06.cn

Go:   a, b = b, a
来源：http://tb.bookmarksfly.cn

Ruby: a, b = b, a
来源：http://ph.521024.cn

C#:   (a, b) = (b, a);
来源：http://db.bjjhwx.cn

[A20] 读取标准输入
来源：http://ws.colortex.cn

Py:   name = input("请输入：")
来源：http://eh.9csxet.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://iu.shtwfgs.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hq.huanxung.cn

TS:   // Node.js：readline 模块
来源：http://xn.shxzskj.cn

Java: new Scanner(System.in).nextLine()
来源：http://pn.hnjuh.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cd.521024.cn

Ruby: gets.chomp
来源：http://yv.jctech888.com.cn

C#:   Console.ReadLine();
来源：http://dy.wgjwhj.cn

[A21] 保留指定小数位输出
来源：http://od.wgjwhj.cn

Py:   f"{3.14159:.2f}"
来源：http://hj.muxihuayi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ew.hnjuh.cn

JS:   (3.14159).toFixed(2)
来源：http://wj.wgjwhj.cn

TS:   (3.14159).toFixed(2)
来源：http://nz.colortex.cn

Java: String.format("%.2f", 3.14159)
来源：http://tt.jctech888.com.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wp.chemitech.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://uu.muxihuayi.cn

C#:   3.14159.ToString("F2")
来源：http://dz.9csxet.cn

[A22] 获取字符串长度
来源：http://mm.jctech888.com.cn

Py:   len(s)
来源：http://bi.hahajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://io.huanxung.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zb.asd995.cn

TS:   s.length
来源：http://zi.colortex.cn

Java: s.length()
来源：http://za.huixiangedu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kp.yuexingan06.cn

Ruby: s.length
来源：http://xl.chemitech.net.cn

C#:   s.Length
来源：http://ob.nicolike.cn

[A23] 大小写转换
来源：http://kq.panjiajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ie.wgjwhj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lr.hahajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dt.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://eu.yuntaijiaju.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wd.muxihuayi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lu.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yn.nicolike.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qo.shxzukj.cn

[A24] 去除首尾空白
来源：http://fv.huanxung.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tp.huanxung.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rx.lnxyls.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vu.9csxet.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mb.huixiangedu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cs.chemitech.net.cn

Go:   strings.TrimSpace(s)
来源：http://nt.nicolike.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://su.521024.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yy.shxzskj.cn

[A25] 字符串比较
来源：http://hh.huanxung.cn

Py:   s1 == s2; s1 != s2
来源：http://gu.panjiajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pr.521024.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://up.gzmigu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tw.muxihuayi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ms.jctech888.com.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pz.muxihuayi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hl.9csxet.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ks.521024.cn

[A26] 类型转换总览
来源：http://dg.yuexingan06.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fy.hnjuh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hj.huixinmuqiang.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ez.colortex.cn

TS:   Number() String() Boolean() x as number
来源：http://cz.shxzukj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ak.chemitech.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xj.521024.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://uc.huixinmuqiang.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ck.hnjuh.cn

================================================================================
来源：http://uu.9csxet.cn

B. 流程控制
来源：http://pk.bookmarksfly.cn

================================================================================
来源：http://io.hnjuh.cn

[B01] 条件判断 if / else
来源：http://vz.chemitech.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jw.bjjhwx.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jo.huixinmuqiang.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gp.colortex.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zn.szxytkj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://br.muxihuayi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xz.gzmigu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fn.yuexingan06.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xa.szsharing.cn

[B02] 多分支 else if / elif
来源：http://wi.nicolike.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mh.shxzukj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lv.chemitech.net.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ee.gzmigu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qt.panjiajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nd.haigaiapp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ta.shxzskj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gj.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iy.chemitech.net.cn

[B03] switch / match / case
来源：http://ym.9csxet.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ol.huixinmuqiang.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ak.szxytkj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://at.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pr.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ld.jctech888.com.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dg.muxihuayi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ya.jianghongdianzi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mm.521024.cn

[B04] for 计数循环
来源：http://hf.asd995.cn

Py:   for i in range(10): print(i)
来源：http://ww.newstarts.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kh.hnjuh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wa.yuntaijiaju.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://am.gzmigu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://op.lnxyls.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://io.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://hz.shtwfgs.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lu.jctech888.com.cn

[B05] 遍历数组 / 列表
来源：http://yd.jctech888.com.cn

Py:   for item in arr: print(item)
来源：http://ca.huixiangedu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fq.521024.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dt.hnjuh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dn.hnjuh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xr.colortex.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tw.szxytkj.cn

Ruby: arr.each { |item| puts item }
来源：http://sd.asd995.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ca.asd995.cn

[B06] 遍历字典 / 对象
来源：http://dv.yuntaijiaju.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ef.lnxyls.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rv.panjiajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sf.shxzukj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ja.hahajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bk.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ip.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ey.bookmarksfly.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ar.shxzskj.cn

[B07] while 循环
来源：http://wd.colortex.cn

Py:   while i < 10: i += 1
来源：http://po.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kc.szsharing.cn

JS:   while (i < 10) { i++; }
来源：http://gg.asd995.cn

TS:   while (i < 10) { i++; }
来源：http://uy.yuntaijiaju.cn

Java: while (i < 10) { i++; }
来源：http://it.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cf.521024.cn

Ruby: while i < 10; i += 1; end
来源：http://cj.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://zv.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://zg.szsharing.cn

Py:   # 无 do-while：用 while True + break
来源：http://de.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ov.szxytkj.cn

JS:   do { i++; } while (i < 10);
来源：http://sk.szxytkj.cn

TS:   do { i++; } while (i < 10);
来源：http://zc.shtwfgs.cn

Java: do { i++; } while (i < 10);
来源：http://vh.521024.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vm.9csxet.cn

Ruby: begin; i += 1; end while i < 10
来源：http://sp.szsharing.cn

C#:   do { i++; } while (i < 10);
来源：http://iv.bookmarksfly.cn

[B09] break 与 continue
来源：http://hr.colortex.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ok.hnjuh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ux.huixinmuqiang.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dy.chemitech.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ii.wgjwhj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ni.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ic.wgjwhj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nm.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fc.szsharing.cn

[B10] 遍历同时拿索引
来源：http://iu.9csxet.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fs.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://id.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wo.asd995.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://su.huanxung.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ba.hnjuh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wm.bjjhwx.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ps.szsharing.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://za.haigaiapp.cn

[B11] 生成数字序列 / 区间
来源：http://ib.lnxyls.cn

Py:   list(range(0, 10, 2))
来源：http://vi.colortex.cn

PHP:  range(0, 10, 2);
来源：http://ub.szxytkj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://br.lnxyls.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ee.muxihuayi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ve.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bw.shtwfgs.cn

Ruby: (0...10).step(2).to_a
来源：http://jc.chemitech.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ob.huixiangedu.cn

[B12] 跳出多层循环
来源：http://cq.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xw.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cc.huixiangedu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ub.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wr.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ow.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ys.yuexingan06.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://il.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lh.szxytkj.cn

[B13] 判断是否为数字
来源：http://ex.jianghongdianzi.cn

Py:   isinstance(x, (int, float))
来源：http://xn.gzmigu.cn

PHP:  is_numeric($x)
来源：http://gn.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://be.szxytkj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lv.gzmigu.cn

Java: x instanceof Number
来源：http://uz.panjiajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kj.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://ac.shtwfgs.cn

C#:   x is int or double or decimal
来源：http://nz.wgjwhj.cn

[B14] 判断值是否在集合内
来源：http://hy.yuexingan06.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://aw.huixiangedu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nv.shxzskj.cn

JS:   [1, 2, 3].includes(x)
来源：http://gq.nicolike.cn

TS:   [1, 2, 3].includes(x)
来源：http://fa.panjiajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://db.hnjuh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sq.nicolike.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xt.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://on.521024.cn

[B15] 布尔运算与取反
来源：http://kc.shxzukj.cn

Py:   a and b or not c
来源：http://nv.yuntaijiaju.cn

PHP:  $a && $b || !$c
来源：http://xl.hnjuh.cn

JS:   a && b || !c
来源：http://dc.bookmarksfly.cn

TS:   a && b || !c
来源：http://qf.huixinmuqiang.cn

Java: a && b || !c
来源：http://mr.yuntaijiaju.cn

Go:   a && b || !c
来源：http://uh.shtwfgs.cn

Ruby: a && b || !c
来源：http://yc.chemitech.net.cn

C#:   a && b || !c
来源：http://oe.asd995.cn

[B16] 卫语句：不满足条件提前返回
来源：http://go.nszjky.cn

Py:   if not data: return
来源：http://hy.huanxung.cn

PHP:  if (!$data) { return; }
来源：http://kk.szxytkj.cn

JS:   if (!data) return;
来源：http://xx.szxytkj.cn

TS:   if (!data) return;
来源：http://ub.hahajie.cn

Java: if (data == null) return;
来源：http://ob.bookmarksfly.cn

Go:   if data == nil { return }
来源：http://ih.chemitech.net.cn

Ruby: return if data.nil?
来源：http://it.bjjhwx.cn

C#:   if (data == null) return;
来源：http://ce.szsharing.cn

================================================================================
来源：http://bq.9csxet.cn

C. 函数与作用域
来源：http://rn.hahajie.cn

================================================================================
来源：http://hx.huixinmuqiang.cn

[C01] 定义函数
来源：http://ce.asd995.cn

Py:   def add(a, b): return a + b
来源：http://fl.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kh.521024.cn

JS:   function add(a, b) { return a + b; }
来源：http://fk.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aw.521024.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xa.hahajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mr.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://re.muxihuayi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jv.lnxyls.cn

[C02] 默认参数
来源：http://hs.muxihuayi.cn

Py:   def greet(name="World"): return name
来源：http://db.wgjwhj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tq.huanxung.cn

JS:   function greet(name = "World") { return name; }
来源：http://es.muxihuayi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wk.gzmigu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ni.panjiajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vu.wgjwhj.cn

Ruby: def greet(name = "World") = name
来源：http://fd.nszjky.cn

C#:   string Greet(string name = "World") => name;
来源：http://vt.wgjwhj.cn

[C03] 可变参数
来源：http://kt.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://jj.521024.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bz.huanxung.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vv.yuexingan06.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sg.jianghongdianzi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tc.gzmigu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bx.shtwfgs.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jf.shxzukj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ok.nicolike.cn

[C04] 命名参数 / 关键字参数
来源：http://zc.shxzskj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vu.lnxyls.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sf.chemitech.net.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wx.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tg.nicolike.cn

Java: // 无：用 Builder 模式或 record
来源：http://ya.muxihuayi.cn


<!-- 参考信息 -->