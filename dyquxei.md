代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://vq.huixiangedu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://sj.hnjuh.cn

Go:   // 单行；/* 多行 */
来源：http://wz.bjjhwx.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ww.shxzskj.cn

C#:   // 单行；/* 多行 */
来源：http://kz.huixinmuqiang.cn

[A15] 空值判断与默认值
来源：http://ay.jianghongdianzi.cn

Py:   value = data or "默认值"
来源：http://nn.haigaiapp.cn

PHP:  $value = $data ?? "默认值";
来源：http://tv.chemitech.net.cn

JS:   const value = data ?? "默认值";
来源：http://ue.wgjwhj.cn

TS:   const value = data ?? "默认值";
来源：http://tv.yuntaijiaju.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pr.hahajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://np.jctech888.com.cn

Ruby: value = data || "默认值"
来源：http://ph.9csxet.cn

C#:   var value = data ?? "默认值";
来源：http://sp.hahajie.cn

[A16] 真假值判断规则
来源：http://jz.nszjky.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kl.hnjuh.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hd.haigaiapp.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://iz.9csxet.cn

TS:   if (!x) {}
来源：http://jo.newstarts.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nt.colortex.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://me.szsharing.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ah.colortex.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://co.9csxet.cn

[A17] 位运算
来源：http://zf.jianghongdianzi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hr.haigaiapp.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rw.bookmarksfly.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qv.bookmarksfly.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wy.shtwfgs.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xh.yuexingan06.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://va.chemitech.net.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gs.newstarts.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fe.huixiangedu.cn

[A18] 字符与 ASCII 码互转
来源：http://zs.lnxyls.cn

Py:   ord("A"); chr(65)
来源：http://xd.bookmarksfly.cn

PHP:  ord("A"); chr(65)
来源：http://xm.jianghongdianzi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ph.szxytkj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pg.nicolike.cn

Java: (int) 'A'; (char) 65
来源：http://vt.gzmigu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dv.hnjuh.cn

Ruby: "A".ord; 65.chr
来源：http://st.huixinmuqiang.cn

C#:   (int)'A'; (char)65
来源：http://zi.shtwfgs.cn

[A19] 交换两个变量
来源：http://vk.yuexingan06.cn

Py:   a, b = b, a
来源：http://ts.szxytkj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qo.huixinmuqiang.cn

JS:   [a, b] = [b, a];
来源：http://wv.9csxet.cn

TS:   [a, b] = [b, a];
来源：http://ns.bookmarksfly.cn

Java: int t = a; a = b; b = t;
来源：http://zl.shxzskj.cn

Go:   a, b = b, a
来源：http://jo.haigaiapp.cn

Ruby: a, b = b, a
来源：http://wb.huixinmuqiang.cn

C#:   (a, b) = (b, a);
来源：http://fl.nszjky.cn

[A20] 读取标准输入
来源：http://uf.shxzskj.cn

Py:   name = input("请输入：")
来源：http://ac.panjiajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://bl.szsharing.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ea.jctech888.com.cn

TS:   // Node.js：readline 模块
来源：http://uv.9csxet.cn

Java: new Scanner(System.in).nextLine()
来源：http://gy.huixinmuqiang.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ny.lnxyls.cn

Ruby: gets.chomp
来源：http://zb.huixiangedu.cn

C#:   Console.ReadLine();
来源：http://ge.huanxung.cn

[A21] 保留指定小数位输出
来源：http://ba.yuexingan06.cn

Py:   f"{3.14159:.2f}"
来源：http://jj.hnjuh.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ig.huanxung.cn

JS:   (3.14159).toFixed(2)
来源：http://ol.huixiangedu.cn

TS:   (3.14159).toFixed(2)
来源：http://xn.nicolike.cn

Java: String.format("%.2f", 3.14159)
来源：http://um.panjiajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ur.yuexingan06.cn

Ruby: format("%.2f", 3.14159)
来源：http://xs.shxzukj.cn

C#:   3.14159.ToString("F2")
来源：http://af.huixiangedu.cn

[A22] 获取字符串长度
来源：http://qr.szxytkj.cn

Py:   len(s)
来源：http://lo.wgjwhj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rd.jctech888.com.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://eg.shxzukj.cn

TS:   s.length
来源：http://hv.wgjwhj.cn

Java: s.length()
来源：http://px.haigaiapp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ks.yuntaijiaju.cn

Ruby: s.length
来源：http://ks.shxzskj.cn

C#:   s.Length
来源：http://ej.huixiangedu.cn

[A23] 大小写转换
来源：http://uy.chemitech.net.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vh.wgjwhj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cs.newstarts.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ok.szxytkj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qb.yuntaijiaju.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://oe.jctech888.com.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cs.yuntaijiaju.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://oz.szxytkj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://kb.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://vm.nicolike.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vb.newstarts.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sn.lnxyls.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lq.huixiangedu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ok.huixiangedu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zt.szxytkj.cn

Go:   strings.TrimSpace(s)
来源：http://tn.haigaiapp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jd.gzmigu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nk.jctech888.com.cn

[A25] 字符串比较
来源：http://wj.szxytkj.cn

Py:   s1 == s2; s1 != s2
来源：http://ve.chemitech.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gx.bookmarksfly.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bd.panjiajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://il.huixinmuqiang.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yd.hnjuh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ka.hnjuh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://du.wgjwhj.cn

[A26] 类型转换总览
来源：http://fe.szxytkj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vr.bookmarksfly.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uq.jctech888.com.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hd.shxzskj.cn

TS:   Number() String() Boolean() x as number
来源：http://kb.hnjuh.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qe.colortex.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ia.9csxet.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mn.hnjuh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ei.jctech888.com.cn

================================================================================
来源：http://kf.bookmarksfly.cn

B. 流程控制
来源：http://rq.bjjhwx.cn

================================================================================
来源：http://yt.521024.cn

[B01] 条件判断 if / else
来源：http://jd.gzmigu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ys.muxihuayi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lu.huanxung.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dh.shxzukj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ic.huixinmuqiang.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cd.muxihuayi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kv.colortex.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vq.bjjhwx.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wt.jianghongdianzi.cn

[B02] 多分支 else if / elif
来源：http://to.huanxung.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wk.haigaiapp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xh.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ka.hnjuh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rf.haigaiapp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ma.jianghongdianzi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fe.yuexingan06.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gg.hahajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://af.panjiajie.cn

[B03] switch / match / case
来源：http://hn.colortex.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zy.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pf.huixinmuqiang.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ne.wgjwhj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uv.colortex.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nw.bookmarksfly.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://az.hahajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ze.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hc.hahajie.cn

[B04] for 计数循环
来源：http://jp.muxihuayi.cn

Py:   for i in range(10): print(i)
来源：http://rg.haigaiapp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ka.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zb.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ul.jctech888.com.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jo.szxytkj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://il.panjiajie.cn

Ruby: 10.times { |i| puts i }
来源：http://pr.haigaiapp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mx.nicolike.cn

[B05] 遍历数组 / 列表
来源：http://rg.gzmigu.cn

Py:   for item in arr: print(item)
来源：http://qj.huixiangedu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qy.asd995.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bh.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://iz.colortex.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xv.521024.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yf.bjjhwx.cn

Ruby: arr.each { |item| puts item }
来源：http://zq.asd995.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fy.shxzskj.cn

[B06] 遍历字典 / 对象
来源：http://wk.lnxyls.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ne.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ua.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://na.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lt.jianghongdianzi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bt.haigaiapp.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qh.shxzskj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rp.jctech888.com.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://iz.haigaiapp.cn

[B07] while 循环
来源：http://re.colortex.cn

Py:   while i < 10: i += 1
来源：http://ax.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://by.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://mw.gzmigu.cn

TS:   while (i < 10) { i++; }
来源：http://rx.shxzukj.cn

Java: while (i < 10) { i++; }
来源：http://fc.521024.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pv.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://zc.haigaiapp.cn

C#:   while (i < 10) { i++; }
来源：http://vz.521024.cn

[B08] do-while（至少执行一次）
来源：http://qy.hnjuh.cn

Py:   # 无 do-while：用 while True + break
来源：http://fi.wgjwhj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bf.szxytkj.cn

JS:   do { i++; } while (i < 10);
来源：http://mp.yuntaijiaju.cn

TS:   do { i++; } while (i < 10);
来源：http://uw.wgjwhj.cn

Java: do { i++; } while (i < 10);
来源：http://ps.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://lt.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bl.huixinmuqiang.cn

C#:   do { i++; } while (i < 10);
来源：http://kn.nszjky.cn

[B09] break 与 continue
来源：http://cy.muxihuayi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kw.huanxung.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rt.9csxet.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gd.shxzskj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vu.muxihuayi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bq.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uu.nicolike.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ru.9csxet.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ab.jianghongdianzi.cn

[B10] 遍历同时拿索引
来源：http://ef.nszjky.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tq.hahajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bk.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zp.newstarts.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ec.wgjwhj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wa.asd995.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uv.szsharing.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://re.gzmigu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dk.huixinmuqiang.cn

[B11] 生成数字序列 / 区间
来源：http://zi.bjjhwx.cn

Py:   list(range(0, 10, 2))
来源：http://lb.nszjky.cn

PHP:  range(0, 10, 2);
来源：http://um.panjiajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lo.szsharing.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ho.521024.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ru.haigaiapp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fb.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://qk.hahajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nc.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://je.hnjuh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ro.chemitech.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ik.szsharing.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lc.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fp.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fi.shtwfgs.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dm.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sl.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rs.colortex.cn

[B13] 判断是否为数字
来源：http://qk.szsharing.cn

Py:   isinstance(x, (int, float))
来源：http://uj.bookmarksfly.cn

PHP:  is_numeric($x)
来源：http://ju.szxytkj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://se.hahajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ew.jctech888.com.cn

Java: x instanceof Number
来源：http://yq.huixinmuqiang.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pv.yuexingan06.cn

Ruby: x.is_a?(Numeric)
来源：http://bf.nszjky.cn

C#:   x is int or double or decimal
来源：http://ow.huixinmuqiang.cn

[B14] 判断值是否在集合内
来源：http://xu.shxzskj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ay.yuntaijiaju.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ob.nszjky.cn

JS:   [1, 2, 3].includes(x)
来源：http://br.shxzukj.cn

TS:   [1, 2, 3].includes(x)
来源：http://ia.haigaiapp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://tu.hnjuh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://et.gzmigu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://th.newstarts.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qa.gzmigu.cn

[B15] 布尔运算与取反
来源：http://za.huixiangedu.cn

Py:   a and b or not c
来源：http://fo.jctech888.com.cn

PHP:  $a && $b || !$c
来源：http://mg.nszjky.cn

JS:   a && b || !c
来源：http://gx.9csxet.cn

TS:   a && b || !c
来源：http://uc.shxzukj.cn

Java: a && b || !c
来源：http://ib.shxzukj.cn

Go:   a && b || !c
来源：http://qx.shxzskj.cn

Ruby: a && b || !c
来源：http://ap.newstarts.cn

C#:   a && b || !c
来源：http://nc.asd995.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vp.panjiajie.cn

Py:   if not data: return
来源：http://of.wgjwhj.cn

PHP:  if (!$data) { return; }
来源：http://so.huixiangedu.cn

JS:   if (!data) return;
来源：http://lf.shxzskj.cn

TS:   if (!data) return;
来源：http://gb.chemitech.net.cn

Java: if (data == null) return;
来源：http://fs.chemitech.net.cn

Go:   if data == nil { return }
来源：http://mk.huanxung.cn

Ruby: return if data.nil?
来源：http://at.szxytkj.cn

C#:   if (data == null) return;
来源：http://nu.521024.cn

================================================================================
来源：http://pk.nszjky.cn

C. 函数与作用域
来源：http://aa.chemitech.net.cn

================================================================================
来源：http://kd.haigaiapp.cn

[C01] 定义函数
来源：http://vq.newstarts.cn

Py:   def add(a, b): return a + b
来源：http://xg.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lf.wgjwhj.cn

JS:   function add(a, b) { return a + b; }
来源：http://lb.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://og.huixiangedu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rv.hnjuh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gj.huixiangedu.cn

Ruby: def add(a, b); a + b; end
来源：http://lx.hahajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mq.colortex.cn

[C02] 默认参数
来源：http://hd.lnxyls.cn

Py:   def greet(name="World"): return name
来源：http://rg.chemitech.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://au.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://bz.hahajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://uw.panjiajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lc.szsharing.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ct.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://jx.bjjhwx.cn

C#:   string Greet(string name = "World") => name;
来源：http://me.hahajie.cn

[C03] 可变参数
来源：http://ry.chemitech.net.cn

Py:   def total(*args): return sum(args)
来源：http://yk.yuexingan06.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://px.asd995.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://id.9csxet.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gw.panjiajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dh.jianghongdianzi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xe.jianghongdianzi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qp.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qt.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://nx.hnjuh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ir.asd995.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://es.muxihuayi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pk.yuexingan06.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qs.asd995.cn

Java: // 无：用 Builder 模式或 record
来源：http://ao.bjjhwx.cn

Go:   // 无：用配置结构体参数
来源：http://tr.shxzukj.cn

Ruby: f(a: 1, b: 2)
来源：http://ur.szxytkj.cn

C#:   f(a: 1, b: 2)
来源：http://ya.gzmigu.cn

[C05] 返回多个值
来源：http://ve.nszjky.cn


<!-- 参考信息 -->