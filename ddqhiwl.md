代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://nq.shtwfgs.cn

TS:   const value = data ?? "默认值";
来源：http://fd.bjjhwx.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nv.hnjuh.cn

Go:   if data == "" { data = "默认值" }
来源：http://nu.haigaiapp.cn

Ruby: value = data || "默认值"
来源：http://ss.newstarts.cn

C#:   var value = data ?? "默认值";
来源：http://rz.yuntaijiaju.cn

[A16] 真假值判断规则
来源：http://lr.bjjhwx.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rt.szxytkj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jb.shxzskj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ua.yuntaijiaju.cn

TS:   if (!x) {}
来源：http://bk.hnjuh.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mx.szxytkj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lc.szxytkj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://sk.panjiajie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pk.wgjwhj.cn

[A17] 位运算
来源：http://km.haigaiapp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ap.shtwfgs.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wq.yuntaijiaju.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xz.chemitech.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fg.wgjwhj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ar.nicolike.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ab.szxytkj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tl.lnxyls.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://he.9csxet.cn

[A18] 字符与 ASCII 码互转
来源：http://rg.newstarts.cn

Py:   ord("A"); chr(65)
来源：http://gl.shtwfgs.cn

PHP:  ord("A"); chr(65)
来源：http://lf.szsharing.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ns.asd995.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ad.yuexingan06.cn

Java: (int) 'A'; (char) 65
来源：http://qs.huixiangedu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pu.panjiajie.cn

Ruby: "A".ord; 65.chr
来源：http://ef.shtwfgs.cn

C#:   (int)'A'; (char)65
来源：http://br.szxytkj.cn

[A19] 交换两个变量
来源：http://uq.nicolike.cn

Py:   a, b = b, a
来源：http://so.jianghongdianzi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ex.bookmarksfly.cn

JS:   [a, b] = [b, a];
来源：http://oa.huanxung.cn

TS:   [a, b] = [b, a];
来源：http://jh.colortex.cn

Java: int t = a; a = b; b = t;
来源：http://cz.hahajie.cn

Go:   a, b = b, a
来源：http://dz.haigaiapp.cn

Ruby: a, b = b, a
来源：http://lr.jianghongdianzi.cn

C#:   (a, b) = (b, a);
来源：http://wn.bjjhwx.cn

[A20] 读取标准输入
来源：http://bh.521024.cn

Py:   name = input("请输入：")
来源：http://pm.lnxyls.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://mb.nszjky.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hj.panjiajie.cn

TS:   // Node.js：readline 模块
来源：http://oj.huixinmuqiang.cn

Java: new Scanner(System.in).nextLine()
来源：http://yu.gzmigu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dn.gzmigu.cn

Ruby: gets.chomp
来源：http://wr.shxzskj.cn

C#:   Console.ReadLine();
来源：http://mw.shtwfgs.cn

[A21] 保留指定小数位输出
来源：http://sz.521024.cn

Py:   f"{3.14159:.2f}"
来源：http://ai.hahajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hr.jianghongdianzi.cn

JS:   (3.14159).toFixed(2)
来源：http://fk.muxihuayi.cn

TS:   (3.14159).toFixed(2)
来源：http://zj.shxzukj.cn

Java: String.format("%.2f", 3.14159)
来源：http://yu.wgjwhj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://uf.panjiajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://iz.shxzskj.cn

C#:   3.14159.ToString("F2")
来源：http://bn.hnjuh.cn

[A22] 获取字符串长度
来源：http://fl.jianghongdianzi.cn

Py:   len(s)
来源：http://aq.huanxung.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qb.jianghongdianzi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jt.hnjuh.cn

TS:   s.length
来源：http://df.gzmigu.cn

Java: s.length()
来源：http://vw.haigaiapp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zr.colortex.cn

Ruby: s.length
来源：http://xe.bjjhwx.cn

C#:   s.Length
来源：http://lm.szsharing.cn

[A23] 大小写转换
来源：http://wy.newstarts.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://yi.jctech888.com.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ik.yuntaijiaju.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vd.haigaiapp.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rw.jianghongdianzi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hr.bjjhwx.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://eo.9csxet.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://iz.bookmarksfly.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://iy.521024.cn

[A24] 去除首尾空白
来源：http://yy.lnxyls.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fr.nszjky.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kk.szsharing.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hx.gzmigu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://om.yuexingan06.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jk.chemitech.net.cn

Go:   strings.TrimSpace(s)
来源：http://bd.szsharing.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ls.bjjhwx.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tr.huanxung.cn

[A25] 字符串比较
来源：http://st.521024.cn

Py:   s1 == s2; s1 != s2
来源：http://sa.bookmarksfly.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gq.haigaiapp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ix.newstarts.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yx.9csxet.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fz.nicolike.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://oa.shxzukj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ww.shxzskj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ek.9csxet.cn

[A26] 类型转换总览
来源：http://gg.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://oc.bookmarksfly.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ul.jianghongdianzi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sf.huixinmuqiang.cn

TS:   Number() String() Boolean() x as number
来源：http://zc.hahajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ke.shxzukj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bg.newstarts.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rl.nszjky.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fe.nszjky.cn

================================================================================
来源：http://eg.huixiangedu.cn

B. 流程控制
来源：http://rt.shtwfgs.cn

================================================================================
来源：http://zk.huixiangedu.cn

[B01] 条件判断 if / else
来源：http://me.gzmigu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://sm.jianghongdianzi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rr.szsharing.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pi.szsharing.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gi.newstarts.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rq.haigaiapp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yt.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rf.asd995.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kt.jctech888.com.cn

[B02] 多分支 else if / elif
来源：http://mv.yuexingan06.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://se.szsharing.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ur.jctech888.com.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://si.shxzukj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jv.bjjhwx.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://va.shtwfgs.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jb.lnxyls.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dt.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jj.shxzskj.cn

[B03] switch / match / case
来源：http://sr.newstarts.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bh.huixiangedu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kt.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mp.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ho.muxihuayi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://de.hahajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nh.gzmigu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qb.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ps.panjiajie.cn

[B04] for 计数循环
来源：http://fp.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://sm.huixinmuqiang.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gc.asd995.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jo.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ep.huanxung.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qo.shxzukj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yw.muxihuayi.cn

Ruby: 10.times { |i| puts i }
来源：http://hn.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://no.huanxung.cn

[B05] 遍历数组 / 列表
来源：http://kr.szsharing.cn

Py:   for item in arr: print(item)
来源：http://uv.bookmarksfly.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lh.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yi.hnjuh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mn.bjjhwx.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mw.hahajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wg.9csxet.cn

Ruby: arr.each { |item| puts item }
来源：http://zv.asd995.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qy.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://xx.nszjky.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sf.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rc.nszjky.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mu.szsharing.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://od.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://eo.521024.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ii.huixinmuqiang.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ht.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jt.panjiajie.cn

[B07] while 循环
来源：http://ap.lnxyls.cn

Py:   while i < 10: i += 1
来源：http://om.asd995.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dh.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://iu.colortex.cn

TS:   while (i < 10) { i++; }
来源：http://pv.muxihuayi.cn

Java: while (i < 10) { i++; }
来源：http://hg.521024.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tp.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://bd.hahajie.cn

C#:   while (i < 10) { i++; }
来源：http://fi.chemitech.net.cn

[B08] do-while（至少执行一次）
来源：http://mz.bjjhwx.cn

Py:   # 无 do-while：用 while True + break
来源：http://zn.panjiajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ds.shtwfgs.cn

JS:   do { i++; } while (i < 10);
来源：http://ar.muxihuayi.cn

TS:   do { i++; } while (i < 10);
来源：http://yw.huixiangedu.cn

Java: do { i++; } while (i < 10);
来源：http://pa.jctech888.com.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pi.521024.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kd.haigaiapp.cn

C#:   do { i++; } while (i < 10);
来源：http://mb.hahajie.cn

[B09] break 与 continue
来源：http://ay.shtwfgs.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cg.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ve.haigaiapp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ft.huanxung.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fh.wgjwhj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yh.muxihuayi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gx.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sm.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://me.nszjky.cn

[B10] 遍历同时拿索引
来源：http://cn.yuntaijiaju.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qk.gzmigu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hs.yuexingan06.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tj.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rb.panjiajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gv.gzmigu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ma.chemitech.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ce.muxihuayi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jf.shxzskj.cn

[B11] 生成数字序列 / 区间
来源：http://xk.jctech888.com.cn

Py:   list(range(0, 10, 2))
来源：http://tb.szxytkj.cn

PHP:  range(0, 10, 2);
来源：http://yj.bjjhwx.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kq.huixinmuqiang.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vu.hnjuh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tn.nszjky.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lb.jctech888.com.cn

Ruby: (0...10).step(2).to_a
来源：http://ew.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fp.jianghongdianzi.cn

[B12] 跳出多层循环
来源：http://wg.hnjuh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ks.shxzskj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://im.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bn.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qi.shxzukj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ks.huixiangedu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://af.haigaiapp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qc.lnxyls.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sl.nicolike.cn

[B13] 判断是否为数字
来源：http://mc.colortex.cn

Py:   isinstance(x, (int, float))
来源：http://vc.wgjwhj.cn

PHP:  is_numeric($x)
来源：http://ce.haigaiapp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://po.hahajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gs.chemitech.net.cn

Java: x instanceof Number
来源：http://cu.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lm.nicolike.cn

Ruby: x.is_a?(Numeric)
来源：http://ma.shxzskj.cn

C#:   x is int or double or decimal
来源：http://us.521024.cn

[B14] 判断值是否在集合内
来源：http://db.nicolike.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pp.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xl.bjjhwx.cn

JS:   [1, 2, 3].includes(x)
来源：http://uk.shxzukj.cn

TS:   [1, 2, 3].includes(x)
来源：http://jv.haigaiapp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vr.huixinmuqiang.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vl.huanxung.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jn.huixiangedu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://da.panjiajie.cn

[B15] 布尔运算与取反
来源：http://pr.lnxyls.cn

Py:   a and b or not c
来源：http://ni.haigaiapp.cn

PHP:  $a && $b || !$c
来源：http://fw.jctech888.com.cn

JS:   a && b || !c
来源：http://aq.bjjhwx.cn

TS:   a && b || !c
来源：http://cj.newstarts.cn

Java: a && b || !c
来源：http://ft.panjiajie.cn

Go:   a && b || !c
来源：http://xk.huixinmuqiang.cn

Ruby: a && b || !c
来源：http://kp.bjjhwx.cn

C#:   a && b || !c
来源：http://fz.yuexingan06.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qf.szxytkj.cn

Py:   if not data: return
来源：http://wd.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://qz.haigaiapp.cn

JS:   if (!data) return;
来源：http://cl.panjiajie.cn

TS:   if (!data) return;
来源：http://ms.lnxyls.cn

Java: if (data == null) return;
来源：http://jj.huixinmuqiang.cn

Go:   if data == nil { return }
来源：http://fh.colortex.cn

Ruby: return if data.nil?
来源：http://ar.chemitech.net.cn

C#:   if (data == null) return;
来源：http://jz.asd995.cn

================================================================================
来源：http://pq.szsharing.cn

C. 函数与作用域
来源：http://xz.muxihuayi.cn

================================================================================
来源：http://kx.asd995.cn

[C01] 定义函数
来源：http://rq.newstarts.cn

Py:   def add(a, b): return a + b
来源：http://qq.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vz.jctech888.com.cn

JS:   function add(a, b) { return a + b; }
来源：http://le.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zm.szsharing.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fp.shtwfgs.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tm.shxzskj.cn

Ruby: def add(a, b); a + b; end
来源：http://lp.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cx.yuexingan06.cn

[C02] 默认参数
来源：http://pn.hahajie.cn

Py:   def greet(name="World"): return name
来源：http://ze.nicolike.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://og.huanxung.cn

JS:   function greet(name = "World") { return name; }
来源：http://bk.panjiajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ym.chemitech.net.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cn.shxzskj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nk.huixinmuqiang.cn

Ruby: def greet(name = "World") = name
来源：http://gk.jctech888.com.cn

C#:   string Greet(string name = "World") => name;
来源：http://sj.panjiajie.cn

[C03] 可变参数
来源：http://kh.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://me.hahajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tq.521024.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qw.jianghongdianzi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pr.asd995.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://no.muxihuayi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rz.521024.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wg.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wt.hnjuh.cn

[C04] 命名参数 / 关键字参数
来源：http://bm.asd995.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hw.521024.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vx.huanxung.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rj.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kj.huixinmuqiang.cn

Java: // 无：用 Builder 模式或 record
来源：http://bq.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://ow.nicolike.cn

Ruby: f(a: 1, b: 2)
来源：http://wz.gzmigu.cn

C#:   f(a: 1, b: 2)
来源：http://wc.lnxyls.cn

[C05] 返回多个值
来源：http://mm.shtwfgs.cn

Py:   return a, b
来源：http://uo.9csxet.cn

PHP:  return [$a, $b];
来源：http://di.shtwfgs.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://po.colortex.cn

TS:   return { a, b };
来源：http://ae.521024.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mm.lnxyls.cn

Go:   return a, b
来源：http://we.huixiangedu.cn

Ruby: return a, b
来源：http://th.hnjuh.cn

C#:   return (a, b);              // ValueTuple
来源：http://jl.bjjhwx.cn


<!-- 参考信息 -->