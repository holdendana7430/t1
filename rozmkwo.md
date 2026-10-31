代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://te.wgjwhj.cn

[A15] 空值判断与默认值
来源：http://hs.yuexingan06.cn

Py:   value = data or "默认值"
来源：http://cs.nicolike.cn

PHP:  $value = $data ?? "默认值";
来源：http://gj.bjjhwx.cn

JS:   const value = data ?? "默认值";
来源：http://pk.shxzukj.cn

TS:   const value = data ?? "默认值";
来源：http://aa.chemitech.net.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bp.huixiangedu.cn

Go:   if data == "" { data = "默认值" }
来源：http://cn.huixinmuqiang.cn

Ruby: value = data || "默认值"
来源：http://yu.jianghongdianzi.cn

C#:   var value = data ?? "默认值";
来源：http://fa.huixiangedu.cn

[A16] 真假值判断规则
来源：http://fw.yuntaijiaju.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cr.huanxung.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ug.newstarts.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://so.bjjhwx.cn

TS:   if (!x) {}
来源：http://ks.newstarts.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://oy.shxzukj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lt.huixinmuqiang.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hn.huanxung.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sx.yuntaijiaju.cn

[A17] 位运算
来源：http://mv.chemitech.net.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ki.hnjuh.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://yp.colortex.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gj.bjjhwx.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jj.wgjwhj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://by.panjiajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dd.521024.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ui.jianghongdianzi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ad.haigaiapp.cn

[A18] 字符与 ASCII 码互转
来源：http://la.lnxyls.cn

Py:   ord("A"); chr(65)
来源：http://rt.asd995.cn

PHP:  ord("A"); chr(65)
来源：http://im.hahajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qn.newstarts.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jo.yuexingan06.cn

Java: (int) 'A'; (char) 65
来源：http://gc.huixinmuqiang.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hq.szsharing.cn

Ruby: "A".ord; 65.chr
来源：http://ha.yuntaijiaju.cn

C#:   (int)'A'; (char)65
来源：http://wn.shxzukj.cn

[A19] 交换两个变量
来源：http://ww.jctech888.com.cn

Py:   a, b = b, a
来源：http://vj.colortex.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tn.jianghongdianzi.cn

JS:   [a, b] = [b, a];
来源：http://af.colortex.cn

TS:   [a, b] = [b, a];
来源：http://jq.huanxung.cn

Java: int t = a; a = b; b = t;
来源：http://pn.colortex.cn

Go:   a, b = b, a
来源：http://lz.shxzskj.cn

Ruby: a, b = b, a
来源：http://rk.lnxyls.cn

C#:   (a, b) = (b, a);
来源：http://vk.gzmigu.cn

[A20] 读取标准输入
来源：http://wp.szxytkj.cn

Py:   name = input("请输入：")
来源：http://tv.nicolike.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://et.haigaiapp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mf.hnjuh.cn

TS:   // Node.js：readline 模块
来源：http://no.szsharing.cn

Java: new Scanner(System.in).nextLine()
来源：http://rz.asd995.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qm.gzmigu.cn

Ruby: gets.chomp
来源：http://rm.hnjuh.cn

C#:   Console.ReadLine();
来源：http://ow.chemitech.net.cn

[A21] 保留指定小数位输出
来源：http://ox.bjjhwx.cn

Py:   f"{3.14159:.2f}"
来源：http://yk.muxihuayi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rx.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://nf.huixinmuqiang.cn

TS:   (3.14159).toFixed(2)
来源：http://kc.shxzskj.cn

Java: String.format("%.2f", 3.14159)
来源：http://mh.lnxyls.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fe.haigaiapp.cn

Ruby: format("%.2f", 3.14159)
来源：http://ry.asd995.cn

C#:   3.14159.ToString("F2")
来源：http://cg.panjiajie.cn

[A22] 获取字符串长度
来源：http://zl.jctech888.com.cn

Py:   len(s)
来源：http://tz.hahajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://en.hnjuh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lw.newstarts.cn

TS:   s.length
来源：http://ad.muxihuayi.cn

Java: s.length()
来源：http://ze.muxihuayi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://op.haigaiapp.cn

Ruby: s.length
来源：http://ui.yuexingan06.cn

C#:   s.Length
来源：http://an.521024.cn

[A23] 大小写转换
来源：http://lu.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://pa.lnxyls.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fy.hahajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://iy.yuntaijiaju.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://st.jianghongdianzi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zg.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qp.szsharing.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xh.newstarts.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ww.szxytkj.cn

[A24] 去除首尾空白
来源：http://ak.haigaiapp.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pa.chemitech.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bk.colortex.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://go.hahajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fp.huanxung.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wq.colortex.cn

Go:   strings.TrimSpace(s)
来源：http://bw.muxihuayi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xi.lnxyls.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://an.9csxet.cn

[A25] 字符串比较
来源：http://lg.colortex.cn

Py:   s1 == s2; s1 != s2
来源：http://ej.szxytkj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wy.jctech888.com.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://oa.haigaiapp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ws.muxihuayi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sa.wgjwhj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pw.wgjwhj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tu.huixinmuqiang.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fi.shxzskj.cn

[A26] 类型转换总览
来源：http://eh.wgjwhj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ad.huixiangedu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ff.huixiangedu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pe.asd995.cn

TS:   Number() String() Boolean() x as number
来源：http://rr.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ji.nicolike.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ii.jctech888.com.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bk.yuexingan06.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ee.yuntaijiaju.cn

================================================================================
来源：http://fc.jctech888.com.cn

B. 流程控制
来源：http://ms.szsharing.cn

================================================================================
来源：http://nj.huixiangedu.cn

[B01] 条件判断 if / else
来源：http://zt.jianghongdianzi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zq.wgjwhj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://si.hahajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bs.asd995.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ba.huixinmuqiang.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ul.jctech888.com.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rf.nszjky.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lq.szsharing.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ih.nszjky.cn

[B02] 多分支 else if / elif
来源：http://hs.colortex.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tf.newstarts.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ef.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uf.hnjuh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cp.shxzskj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zg.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xd.szxytkj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cg.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kw.szxytkj.cn

[B03] switch / match / case
来源：http://ve.lnxyls.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nl.521024.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://eq.jctech888.com.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zm.bjjhwx.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://au.hahajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ji.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ql.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qv.wgjwhj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nk.huixinmuqiang.cn

[B04] for 计数循环
来源：http://or.huanxung.cn

Py:   for i in range(10): print(i)
来源：http://te.huixiangedu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lw.szxytkj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://st.huanxung.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vu.newstarts.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mv.9csxet.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rm.chemitech.net.cn

Ruby: 10.times { |i| puts i }
来源：http://wh.huixiangedu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pm.newstarts.cn

[B05] 遍历数组 / 列表
来源：http://bv.jianghongdianzi.cn

Py:   for item in arr: print(item)
来源：http://bi.nicolike.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nd.bjjhwx.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gl.wgjwhj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ck.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zb.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://az.haigaiapp.cn

Ruby: arr.each { |item| puts item }
来源：http://zq.hnjuh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://au.521024.cn

[B06] 遍历字典 / 对象
来源：http://kb.shxzukj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gj.9csxet.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nu.huixiangedu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kw.muxihuayi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fb.chemitech.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oo.hnjuh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ba.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pp.muxihuayi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sm.colortex.cn

[B07] while 循环
来源：http://df.szsharing.cn

Py:   while i < 10: i += 1
来源：http://ak.shxzukj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://et.muxihuayi.cn

JS:   while (i < 10) { i++; }
来源：http://hk.gzmigu.cn

TS:   while (i < 10) { i++; }
来源：http://au.panjiajie.cn

Java: while (i < 10) { i++; }
来源：http://mj.muxihuayi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fx.huixinmuqiang.cn

Ruby: while i < 10; i += 1; end
来源：http://ij.lnxyls.cn

C#:   while (i < 10) { i++; }
来源：http://wl.colortex.cn

[B08] do-while（至少执行一次）
来源：http://ri.szxytkj.cn

Py:   # 无 do-while：用 while True + break
来源：http://vr.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fc.haigaiapp.cn

JS:   do { i++; } while (i < 10);
来源：http://xp.hnjuh.cn

TS:   do { i++; } while (i < 10);
来源：http://ly.9csxet.cn

Java: do { i++; } while (i < 10);
来源：http://nf.nszjky.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ev.bjjhwx.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ag.shxzskj.cn

C#:   do { i++; } while (i < 10);
来源：http://bu.shtwfgs.cn

[B09] break 与 continue
来源：http://fd.nicolike.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ix.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://db.huanxung.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fx.huanxung.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sf.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ge.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://de.jctech888.com.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ih.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oq.yuntaijiaju.cn

[B10] 遍历同时拿索引
来源：http://vc.bookmarksfly.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://no.asd995.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://in.shtwfgs.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xw.lnxyls.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oa.shtwfgs.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wt.bjjhwx.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vw.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tz.yuntaijiaju.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pi.bjjhwx.cn

[B11] 生成数字序列 / 区间
来源：http://wv.shtwfgs.cn

Py:   list(range(0, 10, 2))
来源：http://jd.szxytkj.cn

PHP:  range(0, 10, 2);
来源：http://xd.jianghongdianzi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bu.gzmigu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dl.hahajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pu.szxytkj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fg.nicolike.cn

Ruby: (0...10).step(2).to_a
来源：http://sd.jianghongdianzi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wb.szxytkj.cn

[B12] 跳出多层循环
来源：http://ia.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ao.shxzskj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://td.chemitech.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mk.newstarts.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://we.newstarts.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fg.521024.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ct.jianghongdianzi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gb.yuexingan06.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ef.9csxet.cn

[B13] 判断是否为数字
来源：http://ls.shxzskj.cn

Py:   isinstance(x, (int, float))
来源：http://kx.hnjuh.cn

PHP:  is_numeric($x)
来源：http://qq.newstarts.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gz.haigaiapp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ld.newstarts.cn

Java: x instanceof Number
来源：http://vf.huanxung.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gc.muxihuayi.cn

Ruby: x.is_a?(Numeric)
来源：http://ox.newstarts.cn

C#:   x is int or double or decimal
来源：http://vr.hnjuh.cn

[B14] 判断值是否在集合内
来源：http://ax.lnxyls.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bp.szxytkj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lk.hahajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://kh.521024.cn

TS:   [1, 2, 3].includes(x)
来源：http://iy.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xt.newstarts.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pj.hahajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qw.shxzukj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uw.huixiangedu.cn

[B15] 布尔运算与取反
来源：http://oz.huanxung.cn

Py:   a and b or not c
来源：http://tn.bjjhwx.cn

PHP:  $a && $b || !$c
来源：http://fn.bookmarksfly.cn

JS:   a && b || !c
来源：http://yt.chemitech.net.cn

TS:   a && b || !c
来源：http://ij.9csxet.cn

Java: a && b || !c
来源：http://qi.haigaiapp.cn

Go:   a && b || !c
来源：http://kk.huixiangedu.cn

Ruby: a && b || !c
来源：http://ma.hnjuh.cn

C#:   a && b || !c
来源：http://na.wgjwhj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wa.jianghongdianzi.cn

Py:   if not data: return
来源：http://xv.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://td.shxzukj.cn

JS:   if (!data) return;
来源：http://kz.yuexingan06.cn

TS:   if (!data) return;
来源：http://mk.bookmarksfly.cn

Java: if (data == null) return;
来源：http://wr.colortex.cn

Go:   if data == nil { return }
来源：http://ai.lnxyls.cn

Ruby: return if data.nil?
来源：http://ff.hahajie.cn

C#:   if (data == null) return;
来源：http://eb.yuntaijiaju.cn

================================================================================
来源：http://wv.yuntaijiaju.cn

C. 函数与作用域
来源：http://ok.muxihuayi.cn

================================================================================
来源：http://ej.shxzskj.cn

[C01] 定义函数
来源：http://yl.nicolike.cn

Py:   def add(a, b): return a + b
来源：http://ii.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kz.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://it.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lu.yuexingan06.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gl.gzmigu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ve.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://rh.bookmarksfly.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yy.huixiangedu.cn

[C02] 默认参数
来源：http://ti.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://nt.huanxung.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://th.shxzukj.cn

JS:   function greet(name = "World") { return name; }
来源：http://ww.huanxung.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hu.lnxyls.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ae.haigaiapp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dp.shxzukj.cn

Ruby: def greet(name = "World") = name
来源：http://bm.wgjwhj.cn

C#:   string Greet(string name = "World") => name;
来源：http://lh.jctech888.com.cn

[C03] 可变参数
来源：http://ws.gzmigu.cn

Py:   def total(*args): return sum(args)
来源：http://rs.shxzskj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zu.hnjuh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yd.9csxet.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fa.521024.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://um.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vx.colortex.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nm.yuexingan06.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wj.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://rh.jctech888.com.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mt.huixinmuqiang.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pn.521024.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tw.hnjuh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gu.szsharing.cn

Java: // 无：用 Builder 模式或 record
来源：http://xr.panjiajie.cn

Go:   // 无：用配置结构体参数
来源：http://dl.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://ph.nicolike.cn

C#:   f(a: 1, b: 2)
来源：http://nd.muxihuayi.cn

[C05] 返回多个值
来源：http://fd.jianghongdianzi.cn

Py:   return a, b
来源：http://yw.lnxyls.cn

PHP:  return [$a, $b];
来源：http://vq.jianghongdianzi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xh.muxihuayi.cn

TS:   return { a, b };
来源：http://ow.shtwfgs.cn


<!-- 参考信息 -->