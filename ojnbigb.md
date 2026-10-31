代发 wailian999

Ruby: value = data || "默认值"
来源：http://hi.huanxung.cn

C#:   var value = data ?? "默认值";
来源：http://up.bjjhwx.cn

[A16] 真假值判断规则
来源：http://yu.bjjhwx.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mc.hahajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jv.gzmigu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ph.chemitech.net.cn

TS:   if (!x) {}
来源：http://yq.521024.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wo.panjiajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xc.yuexingan06.cn

Ruby: unless x            # nil 与 false 为假
来源：http://rh.shxzukj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ry.bookmarksfly.cn

[A17] 位运算
来源：http://yc.shtwfgs.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ws.yuntaijiaju.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lb.nicolike.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ae.panjiajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zl.hahajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ju.panjiajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gw.bookmarksfly.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://za.shxzukj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xn.newstarts.cn

[A18] 字符与 ASCII 码互转
来源：http://nk.521024.cn

Py:   ord("A"); chr(65)
来源：http://ah.jctech888.com.cn

PHP:  ord("A"); chr(65)
来源：http://vf.shxzskj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://aq.panjiajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ja.gzmigu.cn

Java: (int) 'A'; (char) 65
来源：http://zc.nszjky.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ie.szxytkj.cn

Ruby: "A".ord; 65.chr
来源：http://xc.chemitech.net.cn

C#:   (int)'A'; (char)65
来源：http://hw.asd995.cn

[A19] 交换两个变量
来源：http://zv.yuexingan06.cn

Py:   a, b = b, a
来源：http://hb.wgjwhj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://nc.newstarts.cn

JS:   [a, b] = [b, a];
来源：http://sq.wgjwhj.cn

TS:   [a, b] = [b, a];
来源：http://qw.hnjuh.cn

Java: int t = a; a = b; b = t;
来源：http://si.newstarts.cn

Go:   a, b = b, a
来源：http://px.gzmigu.cn

Ruby: a, b = b, a
来源：http://wd.panjiajie.cn

C#:   (a, b) = (b, a);
来源：http://xw.shxzskj.cn

[A20] 读取标准输入
来源：http://qp.hnjuh.cn

Py:   name = input("请输入：")
来源：http://zx.panjiajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://xp.haigaiapp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ns.huixiangedu.cn

TS:   // Node.js：readline 模块
来源：http://ii.shtwfgs.cn

Java: new Scanner(System.in).nextLine()
来源：http://cm.nszjky.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gk.huanxung.cn

Ruby: gets.chomp
来源：http://qz.bookmarksfly.cn

C#:   Console.ReadLine();
来源：http://yx.huanxung.cn

[A21] 保留指定小数位输出
来源：http://hx.muxihuayi.cn

Py:   f"{3.14159:.2f}"
来源：http://nw.9csxet.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://du.9csxet.cn

JS:   (3.14159).toFixed(2)
来源：http://hg.newstarts.cn

TS:   (3.14159).toFixed(2)
来源：http://pa.jianghongdianzi.cn

Java: String.format("%.2f", 3.14159)
来源：http://sh.bjjhwx.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pm.huixiangedu.cn

Ruby: format("%.2f", 3.14159)
来源：http://rz.nicolike.cn

C#:   3.14159.ToString("F2")
来源：http://gw.521024.cn

[A22] 获取字符串长度
来源：http://na.shxzukj.cn

Py:   len(s)
来源：http://js.hnjuh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ac.muxihuayi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tj.yuntaijiaju.cn

TS:   s.length
来源：http://pc.colortex.cn

Java: s.length()
来源：http://cj.shxzskj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nq.panjiajie.cn

Ruby: s.length
来源：http://ln.huixinmuqiang.cn

C#:   s.Length
来源：http://vo.shxzskj.cn

[A23] 大小写转换
来源：http://ku.chemitech.net.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zs.shtwfgs.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mz.bookmarksfly.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cb.huixiangedu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://oc.huixinmuqiang.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ze.bjjhwx.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bl.shtwfgs.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cl.shxzukj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wh.9csxet.cn

[A24] 去除首尾空白
来源：http://zd.huixinmuqiang.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ji.huixiangedu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xk.panjiajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iu.lnxyls.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://on.huixiangedu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wy.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://uh.bookmarksfly.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wk.muxihuayi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://px.hnjuh.cn

[A25] 字符串比较
来源：http://nm.szsharing.cn

Py:   s1 == s2; s1 != s2
来源：http://xv.nicolike.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dt.muxihuayi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://up.nicolike.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jm.asd995.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yd.bookmarksfly.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tj.nicolike.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pa.jianghongdianzi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ok.gzmigu.cn

[A26] 类型转换总览
来源：http://mf.nszjky.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sd.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lo.chemitech.net.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nk.9csxet.cn

TS:   Number() String() Boolean() x as number
来源：http://yq.huixinmuqiang.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wr.szxytkj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jj.szsharing.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hp.521024.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wp.shxzskj.cn

================================================================================
来源：http://fc.asd995.cn

B. 流程控制
来源：http://bn.521024.cn

================================================================================
来源：http://ue.shxzukj.cn

[B01] 条件判断 if / else
来源：http://nz.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mj.gzmigu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bx.muxihuayi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://id.hahajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ch.wgjwhj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pg.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sq.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vf.wgjwhj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nv.szsharing.cn

[B02] 多分支 else if / elif
来源：http://kn.yuntaijiaju.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yx.gzmigu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nt.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yc.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qh.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yz.shxzskj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ho.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rv.hahajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uc.muxihuayi.cn

[B03] switch / match / case
来源：http://bi.hnjuh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ew.newstarts.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uj.wgjwhj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cb.muxihuayi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://at.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://st.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bk.jianghongdianzi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mp.huixiangedu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vl.szxytkj.cn

[B04] for 计数循环
来源：http://mt.yuntaijiaju.cn

Py:   for i in range(10): print(i)
来源：http://ut.chemitech.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tw.szsharing.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nt.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mp.huanxung.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ti.nszjky.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hu.nicolike.cn

Ruby: 10.times { |i| puts i }
来源：http://sr.gzmigu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bo.muxihuayi.cn

[B05] 遍历数组 / 列表
来源：http://bh.bjjhwx.cn

Py:   for item in arr: print(item)
来源：http://az.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gh.muxihuayi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://um.nszjky.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bv.huanxung.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kx.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lo.huanxung.cn

Ruby: arr.each { |item| puts item }
来源：http://kk.bjjhwx.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://go.nszjky.cn

[B06] 遍历字典 / 对象
来源：http://gp.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gs.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yf.szsharing.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zt.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ij.asd995.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ir.gzmigu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tg.shtwfgs.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lo.muxihuayi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ru.huixiangedu.cn

[B07] while 循环
来源：http://cq.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://he.gzmigu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ip.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://xp.nszjky.cn

TS:   while (i < 10) { i++; }
来源：http://ey.asd995.cn

Java: while (i < 10) { i++; }
来源：http://fx.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uh.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://kf.521024.cn

C#:   while (i < 10) { i++; }
来源：http://ja.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://rm.chemitech.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://ci.521024.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qh.huixinmuqiang.cn

JS:   do { i++; } while (i < 10);
来源：http://zd.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://yv.521024.cn

Java: do { i++; } while (i < 10);
来源：http://mi.shtwfgs.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://kf.shtwfgs.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ao.nicolike.cn

C#:   do { i++; } while (i < 10);
来源：http://xo.9csxet.cn

[B09] break 与 continue
来源：http://ap.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uc.szxytkj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vw.nicolike.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mh.gzmigu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ay.szxytkj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pa.bjjhwx.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fq.jctech888.com.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kq.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sr.haigaiapp.cn

[B10] 遍历同时拿索引
来源：http://ky.yuntaijiaju.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pc.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cz.colortex.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tc.hnjuh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jk.wgjwhj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ty.jctech888.com.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oc.newstarts.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rj.huanxung.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pj.hahajie.cn

[B11] 生成数字序列 / 区间
来源：http://sx.panjiajie.cn

Py:   list(range(0, 10, 2))
来源：http://th.colortex.cn

PHP:  range(0, 10, 2);
来源：http://vy.nicolike.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kr.chemitech.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mw.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dz.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pb.szsharing.cn

Ruby: (0...10).step(2).to_a
来源：http://av.muxihuayi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lm.panjiajie.cn

[B12] 跳出多层循环
来源：http://ao.jianghongdianzi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wk.lnxyls.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wh.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ah.gzmigu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://oo.szsharing.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gy.haigaiapp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kl.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pk.shtwfgs.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hp.huixinmuqiang.cn

[B13] 判断是否为数字
来源：http://bp.hahajie.cn

Py:   isinstance(x, (int, float))
来源：http://bg.yuexingan06.cn

PHP:  is_numeric($x)
来源：http://uo.shxzskj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ld.huixiangedu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vt.haigaiapp.cn

Java: x instanceof Number
来源：http://hf.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gv.shtwfgs.cn

Ruby: x.is_a?(Numeric)
来源：http://ej.shxzskj.cn

C#:   x is int or double or decimal
来源：http://tu.muxihuayi.cn

[B14] 判断值是否在集合内
来源：http://gp.asd995.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yr.yuexingan06.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yd.colortex.cn

JS:   [1, 2, 3].includes(x)
来源：http://ug.colortex.cn

TS:   [1, 2, 3].includes(x)
来源：http://pz.asd995.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://af.shxzskj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mf.yuexingan06.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rx.panjiajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ei.yuexingan06.cn

[B15] 布尔运算与取反
来源：http://yp.asd995.cn

Py:   a and b or not c
来源：http://ef.hahajie.cn

PHP:  $a && $b || !$c
来源：http://vz.bjjhwx.cn

JS:   a && b || !c
来源：http://cs.newstarts.cn

TS:   a && b || !c
来源：http://qp.jianghongdianzi.cn

Java: a && b || !c
来源：http://yy.shxzskj.cn

Go:   a && b || !c
来源：http://fy.muxihuayi.cn

Ruby: a && b || !c
来源：http://bf.yuexingan06.cn

C#:   a && b || !c
来源：http://zt.shtwfgs.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kw.bjjhwx.cn

Py:   if not data: return
来源：http://hq.huixiangedu.cn

PHP:  if (!$data) { return; }
来源：http://sy.muxihuayi.cn

JS:   if (!data) return;
来源：http://wn.szxytkj.cn

TS:   if (!data) return;
来源：http://me.huanxung.cn

Java: if (data == null) return;
来源：http://nd.gzmigu.cn

Go:   if data == nil { return }
来源：http://cr.nicolike.cn

Ruby: return if data.nil?
来源：http://vz.huanxung.cn

C#:   if (data == null) return;
来源：http://bs.chemitech.net.cn

================================================================================
来源：http://vd.yuntaijiaju.cn

C. 函数与作用域
来源：http://ob.colortex.cn

================================================================================
来源：http://ab.lnxyls.cn

[C01] 定义函数
来源：http://xg.panjiajie.cn

Py:   def add(a, b): return a + b
来源：http://uc.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kt.nicolike.cn

JS:   function add(a, b) { return a + b; }
来源：http://gd.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jv.szxytkj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jy.szsharing.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ql.hahajie.cn

Ruby: def add(a, b); a + b; end
来源：http://zf.yuexingan06.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ie.asd995.cn

[C02] 默认参数
来源：http://vu.521024.cn

Py:   def greet(name="World"): return name
来源：http://tv.lnxyls.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://sx.huixinmuqiang.cn

JS:   function greet(name = "World") { return name; }
来源：http://my.9csxet.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zn.chemitech.net.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ei.hnjuh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ak.muxihuayi.cn

Ruby: def greet(name = "World") = name
来源：http://cn.shtwfgs.cn

C#:   string Greet(string name = "World") => name;
来源：http://rm.bjjhwx.cn

[C03] 可变参数
来源：http://rr.yuexingan06.cn

Py:   def total(*args): return sum(args)
来源：http://mn.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://td.huanxung.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mc.nicolike.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rv.nszjky.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://de.chemitech.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mk.szxytkj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vl.panjiajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wr.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://dg.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cv.shtwfgs.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fn.wgjwhj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zf.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pp.lnxyls.cn

Java: // 无：用 Builder 模式或 record
来源：http://dg.jianghongdianzi.cn

Go:   // 无：用配置结构体参数
来源：http://pw.yuntaijiaju.cn

Ruby: f(a: 1, b: 2)
来源：http://ad.panjiajie.cn

C#:   f(a: 1, b: 2)
来源：http://ic.521024.cn

[C05] 返回多个值
来源：http://nc.bjjhwx.cn

Py:   return a, b
来源：http://kj.colortex.cn

PHP:  return [$a, $b];
来源：http://qo.muxihuayi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nf.shtwfgs.cn

TS:   return { a, b };
来源：http://ge.chemitech.net.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kl.bjjhwx.cn

Go:   return a, b
来源：http://kr.shxzskj.cn

Ruby: return a, b
来源：http://br.chemitech.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://sm.haigaiapp.cn

[C06] 匿名函数 / lambda
来源：http://nz.shxzskj.cn

Py:   square = lambda x: x * x
来源：http://mv.huixinmuqiang.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://aq.shxzskj.cn

JS:   const square = x => x * x;
来源：http://sp.colortex.cn


<!-- 参考信息 -->