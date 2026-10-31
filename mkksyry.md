代发 wailian999

Ruby: value = data || "默认值"
来源：http://ix.nszjky.cn

C#:   var value = data ?? "默认值";
来源：http://sj.wgjwhj.cn

[A16] 真假值判断规则
来源：http://nm.huixinmuqiang.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pk.chemitech.net.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jq.panjiajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ep.huanxung.cn

TS:   if (!x) {}
来源：http://eh.jianghongdianzi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://is.panjiajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://uv.bjjhwx.cn

Ruby: unless x            # nil 与 false 为假
来源：http://dq.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://eb.huixinmuqiang.cn

[A17] 位运算
来源：http://up.shxzskj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wp.asd995.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sr.szsharing.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zb.colortex.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rd.chemitech.net.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gy.chemitech.net.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cx.colortex.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vu.muxihuayi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ia.newstarts.cn

[A18] 字符与 ASCII 码互转
来源：http://tw.9csxet.cn

Py:   ord("A"); chr(65)
来源：http://vt.lnxyls.cn

PHP:  ord("A"); chr(65)
来源：http://wz.jianghongdianzi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nv.9csxet.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uz.newstarts.cn

Java: (int) 'A'; (char) 65
来源：http://te.szxytkj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://sy.lnxyls.cn

Ruby: "A".ord; 65.chr
来源：http://kq.9csxet.cn

C#:   (int)'A'; (char)65
来源：http://np.panjiajie.cn

[A19] 交换两个变量
来源：http://my.szxytkj.cn

Py:   a, b = b, a
来源：http://jj.9csxet.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://po.colortex.cn

JS:   [a, b] = [b, a];
来源：http://pn.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://wu.bjjhwx.cn

Java: int t = a; a = b; b = t;
来源：http://op.szxytkj.cn

Go:   a, b = b, a
来源：http://sa.hnjuh.cn

Ruby: a, b = b, a
来源：http://yh.huanxung.cn

C#:   (a, b) = (b, a);
来源：http://em.shtwfgs.cn

[A20] 读取标准输入
来源：http://wt.asd995.cn

Py:   name = input("请输入：")
来源：http://ye.muxihuayi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://sp.nszjky.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gt.newstarts.cn

TS:   // Node.js：readline 模块
来源：http://dr.newstarts.cn

Java: new Scanner(System.in).nextLine()
来源：http://cw.yuntaijiaju.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://an.newstarts.cn

Ruby: gets.chomp
来源：http://th.bjjhwx.cn

C#:   Console.ReadLine();
来源：http://dq.lnxyls.cn

[A21] 保留指定小数位输出
来源：http://gi.nicolike.cn

Py:   f"{3.14159:.2f}"
来源：http://kl.wgjwhj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lo.muxihuayi.cn

JS:   (3.14159).toFixed(2)
来源：http://ql.chemitech.net.cn

TS:   (3.14159).toFixed(2)
来源：http://jg.shtwfgs.cn

Java: String.format("%.2f", 3.14159)
来源：http://fy.asd995.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://om.newstarts.cn

Ruby: format("%.2f", 3.14159)
来源：http://mc.gzmigu.cn

C#:   3.14159.ToString("F2")
来源：http://do.nszjky.cn

[A22] 获取字符串长度
来源：http://zc.szsharing.cn

Py:   len(s)
来源：http://pj.jianghongdianzi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mz.asd995.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rf.huanxung.cn

TS:   s.length
来源：http://yu.521024.cn

Java: s.length()
来源：http://vm.nszjky.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fs.hnjuh.cn

Ruby: s.length
来源：http://cq.jctech888.com.cn

C#:   s.Length
来源：http://gt.colortex.cn

[A23] 大小写转换
来源：http://bj.colortex.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://lz.szsharing.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ik.muxihuayi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wr.haigaiapp.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://so.nszjky.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qi.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ev.szsharing.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rx.nszjky.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://kg.newstarts.cn

[A24] 去除首尾空白
来源：http://ua.lnxyls.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pi.9csxet.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zi.yuexingan06.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ky.shtwfgs.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qh.jianghongdianzi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://or.shxzskj.cn

Go:   strings.TrimSpace(s)
来源：http://il.jctech888.com.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://do.huixiangedu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vr.jianghongdianzi.cn

[A25] 字符串比较
来源：http://sx.521024.cn

Py:   s1 == s2; s1 != s2
来源：http://me.bjjhwx.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jb.huanxung.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zf.haigaiapp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yr.gzmigu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kp.bookmarksfly.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zi.hnjuh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nu.muxihuayi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hs.jctech888.com.cn

[A26] 类型转换总览
来源：http://jw.jctech888.com.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wb.huixiangedu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lf.shtwfgs.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tm.panjiajie.cn

TS:   Number() String() Boolean() x as number
来源：http://np.jianghongdianzi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jx.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ox.huixiangedu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pp.szsharing.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rs.panjiajie.cn

================================================================================
来源：http://cj.haigaiapp.cn

B. 流程控制
来源：http://xr.asd995.cn

================================================================================
来源：http://sl.hahajie.cn

[B01] 条件判断 if / else
来源：http://ka.asd995.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://sv.newstarts.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://im.panjiajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://en.yuntaijiaju.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ls.521024.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lw.colortex.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ry.521024.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rc.gzmigu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ol.nszjky.cn

[B02] 多分支 else if / elif
来源：http://at.nszjky.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fo.huixiangedu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yl.szsharing.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dn.huixiangedu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://be.9csxet.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oh.shxzskj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wc.nicolike.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cg.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ld.nszjky.cn

[B03] switch / match / case
来源：http://kp.hnjuh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://po.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://la.shtwfgs.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kl.newstarts.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uh.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ki.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nk.szxytkj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jg.hnjuh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xm.jctech888.com.cn

[B04] for 计数循环
来源：http://ww.yuntaijiaju.cn

Py:   for i in range(10): print(i)
来源：http://yc.chemitech.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://up.shxzskj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://db.9csxet.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ef.jianghongdianzi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uy.newstarts.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kk.muxihuayi.cn

Ruby: 10.times { |i| puts i }
来源：http://xy.newstarts.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ly.bjjhwx.cn

[B05] 遍历数组 / 列表
来源：http://sg.shtwfgs.cn

Py:   for item in arr: print(item)
来源：http://jn.szsharing.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tu.muxihuayi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kf.panjiajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ww.shxzukj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wo.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mq.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://dm.szxytkj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kc.huixiangedu.cn

[B06] 遍历字典 / 对象
来源：http://ai.jctech888.com.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gg.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mp.shxzukj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://id.muxihuayi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://et.jianghongdianzi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fp.hnjuh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yq.521024.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rk.521024.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zq.hnjuh.cn

[B07] while 循环
来源：http://lk.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://lh.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vw.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://gp.asd995.cn

TS:   while (i < 10) { i++; }
来源：http://es.asd995.cn

Java: while (i < 10) { i++; }
来源：http://vg.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bw.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://jd.shtwfgs.cn

C#:   while (i < 10) { i++; }
来源：http://zx.yuntaijiaju.cn

[B08] do-while（至少执行一次）
来源：http://sb.521024.cn

Py:   # 无 do-while：用 while True + break
来源：http://dx.muxihuayi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dg.shtwfgs.cn

JS:   do { i++; } while (i < 10);
来源：http://je.asd995.cn

TS:   do { i++; } while (i < 10);
来源：http://gy.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://tl.szxytkj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cq.bookmarksfly.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ua.gzmigu.cn

C#:   do { i++; } while (i < 10);
来源：http://dk.jianghongdianzi.cn

[B09] break 与 continue
来源：http://ve.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tn.huixinmuqiang.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hr.muxihuayi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ml.muxihuayi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kc.wgjwhj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://co.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ca.haigaiapp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mf.szsharing.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qk.yuexingan06.cn

[B10] 遍历同时拿索引
来源：http://sk.jianghongdianzi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lq.9csxet.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lw.bjjhwx.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cl.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://de.9csxet.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sp.panjiajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://na.haigaiapp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gj.panjiajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sz.jctech888.com.cn

[B11] 生成数字序列 / 区间
来源：http://ya.521024.cn

Py:   list(range(0, 10, 2))
来源：http://iv.521024.cn

PHP:  range(0, 10, 2);
来源：http://yg.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ls.szxytkj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ro.szxytkj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://si.colortex.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ja.huanxung.cn

Ruby: (0...10).step(2).to_a
来源：http://ve.yuntaijiaju.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://be.yuexingan06.cn

[B12] 跳出多层循环
来源：http://tu.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hq.hahajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yf.newstarts.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lo.bookmarksfly.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gh.szxytkj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lw.nszjky.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xv.colortex.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mi.jianghongdianzi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ar.chemitech.net.cn

[B13] 判断是否为数字
来源：http://vr.hnjuh.cn

Py:   isinstance(x, (int, float))
来源：http://ij.yuexingan06.cn

PHP:  is_numeric($x)
来源：http://wu.shxzukj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vq.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shxzukj.cn

Java: x instanceof Number
来源：http://aj.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ri.huixinmuqiang.cn

Ruby: x.is_a?(Numeric)
来源：http://lk.shxzskj.cn

C#:   x is int or double or decimal
来源：http://fy.shtwfgs.cn

[B14] 判断值是否在集合内
来源：http://ee.shxzukj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qu.shxzskj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://aw.9csxet.cn

JS:   [1, 2, 3].includes(x)
来源：http://id.521024.cn

TS:   [1, 2, 3].includes(x)
来源：http://fz.yuntaijiaju.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kq.gzmigu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zw.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ui.lnxyls.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uo.jianghongdianzi.cn

[B15] 布尔运算与取反
来源：http://vr.szxytkj.cn

Py:   a and b or not c
来源：http://yk.yuexingan06.cn

PHP:  $a && $b || !$c
来源：http://hq.muxihuayi.cn

JS:   a && b || !c
来源：http://my.lnxyls.cn

TS:   a && b || !c
来源：http://jt.bookmarksfly.cn

Java: a && b || !c
来源：http://fd.yuntaijiaju.cn

Go:   a && b || !c
来源：http://gn.gzmigu.cn

Ruby: a && b || !c
来源：http://op.jianghongdianzi.cn

C#:   a && b || !c
来源：http://nw.shxzukj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lh.yuntaijiaju.cn

Py:   if not data: return
来源：http://gm.gzmigu.cn

PHP:  if (!$data) { return; }
来源：http://yj.hahajie.cn

JS:   if (!data) return;
来源：http://wd.521024.cn

TS:   if (!data) return;
来源：http://bm.chemitech.net.cn

Java: if (data == null) return;
来源：http://wj.hnjuh.cn

Go:   if data == nil { return }
来源：http://su.shxzukj.cn

Ruby: return if data.nil?
来源：http://pg.bjjhwx.cn

C#:   if (data == null) return;
来源：http://ot.521024.cn

================================================================================
来源：http://sg.haigaiapp.cn

C. 函数与作用域
来源：http://om.chemitech.net.cn

================================================================================
来源：http://bu.nszjky.cn

[C01] 定义函数
来源：http://ge.szsharing.cn

Py:   def add(a, b): return a + b
来源：http://or.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jl.jctech888.com.cn

JS:   function add(a, b) { return a + b; }
来源：http://pr.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vt.huixiangedu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ks.panjiajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rs.szxytkj.cn

Ruby: def add(a, b); a + b; end
来源：http://hl.shxzskj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wr.gzmigu.cn

[C02] 默认参数
来源：http://ri.shxzskj.cn

Py:   def greet(name="World"): return name
来源：http://ml.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zr.521024.cn

JS:   function greet(name = "World") { return name; }
来源：http://zg.haigaiapp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ha.hahajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vj.muxihuayi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ij.jianghongdianzi.cn

Ruby: def greet(name = "World") = name
来源：http://sk.nicolike.cn

C#:   string Greet(string name = "World") => name;
来源：http://nn.huixiangedu.cn

[C03] 可变参数
来源：http://lt.nicolike.cn

Py:   def total(*args): return sum(args)
来源：http://ud.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yb.shtwfgs.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fr.lnxyls.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rg.gzmigu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gp.huixinmuqiang.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kc.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ny.9csxet.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xp.nicolike.cn

[C04] 命名参数 / 关键字参数
来源：http://wt.colortex.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rz.nszjky.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gh.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jr.huixiangedu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pv.nicolike.cn

Java: // 无：用 Builder 模式或 record
来源：http://gk.bjjhwx.cn

Go:   // 无：用配置结构体参数
来源：http://th.colortex.cn

Ruby: f(a: 1, b: 2)
来源：http://qe.jianghongdianzi.cn

C#:   f(a: 1, b: 2)
来源：http://dz.yuexingan06.cn

[C05] 返回多个值
来源：http://dp.nicolike.cn

Py:   return a, b
来源：http://gh.colortex.cn

PHP:  return [$a, $b];
来源：http://sp.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zf.nicolike.cn

TS:   return { a, b };
来源：http://zi.yuntaijiaju.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fg.shxzukj.cn

Go:   return a, b
来源：http://xr.asd995.cn

Ruby: return a, b
来源：http://wn.jianghongdianzi.cn

C#:   return (a, b);              // ValueTuple
来源：http://yl.asd995.cn

[C06] 匿名函数 / lambda
来源：http://ln.bookmarksfly.cn

Py:   square = lambda x: x * x
来源：http://qi.colortex.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rm.colortex.cn

JS:   const square = x => x * x;
来源：http://wz.hnjuh.cn


<!-- 参考信息 -->