代发 wailian999

Ruby: value = data || "默认值"
来源：http://zp.asd995.cn

C#:   var value = data ?? "默认值";
来源：http://vu.shxzukj.cn

[A16] 真假值判断规则
来源：http://jf.colortex.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://sq.asd995.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://sh.huixinmuqiang.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zm.yuntaijiaju.cn

TS:   if (!x) {}
来源：http://uf.521024.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://js.yuntaijiaju.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zd.asd995.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lv.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xo.gzmigu.cn

[A17] 位运算
来源：http://sy.hahajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wy.hnjuh.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mi.newstarts.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tq.asd995.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zi.jctech888.com.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qm.muxihuayi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ym.haigaiapp.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ky.gzmigu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vy.huixiangedu.cn

[A18] 字符与 ASCII 码互转
来源：http://mr.gzmigu.cn

Py:   ord("A"); chr(65)
来源：http://kn.shtwfgs.cn

PHP:  ord("A"); chr(65)
来源：http://qd.huixiangedu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ns.shxzskj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oj.huanxung.cn

Java: (int) 'A'; (char) 65
来源：http://pe.newstarts.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ud.9csxet.cn

Ruby: "A".ord; 65.chr
来源：http://lk.yuntaijiaju.cn

C#:   (int)'A'; (char)65
来源：http://mm.huixiangedu.cn

[A19] 交换两个变量
来源：http://uy.shxzukj.cn

Py:   a, b = b, a
来源：http://qq.muxihuayi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://wu.huanxung.cn

JS:   [a, b] = [b, a];
来源：http://xp.huixinmuqiang.cn

TS:   [a, b] = [b, a];
来源：http://ls.colortex.cn

Java: int t = a; a = b; b = t;
来源：http://ao.chemitech.net.cn

Go:   a, b = b, a
来源：http://eq.szxytkj.cn

Ruby: a, b = b, a
来源：http://nu.yuexingan06.cn

C#:   (a, b) = (b, a);
来源：http://tm.9csxet.cn

[A20] 读取标准输入
来源：http://mi.wgjwhj.cn

Py:   name = input("请输入：")
来源：http://bq.yuntaijiaju.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://uc.hahajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ek.lnxyls.cn

TS:   // Node.js：readline 模块
来源：http://mr.panjiajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://ar.lnxyls.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dp.shxzukj.cn

Ruby: gets.chomp
来源：http://no.newstarts.cn

C#:   Console.ReadLine();
来源：http://jb.szsharing.cn

[A21] 保留指定小数位输出
来源：http://wc.bjjhwx.cn

Py:   f"{3.14159:.2f}"
来源：http://cj.panjiajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ql.szxytkj.cn

JS:   (3.14159).toFixed(2)
来源：http://kr.yuexingan06.cn

TS:   (3.14159).toFixed(2)
来源：http://gt.huanxung.cn

Java: String.format("%.2f", 3.14159)
来源：http://wu.huanxung.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xh.huixiangedu.cn

Ruby: format("%.2f", 3.14159)
来源：http://ft.panjiajie.cn

C#:   3.14159.ToString("F2")
来源：http://ct.shxzskj.cn

[A22] 获取字符串长度
来源：http://pm.bjjhwx.cn

Py:   len(s)
来源：http://us.shtwfgs.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pb.jianghongdianzi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tn.yuntaijiaju.cn

TS:   s.length
来源：http://ah.jianghongdianzi.cn

Java: s.length()
来源：http://zl.muxihuayi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zm.chemitech.net.cn

Ruby: s.length
来源：http://ym.shxzukj.cn

C#:   s.Length
来源：http://tp.szxytkj.cn

[A23] 大小写转换
来源：http://he.lnxyls.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hk.newstarts.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yv.muxihuayi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rj.haigaiapp.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pm.newstarts.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mm.nszjky.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sd.hahajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hn.yuntaijiaju.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://kj.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://vb.yuexingan06.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dn.shxzskj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vl.hnjuh.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zy.haigaiapp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tj.nszjky.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pd.nszjky.cn

Go:   strings.TrimSpace(s)
来源：http://ve.shxzskj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bj.huixinmuqiang.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qq.jianghongdianzi.cn

[A25] 字符串比较
来源：http://pi.nszjky.cn

Py:   s1 == s2; s1 != s2
来源：http://ba.nszjky.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uu.szsharing.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hk.nicolike.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pl.bookmarksfly.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nj.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ju.shxzukj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lc.bookmarksfly.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lr.shxzukj.cn

[A26] 类型转换总览
来源：http://ly.yuntaijiaju.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://iq.newstarts.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ic.nszjky.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yd.gzmigu.cn

TS:   Number() String() Boolean() x as number
来源：http://xv.hahajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sq.asd995.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ym.shxzukj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hk.nszjky.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gq.szxytkj.cn

================================================================================
来源：http://ki.panjiajie.cn

B. 流程控制
来源：http://rw.yuntaijiaju.cn

================================================================================
来源：http://kl.huixiangedu.cn

[B01] 条件判断 if / else
来源：http://yq.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://is.hahajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ya.newstarts.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ej.szxytkj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nw.colortex.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://nr.panjiajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wn.lnxyls.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nh.huixinmuqiang.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://aj.szxytkj.cn

[B02] 多分支 else if / elif
来源：http://cg.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ch.haigaiapp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tt.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mk.asd995.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wc.jianghongdianzi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jp.huixinmuqiang.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lq.yuexingan06.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wy.hnjuh.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ew.asd995.cn

[B03] switch / match / case
来源：http://ov.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bb.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lw.haigaiapp.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bv.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://la.shxzskj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ei.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yg.panjiajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://io.hnjuh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yl.9csxet.cn

[B04] for 计数循环
来源：http://as.jctech888.com.cn

Py:   for i in range(10): print(i)
来源：http://bs.bjjhwx.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://op.muxihuayi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ll.bjjhwx.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ld.gzmigu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ww.yuexingan06.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rz.jianghongdianzi.cn

Ruby: 10.times { |i| puts i }
来源：http://xd.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kd.szsharing.cn

[B05] 遍历数组 / 列表
来源：http://wx.bjjhwx.cn

Py:   for item in arr: print(item)
来源：http://zk.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ic.asd995.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rb.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wx.shtwfgs.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yl.huixinmuqiang.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nv.521024.cn

Ruby: arr.each { |item| puts item }
来源：http://uv.shxzskj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pb.jctech888.com.cn

[B06] 遍历字典 / 对象
来源：http://an.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vu.huixinmuqiang.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jh.nszjky.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kk.wgjwhj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cn.huanxung.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bf.jctech888.com.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zn.nicolike.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qa.bookmarksfly.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://up.9csxet.cn

[B07] while 循环
来源：http://ch.chemitech.net.cn

Py:   while i < 10: i += 1
来源：http://se.huanxung.cn

PHP:  while ($i < 10) { $i++; }
来源：http://aj.nszjky.cn

JS:   while (i < 10) { i++; }
来源：http://ki.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://lf.shxzukj.cn

Java: while (i < 10) { i++; }
来源：http://ng.hahajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wy.asd995.cn

Ruby: while i < 10; i += 1; end
来源：http://sv.lnxyls.cn

C#:   while (i < 10) { i++; }
来源：http://vn.hahajie.cn

[B08] do-while（至少执行一次）
来源：http://sg.hnjuh.cn

Py:   # 无 do-while：用 while True + break
来源：http://ar.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zx.jianghongdianzi.cn

JS:   do { i++; } while (i < 10);
来源：http://ci.bjjhwx.cn

TS:   do { i++; } while (i < 10);
来源：http://bc.9csxet.cn

Java: do { i++; } while (i < 10);
来源：http://xs.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gs.szxytkj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ju.lnxyls.cn

C#:   do { i++; } while (i < 10);
来源：http://jd.colortex.cn

[B09] break 与 continue
来源：http://yk.shtwfgs.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dk.bjjhwx.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ot.szsharing.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://st.chemitech.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zt.lnxyls.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vc.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gc.jianghongdianzi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ze.yuexingan06.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qv.szsharing.cn

[B10] 遍历同时拿索引
来源：http://sv.newstarts.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cj.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://db.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sa.bookmarksfly.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vl.muxihuayi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hw.szsharing.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jy.shtwfgs.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ms.bjjhwx.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ba.nszjky.cn

[B11] 生成数字序列 / 区间
来源：http://rl.gzmigu.cn

Py:   list(range(0, 10, 2))
来源：http://si.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://hp.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bl.nicolike.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fc.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dp.521024.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hl.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://yx.lnxyls.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ej.shxzukj.cn

[B12] 跳出多层循环
来源：http://og.colortex.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pr.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mh.9csxet.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bt.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ic.bjjhwx.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tu.panjiajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lm.szxytkj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sb.shtwfgs.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zd.jianghongdianzi.cn

[B13] 判断是否为数字
来源：http://jd.9csxet.cn

Py:   isinstance(x, (int, float))
来源：http://pw.colortex.cn

PHP:  is_numeric($x)
来源：http://ah.gzmigu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lw.lnxyls.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qu.szxytkj.cn

Java: x instanceof Number
来源：http://nk.gzmigu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fa.huixinmuqiang.cn

Ruby: x.is_a?(Numeric)
来源：http://jp.nicolike.cn

C#:   x is int or double or decimal
来源：http://tv.huixinmuqiang.cn

[B14] 判断值是否在集合内
来源：http://jf.nszjky.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ie.jianghongdianzi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uo.hnjuh.cn

JS:   [1, 2, 3].includes(x)
来源：http://os.chemitech.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://wj.newstarts.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gv.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mi.lnxyls.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dh.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jj.shxzukj.cn

[B15] 布尔运算与取反
来源：http://ta.bjjhwx.cn

Py:   a and b or not c
来源：http://vz.gzmigu.cn

PHP:  $a && $b || !$c
来源：http://df.asd995.cn

JS:   a && b || !c
来源：http://yh.shtwfgs.cn

TS:   a && b || !c
来源：http://ze.szsharing.cn

Java: a && b || !c
来源：http://kx.lnxyls.cn

Go:   a && b || !c
来源：http://ly.yuntaijiaju.cn

Ruby: a && b || !c
来源：http://xo.hnjuh.cn

C#:   a && b || !c
来源：http://be.521024.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ku.shxzskj.cn

Py:   if not data: return
来源：http://ik.shxzukj.cn

PHP:  if (!$data) { return; }
来源：http://pq.panjiajie.cn

JS:   if (!data) return;
来源：http://bg.jianghongdianzi.cn

TS:   if (!data) return;
来源：http://eu.szxytkj.cn

Java: if (data == null) return;
来源：http://zd.muxihuayi.cn

Go:   if data == nil { return }
来源：http://av.colortex.cn

Ruby: return if data.nil?
来源：http://nu.gzmigu.cn

C#:   if (data == null) return;
来源：http://eo.asd995.cn

================================================================================
来源：http://rh.yuntaijiaju.cn

C. 函数与作用域
来源：http://wb.newstarts.cn

================================================================================
来源：http://wn.shtwfgs.cn

[C01] 定义函数
来源：http://zf.newstarts.cn

Py:   def add(a, b): return a + b
来源：http://xh.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ld.chemitech.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://yn.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bs.shtwfgs.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tq.521024.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ri.yuexingan06.cn

Ruby: def add(a, b); a + b; end
来源：http://cy.jianghongdianzi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hv.haigaiapp.cn

[C02] 默认参数
来源：http://ef.jianghongdianzi.cn

Py:   def greet(name="World"): return name
来源：http://op.hnjuh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xa.panjiajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://im.szxytkj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://oj.bjjhwx.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qc.yuexingan06.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ch.panjiajie.cn

Ruby: def greet(name = "World") = name
来源：http://ss.521024.cn

C#:   string Greet(string name = "World") => name;
来源：http://gy.muxihuayi.cn

[C03] 可变参数
来源：http://ap.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://uz.yuexingan06.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gq.chemitech.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kn.haigaiapp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dg.nszjky.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gr.bookmarksfly.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ah.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cs.yuexingan06.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gb.9csxet.cn

[C04] 命名参数 / 关键字参数
来源：http://ed.521024.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ei.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ww.huixiangedu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qe.muxihuayi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xl.gzmigu.cn

Java: // 无：用 Builder 模式或 record
来源：http://fu.nszjky.cn

Go:   // 无：用配置结构体参数
来源：http://gb.lnxyls.cn

Ruby: f(a: 1, b: 2)
来源：http://fn.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://hj.muxihuayi.cn

[C05] 返回多个值
来源：http://ju.nszjky.cn

Py:   return a, b
来源：http://im.nszjky.cn

PHP:  return [$a, $b];
来源：http://cn.hnjuh.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hc.newstarts.cn

TS:   return { a, b };
来源：http://qb.huanxung.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mk.chemitech.net.cn

Go:   return a, b
来源：http://nq.yuexingan06.cn

Ruby: return a, b
来源：http://qw.jianghongdianzi.cn

C#:   return (a, b);              // ValueTuple
来源：http://nj.chemitech.net.cn

[C06] 匿名函数 / lambda
来源：http://kc.lnxyls.cn

Py:   square = lambda x: x * x
来源：http://ge.shtwfgs.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xp.lnxyls.cn

JS:   const square = x => x * x;
来源：http://zl.nicolike.cn


<!-- 参考信息 -->