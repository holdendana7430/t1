代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://bj.muxihuayi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lq.haigaiapp.cn

Go:   // 单行；/* 多行 */
来源：http://pu.shxzukj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://bp.newstarts.cn

C#:   // 单行；/* 多行 */
来源：http://nm.bookmarksfly.cn

[A15] 空值判断与默认值
来源：http://oz.nicolike.cn

Py:   value = data or "默认值"
来源：http://xy.wgjwhj.cn

PHP:  $value = $data ?? "默认值";
来源：http://jj.szxytkj.cn

JS:   const value = data ?? "默认值";
来源：http://xu.jctech888.com.cn

TS:   const value = data ?? "默认值";
来源：http://dr.lnxyls.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xh.haigaiapp.cn

Go:   if data == "" { data = "默认值" }
来源：http://cg.muxihuayi.cn

Ruby: value = data || "默认值"
来源：http://la.hnjuh.cn

C#:   var value = data ?? "默认值";
来源：http://kd.szsharing.cn

[A16] 真假值判断规则
来源：http://ns.chemitech.net.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://va.huanxung.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://en.shxzskj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xk.hnjuh.cn

TS:   if (!x) {}
来源：http://dv.huixinmuqiang.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hl.shtwfgs.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ea.bookmarksfly.cn

Ruby: unless x            # nil 与 false 为假
来源：http://yl.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ry.shxzskj.cn

[A17] 位运算
来源：http://kx.panjiajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gh.muxihuayi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vx.newstarts.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uy.lnxyls.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://sb.bookmarksfly.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sl.newstarts.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://em.lnxyls.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jd.nszjky.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ef.colortex.cn

[A18] 字符与 ASCII 码互转
来源：http://pq.521024.cn

Py:   ord("A"); chr(65)
来源：http://wm.jctech888.com.cn

PHP:  ord("A"); chr(65)
来源：http://it.jctech888.com.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zk.muxihuayi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wj.9csxet.cn

Java: (int) 'A'; (char) 65
来源：http://ex.chemitech.net.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qy.9csxet.cn

Ruby: "A".ord; 65.chr
来源：http://iq.hnjuh.cn

C#:   (int)'A'; (char)65
来源：http://ao.szsharing.cn

[A19] 交换两个变量
来源：http://tl.huixiangedu.cn

Py:   a, b = b, a
来源：http://yj.nszjky.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://df.jctech888.com.cn

JS:   [a, b] = [b, a];
来源：http://zn.muxihuayi.cn

TS:   [a, b] = [b, a];
来源：http://dm.jctech888.com.cn

Java: int t = a; a = b; b = t;
来源：http://xe.wgjwhj.cn

Go:   a, b = b, a
来源：http://hm.nszjky.cn

Ruby: a, b = b, a
来源：http://kn.shxzskj.cn

C#:   (a, b) = (b, a);
来源：http://qg.bjjhwx.cn

[A20] 读取标准输入
来源：http://vb.shtwfgs.cn

Py:   name = input("请输入：")
来源：http://je.hnjuh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://bz.muxihuayi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lt.bookmarksfly.cn

TS:   // Node.js：readline 模块
来源：http://hy.shtwfgs.cn

Java: new Scanner(System.in).nextLine()
来源：http://ai.hnjuh.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://to.9csxet.cn

Ruby: gets.chomp
来源：http://ll.asd995.cn

C#:   Console.ReadLine();
来源：http://mz.bookmarksfly.cn

[A21] 保留指定小数位输出
来源：http://yu.colortex.cn

Py:   f"{3.14159:.2f}"
来源：http://il.jctech888.com.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ca.wgjwhj.cn

JS:   (3.14159).toFixed(2)
来源：http://xe.huanxung.cn

TS:   (3.14159).toFixed(2)
来源：http://ex.shxzskj.cn

Java: String.format("%.2f", 3.14159)
来源：http://eu.nszjky.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rw.chemitech.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://bb.shxzskj.cn

C#:   3.14159.ToString("F2")
来源：http://da.szsharing.cn

[A22] 获取字符串长度
来源：http://he.gzmigu.cn

Py:   len(s)
来源：http://vz.newstarts.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zy.huixiangedu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mr.szsharing.cn

TS:   s.length
来源：http://co.jianghongdianzi.cn

Java: s.length()
来源：http://og.jianghongdianzi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ok.lnxyls.cn

Ruby: s.length
来源：http://or.bookmarksfly.cn

C#:   s.Length
来源：http://gd.gzmigu.cn

[A23] 大小写转换
来源：http://ix.yuexingan06.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://lo.colortex.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mw.9csxet.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://os.shxzskj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ci.szsharing.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bb.yuntaijiaju.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cl.szsharing.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ud.shtwfgs.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ns.yuexingan06.cn

[A24] 去除首尾空白
来源：http://fi.lnxyls.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://to.wgjwhj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yv.gzmigu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kn.yuntaijiaju.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kk.asd995.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://br.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://lx.jianghongdianzi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vx.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hk.wgjwhj.cn

[A25] 字符串比较
来源：http://wl.huixinmuqiang.cn

Py:   s1 == s2; s1 != s2
来源：http://os.yuexingan06.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://as.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ga.huixiangedu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://db.521024.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ss.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vx.huixiangedu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hs.panjiajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://om.chemitech.net.cn

[A26] 类型转换总览
来源：http://gt.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rp.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ws.jianghongdianzi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bj.jctech888.com.cn

TS:   Number() String() Boolean() x as number
来源：http://ob.lnxyls.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qw.muxihuayi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://st.jctech888.com.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://iz.panjiajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kz.szxytkj.cn

================================================================================
来源：http://bg.nszjky.cn

B. 流程控制
来源：http://aj.huanxung.cn

================================================================================
来源：http://cb.9csxet.cn

[B01] 条件判断 if / else
来源：http://dc.nszjky.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://uv.szxytkj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qg.szsharing.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xg.bjjhwx.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://st.hnjuh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ra.shxzukj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tt.huanxung.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rr.9csxet.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nw.asd995.cn

[B02] 多分支 else if / elif
来源：http://ru.shxzukj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dq.hnjuh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ph.asd995.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gt.huixinmuqiang.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yo.szxytkj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tj.9csxet.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nf.szxytkj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ue.bookmarksfly.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://we.wgjwhj.cn

[B03] switch / match / case
来源：http://xr.521024.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mb.shxzskj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nj.yuntaijiaju.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yf.hnjuh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kb.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dl.nszjky.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xh.shxzukj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hh.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ie.hahajie.cn

[B04] for 计数循环
来源：http://ly.bjjhwx.cn

Py:   for i in range(10): print(i)
来源：http://xs.yuntaijiaju.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://en.nicolike.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wq.asd995.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ca.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lv.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pl.jianghongdianzi.cn

Ruby: 10.times { |i| puts i }
来源：http://ny.shtwfgs.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xq.wgjwhj.cn

[B05] 遍历数组 / 列表
来源：http://va.asd995.cn

Py:   for item in arr: print(item)
来源：http://ni.newstarts.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jb.gzmigu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gx.shxzskj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yj.jianghongdianzi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zk.colortex.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vf.wgjwhj.cn

Ruby: arr.each { |item| puts item }
来源：http://tr.yuntaijiaju.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rr.huanxung.cn

[B06] 遍历字典 / 对象
来源：http://vw.shtwfgs.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ra.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cl.nszjky.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dt.bjjhwx.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fy.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ll.huixiangedu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xa.nicolike.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lh.shxzukj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kz.yuntaijiaju.cn

[B07] while 循环
来源：http://fb.gzmigu.cn

Py:   while i < 10: i += 1
来源：http://hn.gzmigu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ei.panjiajie.cn

JS:   while (i < 10) { i++; }
来源：http://xn.521024.cn

TS:   while (i < 10) { i++; }
来源：http://dq.gzmigu.cn

Java: while (i < 10) { i++; }
来源：http://nn.asd995.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hp.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://tn.colortex.cn

C#:   while (i < 10) { i++; }
来源：http://ib.yuntaijiaju.cn

[B08] do-while（至少执行一次）
来源：http://ph.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://nv.jianghongdianzi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://se.yuexingan06.cn

JS:   do { i++; } while (i < 10);
来源：http://um.shtwfgs.cn

TS:   do { i++; } while (i < 10);
来源：http://bn.huixinmuqiang.cn

Java: do { i++; } while (i < 10);
来源：http://ph.huanxung.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bw.muxihuayi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pi.521024.cn

C#:   do { i++; } while (i < 10);
来源：http://kp.gzmigu.cn

[B09] break 与 continue
来源：http://zr.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://im.muxihuayi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://aq.huixiangedu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jc.shxzskj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qj.wgjwhj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oo.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pa.yuexingan06.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vl.panjiajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://il.hahajie.cn

[B10] 遍历同时拿索引
来源：http://zj.muxihuayi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yx.hahajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://id.asd995.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jf.chemitech.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ht.bookmarksfly.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://st.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ac.muxihuayi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iz.yuntaijiaju.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sp.szsharing.cn

[B11] 生成数字序列 / 区间
来源：http://bj.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://hd.521024.cn

PHP:  range(0, 10, 2);
来源：http://ea.shxzukj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wc.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qj.szxytkj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hh.bjjhwx.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ei.9csxet.cn

Ruby: (0...10).step(2).to_a
来源：http://gy.shxzskj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vf.asd995.cn

[B12] 跳出多层循环
来源：http://gi.chemitech.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xw.colortex.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vg.hahajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wb.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wx.9csxet.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wj.gzmigu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ot.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pu.lnxyls.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://br.huanxung.cn

[B13] 判断是否为数字
来源：http://ry.huixinmuqiang.cn

Py:   isinstance(x, (int, float))
来源：http://at.shxzukj.cn

PHP:  is_numeric($x)
来源：http://fb.jianghongdianzi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vq.asd995.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mf.jianghongdianzi.cn

Java: x instanceof Number
来源：http://bh.jctech888.com.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gg.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://zl.panjiajie.cn

C#:   x is int or double or decimal
来源：http://yg.hahajie.cn

[B14] 判断值是否在集合内
来源：http://wd.lnxyls.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://et.huixiangedu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bo.chemitech.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://tw.wgjwhj.cn

TS:   [1, 2, 3].includes(x)
来源：http://cf.muxihuayi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pu.szsharing.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gv.bookmarksfly.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vx.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://op.shtwfgs.cn

[B15] 布尔运算与取反
来源：http://wk.szxytkj.cn

Py:   a and b or not c
来源：http://bl.yuexingan06.cn

PHP:  $a && $b || !$c
来源：http://pk.szsharing.cn

JS:   a && b || !c
来源：http://nd.bjjhwx.cn

TS:   a && b || !c
来源：http://ce.shxzukj.cn

Java: a && b || !c
来源：http://dr.jctech888.com.cn

Go:   a && b || !c
来源：http://tx.wgjwhj.cn

Ruby: a && b || !c
来源：http://fj.bjjhwx.cn

C#:   a && b || !c
来源：http://mb.huixiangedu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nx.huanxung.cn

Py:   if not data: return
来源：http://nc.huixiangedu.cn

PHP:  if (!$data) { return; }
来源：http://bz.jctech888.com.cn

JS:   if (!data) return;
来源：http://ek.shtwfgs.cn

TS:   if (!data) return;
来源：http://sk.shtwfgs.cn

Java: if (data == null) return;
来源：http://vw.huixiangedu.cn

Go:   if data == nil { return }
来源：http://bk.shxzskj.cn

Ruby: return if data.nil?
来源：http://zu.szsharing.cn

C#:   if (data == null) return;
来源：http://dr.hahajie.cn

================================================================================
来源：http://xk.shtwfgs.cn

C. 函数与作用域
来源：http://na.shtwfgs.cn

================================================================================
来源：http://yb.haigaiapp.cn

[C01] 定义函数
来源：http://vn.yuexingan06.cn

Py:   def add(a, b): return a + b
来源：http://xp.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xv.bjjhwx.cn

JS:   function add(a, b) { return a + b; }
来源：http://sx.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lt.panjiajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mq.colortex.cn

Go:   func add(a, b int) int { return a + b }
来源：http://im.nicolike.cn

Ruby: def add(a, b); a + b; end
来源：http://vu.szsharing.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fj.jctech888.com.cn

[C02] 默认参数
来源：http://wv.nszjky.cn

Py:   def greet(name="World"): return name
来源：http://fb.chemitech.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cl.hahajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://mk.asd995.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vo.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://av.9csxet.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ew.9csxet.cn

Ruby: def greet(name = "World") = name
来源：http://fj.szxytkj.cn

C#:   string Greet(string name = "World") => name;
来源：http://cf.9csxet.cn

[C03] 可变参数
来源：http://wd.shxzskj.cn

Py:   def total(*args): return sum(args)
来源：http://rl.huanxung.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ac.jianghongdianzi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://li.huixinmuqiang.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fq.nicolike.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pp.jianghongdianzi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ht.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pr.huanxung.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://er.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://od.bookmarksfly.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ii.gzmigu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vc.shtwfgs.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uz.bookmarksfly.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bg.yuntaijiaju.cn

Java: // 无：用 Builder 模式或 record
来源：http://ij.asd995.cn

Go:   // 无：用配置结构体参数
来源：http://eh.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://hv.yuexingan06.cn

C#:   f(a: 1, b: 2)
来源：http://gh.nicolike.cn

[C05] 返回多个值
来源：http://tz.nicolike.cn


<!-- 参考信息 -->