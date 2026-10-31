代发 wailian999

Ruby: value = data || "默认值"
来源：http://xa.521024.cn

C#:   var value = data ?? "默认值";
来源：http://ta.huixinmuqiang.cn

[A16] 真假值判断规则
来源：http://ne.newstarts.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dm.bookmarksfly.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nv.shxzskj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fh.szxytkj.cn

TS:   if (!x) {}
来源：http://lp.hahajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jd.jctech888.com.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xn.shxzskj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://cc.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pm.wgjwhj.cn

[A17] 位运算
来源：http://gs.nicolike.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yn.jianghongdianzi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xr.panjiajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ky.muxihuayi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zl.yuntaijiaju.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pi.shtwfgs.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pq.huanxung.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wh.jctech888.com.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eq.huixinmuqiang.cn

[A18] 字符与 ASCII 码互转
来源：http://gj.hnjuh.cn

Py:   ord("A"); chr(65)
来源：http://yi.bookmarksfly.cn

PHP:  ord("A"); chr(65)
来源：http://xz.huixinmuqiang.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dr.bjjhwx.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rj.shxzskj.cn

Java: (int) 'A'; (char) 65
来源：http://cb.wgjwhj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ei.jctech888.com.cn

Ruby: "A".ord; 65.chr
来源：http://rm.szsharing.cn

C#:   (int)'A'; (char)65
来源：http://me.jianghongdianzi.cn

[A19] 交换两个变量
来源：http://xp.shtwfgs.cn

Py:   a, b = b, a
来源：http://sk.9csxet.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://iw.huixinmuqiang.cn

JS:   [a, b] = [b, a];
来源：http://bf.newstarts.cn

TS:   [a, b] = [b, a];
来源：http://og.521024.cn

Java: int t = a; a = b; b = t;
来源：http://eh.hnjuh.cn

Go:   a, b = b, a
来源：http://io.huixiangedu.cn

Ruby: a, b = b, a
来源：http://et.huixinmuqiang.cn

C#:   (a, b) = (b, a);
来源：http://ul.gzmigu.cn

[A20] 读取标准输入
来源：http://wz.jianghongdianzi.cn

Py:   name = input("请输入：")
来源：http://sd.hnjuh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qo.muxihuayi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ok.huanxung.cn

TS:   // Node.js：readline 模块
来源：http://jh.521024.cn

Java: new Scanner(System.in).nextLine()
来源：http://pb.shxzukj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bg.wgjwhj.cn

Ruby: gets.chomp
来源：http://xm.newstarts.cn

C#:   Console.ReadLine();
来源：http://be.colortex.cn

[A21] 保留指定小数位输出
来源：http://dr.shtwfgs.cn

Py:   f"{3.14159:.2f}"
来源：http://tw.jianghongdianzi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xl.yuexingan06.cn

JS:   (3.14159).toFixed(2)
来源：http://ph.shtwfgs.cn

TS:   (3.14159).toFixed(2)
来源：http://vm.asd995.cn

Java: String.format("%.2f", 3.14159)
来源：http://ed.yuntaijiaju.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ut.nicolike.cn

Ruby: format("%.2f", 3.14159)
来源：http://de.muxihuayi.cn

C#:   3.14159.ToString("F2")
来源：http://vd.szsharing.cn

[A22] 获取字符串长度
来源：http://vl.nicolike.cn

Py:   len(s)
来源：http://rm.huixinmuqiang.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jl.nszjky.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vl.bjjhwx.cn

TS:   s.length
来源：http://wr.9csxet.cn

Java: s.length()
来源：http://xk.asd995.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yj.huanxung.cn

Ruby: s.length
来源：http://kt.gzmigu.cn

C#:   s.Length
来源：http://lj.asd995.cn

[A23] 大小写转换
来源：http://yq.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ut.huixinmuqiang.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lf.shxzskj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://et.nicolike.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fr.hnjuh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bl.newstarts.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jh.panjiajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ih.asd995.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fh.yuexingan06.cn

[A24] 去除首尾空白
来源：http://ow.hahajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nc.szxytkj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ab.jianghongdianzi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tw.jctech888.com.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qa.muxihuayi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://av.huanxung.cn

Go:   strings.TrimSpace(s)
来源：http://ey.szxytkj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ux.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://op.gzmigu.cn

[A25] 字符串比较
来源：http://qb.wgjwhj.cn

Py:   s1 == s2; s1 != s2
来源：http://jm.huanxung.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://av.asd995.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ld.hnjuh.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ah.huanxung.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tg.wgjwhj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nw.nicolike.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vs.hnjuh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sy.shxzukj.cn

[A26] 类型转换总览
来源：http://lv.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fl.chemitech.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://aj.wgjwhj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ng.bookmarksfly.cn

TS:   Number() String() Boolean() x as number
来源：http://si.yuexingan06.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rc.panjiajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ps.wgjwhj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vq.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gu.wgjwhj.cn

================================================================================
来源：http://dv.hnjuh.cn

B. 流程控制
来源：http://tf.jianghongdianzi.cn

================================================================================
来源：http://iy.yuntaijiaju.cn

[B01] 条件判断 if / else
来源：http://gb.jctech888.com.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xc.colortex.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ht.jianghongdianzi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gq.muxihuayi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ds.panjiajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ol.haigaiapp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://av.nszjky.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ss.hahajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zo.haigaiapp.cn

[B02] 多分支 else if / elif
来源：http://ic.nszjky.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vn.bookmarksfly.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gm.newstarts.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://il.asd995.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qy.yuntaijiaju.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wl.hahajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bz.huixinmuqiang.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hm.panjiajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lg.asd995.cn

[B03] switch / match / case
来源：http://vf.nicolike.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ka.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wi.huanxung.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qu.haigaiapp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bq.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pq.lnxyls.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xx.huanxung.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oa.yuntaijiaju.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wt.shxzukj.cn

[B04] for 计数循环
来源：http://px.muxihuayi.cn

Py:   for i in range(10): print(i)
来源：http://fp.jctech888.com.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qf.wgjwhj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://se.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vt.szsharing.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ws.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lj.muxihuayi.cn

Ruby: 10.times { |i| puts i }
来源：http://pr.bjjhwx.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lv.panjiajie.cn

[B05] 遍历数组 / 列表
来源：http://xp.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://wr.jianghongdianzi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://aj.chemitech.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wo.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gm.bjjhwx.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lt.hnjuh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tv.gzmigu.cn

Ruby: arr.each { |item| puts item }
来源：http://ms.szxytkj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vj.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://jd.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mu.hnjuh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zp.bjjhwx.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jj.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vc.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ul.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rp.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ay.shtwfgs.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sw.nszjky.cn

[B07] while 循环
来源：http://da.asd995.cn

Py:   while i < 10: i += 1
来源：http://ix.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://sd.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://qp.szxytkj.cn

TS:   while (i < 10) { i++; }
来源：http://xv.newstarts.cn

Java: while (i < 10) { i++; }
来源：http://oi.szxytkj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wd.hnjuh.cn

Ruby: while i < 10; i += 1; end
来源：http://pj.jianghongdianzi.cn

C#:   while (i < 10) { i++; }
来源：http://km.haigaiapp.cn

[B08] do-while（至少执行一次）
来源：http://rg.huixinmuqiang.cn

Py:   # 无 do-while：用 while True + break
来源：http://ej.lnxyls.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jg.asd995.cn

JS:   do { i++; } while (i < 10);
来源：http://gf.panjiajie.cn

TS:   do { i++; } while (i < 10);
来源：http://de.hnjuh.cn

Java: do { i++; } while (i < 10);
来源：http://sh.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fd.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ay.gzmigu.cn

C#:   do { i++; } while (i < 10);
来源：http://zu.huixiangedu.cn

[B09] break 与 continue
来源：http://ic.521024.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://il.szsharing.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oz.shxzskj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yb.colortex.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ih.szsharing.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hb.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jk.jianghongdianzi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fm.hahajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zr.yuntaijiaju.cn

[B10] 遍历同时拿索引
来源：http://ua.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cc.9csxet.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nh.asd995.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nm.bookmarksfly.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kv.chemitech.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rw.bjjhwx.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ji.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qg.hnjuh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pk.hahajie.cn

[B11] 生成数字序列 / 区间
来源：http://cd.shxzukj.cn

Py:   list(range(0, 10, 2))
来源：http://lg.bjjhwx.cn

PHP:  range(0, 10, 2);
来源：http://ja.shtwfgs.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nx.yuntaijiaju.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://np.szsharing.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://av.colortex.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://aa.panjiajie.cn

Ruby: (0...10).step(2).to_a
来源：http://he.muxihuayi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jz.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://ll.colortex.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ol.shxzukj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yx.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hj.gzmigu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lm.chemitech.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fa.521024.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://he.huixiangedu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uh.jctech888.com.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ag.muxihuayi.cn

[B13] 判断是否为数字
来源：http://xu.bjjhwx.cn

Py:   isinstance(x, (int, float))
来源：http://zo.huixinmuqiang.cn

PHP:  is_numeric($x)
来源：http://ok.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ad.bjjhwx.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zh.lnxyls.cn

Java: x instanceof Number
来源：http://mu.chemitech.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://my.nicolike.cn

Ruby: x.is_a?(Numeric)
来源：http://uk.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://pv.muxihuayi.cn

[B14] 判断值是否在集合内
来源：http://gr.hnjuh.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rz.wgjwhj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oj.hnjuh.cn

JS:   [1, 2, 3].includes(x)
来源：http://vc.shtwfgs.cn

TS:   [1, 2, 3].includes(x)
来源：http://nj.asd995.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://si.huixiangedu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yf.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vj.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wo.bookmarksfly.cn

[B15] 布尔运算与取反
来源：http://bu.521024.cn

Py:   a and b or not c
来源：http://ln.shxzskj.cn

PHP:  $a && $b || !$c
来源：http://jd.jianghongdianzi.cn

JS:   a && b || !c
来源：http://da.yuntaijiaju.cn

TS:   a && b || !c
来源：http://zh.bjjhwx.cn

Java: a && b || !c
来源：http://rf.hahajie.cn

Go:   a && b || !c
来源：http://mb.jianghongdianzi.cn

Ruby: a && b || !c
来源：http://fr.colortex.cn

C#:   a && b || !c
来源：http://bd.colortex.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gu.asd995.cn

Py:   if not data: return
来源：http://ce.huanxung.cn

PHP:  if (!$data) { return; }
来源：http://yo.panjiajie.cn

JS:   if (!data) return;
来源：http://vt.asd995.cn

TS:   if (!data) return;
来源：http://gh.jctech888.com.cn

Java: if (data == null) return;
来源：http://rt.szsharing.cn

Go:   if data == nil { return }
来源：http://st.9csxet.cn

Ruby: return if data.nil?
来源：http://qy.wgjwhj.cn

C#:   if (data == null) return;
来源：http://fa.chemitech.net.cn

================================================================================
来源：http://up.huixiangedu.cn

C. 函数与作用域
来源：http://nl.szsharing.cn

================================================================================
来源：http://vw.colortex.cn

[C01] 定义函数
来源：http://pv.huixiangedu.cn

Py:   def add(a, b): return a + b
来源：http://yu.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jm.chemitech.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://ja.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pj.huixiangedu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dw.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://oy.huanxung.cn

Ruby: def add(a, b); a + b; end
来源：http://md.hnjuh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cr.bjjhwx.cn

[C02] 默认参数
来源：http://yq.9csxet.cn

Py:   def greet(name="World"): return name
来源：http://bp.nszjky.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://co.hnjuh.cn

JS:   function greet(name = "World") { return name; }
来源：http://ep.huanxung.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mh.chemitech.net.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://eb.huanxung.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ya.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://ri.nicolike.cn

C#:   string Greet(string name = "World") => name;
来源：http://ko.asd995.cn

[C03] 可变参数
来源：http://zr.wgjwhj.cn

Py:   def total(*args): return sum(args)
来源：http://vu.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ep.nicolike.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wy.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xp.nszjky.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xb.chemitech.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nn.nicolike.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mo.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ju.colortex.cn

[C04] 命名参数 / 关键字参数
来源：http://cw.wgjwhj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bj.9csxet.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xc.bookmarksfly.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://op.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gw.haigaiapp.cn

Java: // 无：用 Builder 模式或 record
来源：http://pg.szsharing.cn

Go:   // 无：用配置结构体参数
来源：http://nu.shxzukj.cn

Ruby: f(a: 1, b: 2)
来源：http://xc.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://bk.shxzskj.cn

[C05] 返回多个值
来源：http://yd.shxzskj.cn

Py:   return a, b
来源：http://su.muxihuayi.cn

PHP:  return [$a, $b];
来源：http://rp.lnxyls.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ky.shxzskj.cn

TS:   return { a, b };
来源：http://sd.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ca.panjiajie.cn

Go:   return a, b
来源：http://il.newstarts.cn

Ruby: return a, b
来源：http://oj.lnxyls.cn

C#:   return (a, b);              // ValueTuple
来源：http://pq.szsharing.cn

[C06] 匿名函数 / lambda
来源：http://hb.huixinmuqiang.cn

Py:   square = lambda x: x * x
来源：http://jp.bjjhwx.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ue.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://kz.shxzskj.cn


<!-- 参考信息 -->