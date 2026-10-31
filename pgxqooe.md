代发 wailian999

[A14] 注释写法
来源：http://ge.huixinmuqiang.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://uu.wgjwhj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://nx.szxytkj.cn

JS:   // 单行；/* 多行 */
来源：http://az.9csxet.cn

TS:   // 单行；/* 多行 */
来源：http://na.hahajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cw.huixinmuqiang.cn

Go:   // 单行；/* 多行 */
来源：http://rt.muxihuayi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://en.newstarts.cn

C#:   // 单行；/* 多行 */
来源：http://nx.9csxet.cn

[A15] 空值判断与默认值
来源：http://tb.nszjky.cn

Py:   value = data or "默认值"
来源：http://ap.9csxet.cn

PHP:  $value = $data ?? "默认值";
来源：http://bd.huanxung.cn

JS:   const value = data ?? "默认值";
来源：http://jx.lnxyls.cn

TS:   const value = data ?? "默认值";
来源：http://zr.huixinmuqiang.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cl.jctech888.com.cn

Go:   if data == "" { data = "默认值" }
来源：http://cx.bookmarksfly.cn

Ruby: value = data || "默认值"
来源：http://so.521024.cn

C#:   var value = data ?? "默认值";
来源：http://dc.panjiajie.cn

[A16] 真假值判断规则
来源：http://qh.muxihuayi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ni.newstarts.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cx.newstarts.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ph.nicolike.cn

TS:   if (!x) {}
来源：http://lu.lnxyls.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jo.colortex.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://eo.newstarts.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xb.nicolike.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://or.huixinmuqiang.cn

[A17] 位运算
来源：http://qw.shxzukj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hq.nszjky.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mp.haigaiapp.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gc.bookmarksfly.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://om.yuntaijiaju.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hr.wgjwhj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://eq.newstarts.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uu.chemitech.net.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ij.huixiangedu.cn

[A18] 字符与 ASCII 码互转
来源：http://sm.colortex.cn

Py:   ord("A"); chr(65)
来源：http://gj.521024.cn

PHP:  ord("A"); chr(65)
来源：http://mk.nicolike.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xo.hahajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hi.hahajie.cn

Java: (int) 'A'; (char) 65
来源：http://ad.yuntaijiaju.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wi.asd995.cn

Ruby: "A".ord; 65.chr
来源：http://tn.jianghongdianzi.cn

C#:   (int)'A'; (char)65
来源：http://gh.huanxung.cn

[A19] 交换两个变量
来源：http://xm.bjjhwx.cn

Py:   a, b = b, a
来源：http://av.bookmarksfly.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vs.szxytkj.cn

JS:   [a, b] = [b, a];
来源：http://rr.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://yg.9csxet.cn

Java: int t = a; a = b; b = t;
来源：http://wx.panjiajie.cn

Go:   a, b = b, a
来源：http://cw.bookmarksfly.cn

Ruby: a, b = b, a
来源：http://nl.muxihuayi.cn

C#:   (a, b) = (b, a);
来源：http://qg.yuexingan06.cn

[A20] 读取标准输入
来源：http://rl.bookmarksfly.cn

Py:   name = input("请输入：")
来源：http://nh.hnjuh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ab.hnjuh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sg.newstarts.cn

TS:   // Node.js：readline 模块
来源：http://zt.bookmarksfly.cn

Java: new Scanner(System.in).nextLine()
来源：http://sy.yuntaijiaju.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rv.yuexingan06.cn

Ruby: gets.chomp
来源：http://zu.colortex.cn

C#:   Console.ReadLine();
来源：http://qh.panjiajie.cn

[A21] 保留指定小数位输出
来源：http://kh.gzmigu.cn

Py:   f"{3.14159:.2f}"
来源：http://an.nszjky.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ds.521024.cn

JS:   (3.14159).toFixed(2)
来源：http://lz.shxzukj.cn

TS:   (3.14159).toFixed(2)
来源：http://qb.haigaiapp.cn

Java: String.format("%.2f", 3.14159)
来源：http://ab.gzmigu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fx.huixinmuqiang.cn

Ruby: format("%.2f", 3.14159)
来源：http://jq.huixiangedu.cn

C#:   3.14159.ToString("F2")
来源：http://kk.huixiangedu.cn

[A22] 获取字符串长度
来源：http://tq.nicolike.cn

Py:   len(s)
来源：http://me.shtwfgs.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://us.huixinmuqiang.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gs.nszjky.cn

TS:   s.length
来源：http://oa.huixiangedu.cn

Java: s.length()
来源：http://hs.nszjky.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jo.shtwfgs.cn

Ruby: s.length
来源：http://rm.hnjuh.cn

C#:   s.Length
来源：http://hr.huixinmuqiang.cn

[A23] 大小写转换
来源：http://ma.bookmarksfly.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wz.hahajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lk.panjiajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ez.nicolike.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ow.newstarts.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ys.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ty.hnjuh.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qe.panjiajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://oy.jianghongdianzi.cn

[A24] 去除首尾空白
来源：http://to.chemitech.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rt.huixiangedu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mp.nicolike.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://we.panjiajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zw.muxihuayi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://do.huanxung.cn

Go:   strings.TrimSpace(s)
来源：http://ag.huixinmuqiang.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zb.haigaiapp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zx.shxzukj.cn

[A25] 字符串比较
来源：http://hy.nszjky.cn

Py:   s1 == s2; s1 != s2
来源：http://vi.bookmarksfly.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uv.shxzskj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://iv.bookmarksfly.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mv.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vo.shxzukj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ik.nszjky.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bd.colortex.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rs.9csxet.cn

[A26] 类型转换总览
来源：http://ru.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ur.nszjky.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vv.szxytkj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://oh.chemitech.net.cn

TS:   Number() String() Boolean() x as number
来源：http://xv.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yf.wgjwhj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nk.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kr.yuexingan06.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://do.shxzukj.cn

================================================================================
来源：http://qu.hahajie.cn

B. 流程控制
来源：http://er.haigaiapp.cn

================================================================================
来源：http://hs.lnxyls.cn

[B01] 条件判断 if / else
来源：http://mn.panjiajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ax.nicolike.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ij.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vb.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bi.colortex.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://oc.lnxyls.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kb.521024.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://of.521024.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uu.huanxung.cn

[B02] 多分支 else if / elif
来源：http://gh.huanxung.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rd.muxihuayi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yh.huixinmuqiang.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ae.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://um.nszjky.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pu.newstarts.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gl.bookmarksfly.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://op.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xv.huanxung.cn

[B03] switch / match / case
来源：http://ip.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yv.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sd.huixinmuqiang.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hs.asd995.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ee.muxihuayi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qy.lnxyls.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zk.bjjhwx.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kd.9csxet.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hs.bjjhwx.cn

[B04] for 计数循环
来源：http://tv.huixiangedu.cn

Py:   for i in range(10): print(i)
来源：http://hs.jianghongdianzi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fg.nicolike.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vh.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nw.yuexingan06.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://id.lnxyls.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gu.bjjhwx.cn

Ruby: 10.times { |i| puts i }
来源：http://ad.jctech888.com.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ou.521024.cn

[B05] 遍历数组 / 列表
来源：http://sn.bjjhwx.cn

Py:   for item in arr: print(item)
来源：http://xr.asd995.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wm.yuntaijiaju.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ah.asd995.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hb.shxzskj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ff.szxytkj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zl.newstarts.cn

Ruby: arr.each { |item| puts item }
来源：http://gg.9csxet.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bv.hahajie.cn

[B06] 遍历字典 / 对象
来源：http://oi.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://iz.gzmigu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uf.shxzskj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xu.haigaiapp.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ms.newstarts.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ny.shxzskj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qh.yuntaijiaju.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pz.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ok.hnjuh.cn

[B07] while 循环
来源：http://ap.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://zx.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hf.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://dc.asd995.cn

TS:   while (i < 10) { i++; }
来源：http://ks.newstarts.cn

Java: while (i < 10) { i++; }
来源：http://xp.huanxung.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gi.chemitech.net.cn

Ruby: while i < 10; i += 1; end
来源：http://ve.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://dg.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://xj.jctech888.com.cn

Py:   # 无 do-while：用 while True + break
来源：http://ul.huixinmuqiang.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hn.colortex.cn

JS:   do { i++; } while (i < 10);
来源：http://iq.shtwfgs.cn

TS:   do { i++; } while (i < 10);
来源：http://dz.huixiangedu.cn

Java: do { i++; } while (i < 10);
来源：http://xm.lnxyls.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cz.muxihuayi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qx.hnjuh.cn

C#:   do { i++; } while (i < 10);
来源：http://sf.colortex.cn

[B09] break 与 continue
来源：http://cr.asd995.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lz.szxytkj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zt.huixinmuqiang.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ze.nicolike.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ev.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wv.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mc.haigaiapp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nf.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bo.szxytkj.cn

[B10] 遍历同时拿索引
来源：http://ag.hahajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tr.nicolike.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gr.gzmigu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ld.hahajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yb.nszjky.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xa.colortex.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lv.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nw.lnxyls.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xz.szsharing.cn

[B11] 生成数字序列 / 区间
来源：http://fe.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://ox.huanxung.cn

PHP:  range(0, 10, 2);
来源：http://uq.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bw.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://br.bjjhwx.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ta.yuntaijiaju.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kl.yuexingan06.cn

Ruby: (0...10).step(2).to_a
来源：http://js.hahajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lx.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://gn.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ur.yuexingan06.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ki.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ju.haigaiapp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dr.hahajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ze.panjiajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ii.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fc.chemitech.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gi.bjjhwx.cn

[B13] 判断是否为数字
来源：http://qa.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://tn.wgjwhj.cn

PHP:  is_numeric($x)
来源：http://ey.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://do.jianghongdianzi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xe.chemitech.net.cn

Java: x instanceof Number
来源：http://eq.chemitech.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bl.huanxung.cn

Ruby: x.is_a?(Numeric)
来源：http://vt.muxihuayi.cn

C#:   x is int or double or decimal
来源：http://bf.jctech888.com.cn

[B14] 判断值是否在集合内
来源：http://gc.huanxung.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uk.gzmigu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gc.szxytkj.cn

JS:   [1, 2, 3].includes(x)
来源：http://sj.521024.cn

TS:   [1, 2, 3].includes(x)
来源：http://zv.wgjwhj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mc.bjjhwx.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yp.9csxet.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wd.newstarts.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qe.521024.cn

[B15] 布尔运算与取反
来源：http://ds.panjiajie.cn

Py:   a and b or not c
来源：http://rt.huixinmuqiang.cn

PHP:  $a && $b || !$c
来源：http://mn.yuexingan06.cn

JS:   a && b || !c
来源：http://hd.huanxung.cn

TS:   a && b || !c
来源：http://fk.gzmigu.cn

Java: a && b || !c
来源：http://ct.hahajie.cn

Go:   a && b || !c
来源：http://wn.gzmigu.cn

Ruby: a && b || !c
来源：http://ob.jianghongdianzi.cn

C#:   a && b || !c
来源：http://zb.newstarts.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kh.szsharing.cn

Py:   if not data: return
来源：http://uv.colortex.cn

PHP:  if (!$data) { return; }
来源：http://oi.lnxyls.cn

JS:   if (!data) return;
来源：http://fj.newstarts.cn

TS:   if (!data) return;
来源：http://dr.bookmarksfly.cn

Java: if (data == null) return;
来源：http://nl.huanxung.cn

Go:   if data == nil { return }
来源：http://lx.wgjwhj.cn

Ruby: return if data.nil?
来源：http://sg.shxzukj.cn

C#:   if (data == null) return;
来源：http://on.huanxung.cn

================================================================================
来源：http://zx.gzmigu.cn

C. 函数与作用域
来源：http://qx.9csxet.cn

================================================================================
来源：http://ux.shtwfgs.cn

[C01] 定义函数
来源：http://pg.jianghongdianzi.cn

Py:   def add(a, b): return a + b
来源：http://al.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nh.yuntaijiaju.cn

JS:   function add(a, b) { return a + b; }
来源：http://il.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cp.bookmarksfly.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://al.newstarts.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sw.jctech888.com.cn

Ruby: def add(a, b); a + b; end
来源：http://pm.huanxung.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uw.asd995.cn

[C02] 默认参数
来源：http://vz.wgjwhj.cn

Py:   def greet(name="World"): return name
来源：http://sx.shxzskj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ot.huanxung.cn

JS:   function greet(name = "World") { return name; }
来源：http://ba.asd995.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ul.huixinmuqiang.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ri.yuexingan06.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://da.chemitech.net.cn

Ruby: def greet(name = "World") = name
来源：http://qk.yuexingan06.cn

C#:   string Greet(string name = "World") => name;
来源：http://sw.shxzukj.cn

[C03] 可变参数
来源：http://kq.shxzskj.cn

Py:   def total(*args): return sum(args)
来源：http://bo.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zw.bjjhwx.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ei.jctech888.com.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wk.shxzukj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mu.nicolike.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dl.shtwfgs.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fw.huixiangedu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hi.colortex.cn

[C04] 命名参数 / 关键字参数
来源：http://um.nicolike.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ig.bookmarksfly.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://go.wgjwhj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wn.szxytkj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ci.nszjky.cn

Java: // 无：用 Builder 模式或 record
来源：http://df.bjjhwx.cn


<!-- 参考信息 -->