代发 wailian999

[A14] 注释写法
来源：http://zx.szsharing.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://qx.shtwfgs.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ku.bjjhwx.cn

JS:   // 单行；/* 多行 */
来源：http://rl.hahajie.cn

TS:   // 单行；/* 多行 */
来源：http://yp.hahajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xs.chemitech.net.cn

Go:   // 单行；/* 多行 */
来源：http://ke.jctech888.com.cn

Ruby: # 单行；=begin 多行 =end
来源：http://tw.huanxung.cn

C#:   // 单行；/* 多行 */
来源：http://yn.szxytkj.cn

[A15] 空值判断与默认值
来源：http://rl.shtwfgs.cn

Py:   value = data or "默认值"
来源：http://ts.colortex.cn

PHP:  $value = $data ?? "默认值";
来源：http://wx.colortex.cn

JS:   const value = data ?? "默认值";
来源：http://st.nszjky.cn

TS:   const value = data ?? "默认值";
来源：http://pp.lnxyls.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ys.wgjwhj.cn

Go:   if data == "" { data = "默认值" }
来源：http://uf.chemitech.net.cn

Ruby: value = data || "默认值"
来源：http://id.huixiangedu.cn

C#:   var value = data ?? "默认值";
来源：http://gh.gzmigu.cn

[A16] 真假值判断规则
来源：http://kt.jianghongdianzi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nu.huixinmuqiang.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://az.nicolike.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mw.haigaiapp.cn

TS:   if (!x) {}
来源：http://bn.panjiajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gr.colortex.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gp.huixinmuqiang.cn

Ruby: unless x            # nil 与 false 为假
来源：http://qy.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ms.huixiangedu.cn

[A17] 位运算
来源：http://fm.asd995.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qx.chemitech.net.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pr.bjjhwx.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zx.asd995.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lt.huixinmuqiang.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://km.shxzskj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nv.lnxyls.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gn.muxihuayi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pm.chemitech.net.cn

[A18] 字符与 ASCII 码互转
来源：http://is.yuexingan06.cn

Py:   ord("A"); chr(65)
来源：http://yf.shxzukj.cn

PHP:  ord("A"); chr(65)
来源：http://wf.hahajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bu.hnjuh.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zp.szsharing.cn

Java: (int) 'A'; (char) 65
来源：http://wj.szxytkj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://su.muxihuayi.cn

Ruby: "A".ord; 65.chr
来源：http://zj.shxzukj.cn

C#:   (int)'A'; (char)65
来源：http://wv.bjjhwx.cn

[A19] 交换两个变量
来源：http://bc.colortex.cn

Py:   a, b = b, a
来源：http://pc.huixinmuqiang.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yc.colortex.cn

JS:   [a, b] = [b, a];
来源：http://aw.newstarts.cn

TS:   [a, b] = [b, a];
来源：http://kc.521024.cn

Java: int t = a; a = b; b = t;
来源：http://eg.panjiajie.cn

Go:   a, b = b, a
来源：http://rg.hahajie.cn

Ruby: a, b = b, a
来源：http://ab.shxzukj.cn

C#:   (a, b) = (b, a);
来源：http://ff.muxihuayi.cn

[A20] 读取标准输入
来源：http://cc.gzmigu.cn

Py:   name = input("请输入：")
来源：http://ed.bookmarksfly.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zo.shtwfgs.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yy.yuexingan06.cn

TS:   // Node.js：readline 模块
来源：http://gk.szxytkj.cn

Java: new Scanner(System.in).nextLine()
来源：http://sb.lnxyls.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mp.newstarts.cn

Ruby: gets.chomp
来源：http://gv.shxzskj.cn

C#:   Console.ReadLine();
来源：http://gv.jianghongdianzi.cn

[A21] 保留指定小数位输出
来源：http://ly.bjjhwx.cn

Py:   f"{3.14159:.2f}"
来源：http://gi.jctech888.com.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://om.hahajie.cn

JS:   (3.14159).toFixed(2)
来源：http://uv.hnjuh.cn

TS:   (3.14159).toFixed(2)
来源：http://cj.521024.cn

Java: String.format("%.2f", 3.14159)
来源：http://gb.szsharing.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ft.huixiangedu.cn

Ruby: format("%.2f", 3.14159)
来源：http://cb.haigaiapp.cn

C#:   3.14159.ToString("F2")
来源：http://rd.haigaiapp.cn

[A22] 获取字符串长度
来源：http://pk.szsharing.cn

Py:   len(s)
来源：http://zc.muxihuayi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://of.jctech888.com.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://am.wgjwhj.cn

TS:   s.length
来源：http://sj.newstarts.cn

Java: s.length()
来源：http://lc.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bi.gzmigu.cn

Ruby: s.length
来源：http://ek.yuntaijiaju.cn

C#:   s.Length
来源：http://aj.hahajie.cn

[A23] 大小写转换
来源：http://mn.muxihuayi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hf.521024.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ij.wgjwhj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zr.szxytkj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zp.hahajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://br.bjjhwx.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ch.521024.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xr.bjjhwx.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xx.asd995.cn

[A24] 去除首尾空白
来源：http://eh.huixiangedu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vi.nszjky.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wh.muxihuayi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ab.huixinmuqiang.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iy.szsharing.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ng.jctech888.com.cn

Go:   strings.TrimSpace(s)
来源：http://qb.huanxung.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mi.huanxung.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yz.bjjhwx.cn

[A25] 字符串比较
来源：http://gj.huixiangedu.cn

Py:   s1 == s2; s1 != s2
来源：http://oy.shxzukj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fk.panjiajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://su.newstarts.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ct.huanxung.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hg.bookmarksfly.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://np.asd995.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://sb.huixinmuqiang.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vd.panjiajie.cn

[A26] 类型转换总览
来源：http://eo.huixiangedu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vq.shxzukj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ep.jctech888.com.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jq.bookmarksfly.cn

TS:   Number() String() Boolean() x as number
来源：http://az.yuexingan06.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tg.hahajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dp.bjjhwx.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://uh.shxzukj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://it.nicolike.cn

================================================================================
来源：http://bt.hnjuh.cn

B. 流程控制
来源：http://pi.hahajie.cn

================================================================================
来源：http://gl.chemitech.net.cn

[B01] 条件判断 if / else
来源：http://ld.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fl.szsharing.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hu.huixinmuqiang.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ep.lnxyls.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qi.hnjuh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hp.wgjwhj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rq.lnxyls.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hg.gzmigu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ox.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://yy.wgjwhj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://te.nszjky.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bg.chemitech.net.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zn.521024.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hb.huixiangedu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yi.shtwfgs.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qw.shxzskj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qq.nszjky.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ec.bookmarksfly.cn

[B03] switch / match / case
来源：http://kf.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fy.nszjky.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uz.yuntaijiaju.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ak.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://go.bjjhwx.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://um.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://au.shtwfgs.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ef.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hx.huixinmuqiang.cn

[B04] for 计数循环
来源：http://nh.bjjhwx.cn

Py:   for i in range(10): print(i)
来源：http://tk.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ud.nicolike.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bx.shtwfgs.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ch.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vt.shtwfgs.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dc.521024.cn

Ruby: 10.times { |i| puts i }
来源：http://zi.jctech888.com.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://di.9csxet.cn

[B05] 遍历数组 / 列表
来源：http://rl.huanxung.cn

Py:   for item in arr: print(item)
来源：http://uj.bookmarksfly.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hv.lnxyls.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://do.huixiangedu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pm.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kn.huixiangedu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ok.hnjuh.cn

Ruby: arr.each { |item| puts item }
来源：http://vw.9csxet.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zt.shtwfgs.cn

[B06] 遍历字典 / 对象
来源：http://om.nszjky.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://em.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://et.nszjky.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fl.jianghongdianzi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hs.szsharing.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wh.huanxung.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nm.bjjhwx.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zl.nicolike.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ns.gzmigu.cn

[B07] while 循环
来源：http://mc.hnjuh.cn

Py:   while i < 10: i += 1
来源：http://fg.szsharing.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vi.newstarts.cn

JS:   while (i < 10) { i++; }
来源：http://jw.yuexingan06.cn

TS:   while (i < 10) { i++; }
来源：http://vn.colortex.cn

Java: while (i < 10) { i++; }
来源：http://bu.nszjky.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gc.yuntaijiaju.cn

Ruby: while i < 10; i += 1; end
来源：http://qk.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://wg.huixiangedu.cn

[B08] do-while（至少执行一次）
来源：http://zk.chemitech.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://jp.hnjuh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://iw.yuexingan06.cn

JS:   do { i++; } while (i < 10);
来源：http://bw.haigaiapp.cn

TS:   do { i++; } while (i < 10);
来源：http://rw.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://hv.haigaiapp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ha.shtwfgs.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xk.hnjuh.cn

C#:   do { i++; } while (i < 10);
来源：http://es.huixinmuqiang.cn

[B09] break 与 continue
来源：http://wg.shxzskj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://oq.hahajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ms.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lq.hahajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hw.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ah.hahajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ty.huanxung.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pc.lnxyls.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yw.jctech888.com.cn

[B10] 遍历同时拿索引
来源：http://rb.huixinmuqiang.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gz.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gj.shtwfgs.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gs.9csxet.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vt.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rc.nicolike.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qw.muxihuayi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kx.szxytkj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sm.huanxung.cn

[B11] 生成数字序列 / 区间
来源：http://pv.szxytkj.cn

Py:   list(range(0, 10, 2))
来源：http://wf.muxihuayi.cn

PHP:  range(0, 10, 2);
来源：http://fz.wgjwhj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vr.wgjwhj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fa.szsharing.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://db.shtwfgs.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qa.haigaiapp.cn

Ruby: (0...10).step(2).to_a
来源：http://kd.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://md.szxytkj.cn

[B12] 跳出多层循环
来源：http://hw.jctech888.com.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ny.shxzukj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sw.bookmarksfly.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yf.newstarts.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://po.shxzukj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ck.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wx.jctech888.com.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vg.gzmigu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ny.wgjwhj.cn

[B13] 判断是否为数字
来源：http://dh.szxytkj.cn

Py:   isinstance(x, (int, float))
来源：http://po.shtwfgs.cn

PHP:  is_numeric($x)
来源：http://fe.hnjuh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mi.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yi.chemitech.net.cn

Java: x instanceof Number
来源：http://xm.jianghongdianzi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ze.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://uq.huixiangedu.cn

C#:   x is int or double or decimal
来源：http://ad.szxytkj.cn

[B14] 判断值是否在集合内
来源：http://vh.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rj.muxihuayi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uq.wgjwhj.cn

JS:   [1, 2, 3].includes(x)
来源：http://fl.jianghongdianzi.cn

TS:   [1, 2, 3].includes(x)
来源：http://ja.szxytkj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rs.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nz.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pr.nicolike.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zn.yuexingan06.cn

[B15] 布尔运算与取反
来源：http://yi.hahajie.cn

Py:   a and b or not c
来源：http://pu.wgjwhj.cn

PHP:  $a && $b || !$c
来源：http://zd.asd995.cn

JS:   a && b || !c
来源：http://zx.nszjky.cn

TS:   a && b || !c
来源：http://by.szsharing.cn

Java: a && b || !c
来源：http://zx.shtwfgs.cn

Go:   a && b || !c
来源：http://lf.lnxyls.cn

Ruby: a && b || !c
来源：http://ds.bjjhwx.cn

C#:   a && b || !c
来源：http://zw.bjjhwx.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sg.gzmigu.cn

Py:   if not data: return
来源：http://ye.szsharing.cn

PHP:  if (!$data) { return; }
来源：http://la.9csxet.cn

JS:   if (!data) return;
来源：http://pr.newstarts.cn

TS:   if (!data) return;
来源：http://vr.hnjuh.cn

Java: if (data == null) return;
来源：http://hf.shxzskj.cn

Go:   if data == nil { return }
来源：http://ep.gzmigu.cn

Ruby: return if data.nil?
来源：http://ga.bjjhwx.cn

C#:   if (data == null) return;
来源：http://ji.muxihuayi.cn

================================================================================
来源：http://co.newstarts.cn

C. 函数与作用域
来源：http://hy.wgjwhj.cn

================================================================================
来源：http://ob.yuexingan06.cn

[C01] 定义函数
来源：http://hf.haigaiapp.cn

Py:   def add(a, b): return a + b
来源：http://xu.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hc.colortex.cn

JS:   function add(a, b) { return a + b; }
来源：http://aw.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sg.szsharing.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kn.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ta.szsharing.cn

Ruby: def add(a, b); a + b; end
来源：http://ly.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ql.huixinmuqiang.cn

[C02] 默认参数
来源：http://zz.asd995.cn

Py:   def greet(name="World"): return name
来源：http://fk.gzmigu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bj.newstarts.cn

JS:   function greet(name = "World") { return name; }
来源：http://gm.szsharing.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://kl.huixinmuqiang.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dh.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://em.hahajie.cn

Ruby: def greet(name = "World") = name
来源：http://kt.nicolike.cn

C#:   string Greet(string name = "World") => name;
来源：http://hv.colortex.cn

[C03] 可变参数
来源：http://zi.huixinmuqiang.cn

Py:   def total(*args): return sum(args)
来源：http://tj.chemitech.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jn.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ak.lnxyls.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://al.huanxung.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nk.jianghongdianzi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kz.jctech888.com.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hv.huanxung.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sv.jctech888.com.cn

[C04] 命名参数 / 关键字参数
来源：http://ju.nicolike.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ng.huixinmuqiang.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nv.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mc.wgjwhj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lg.chemitech.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://zl.hahajie.cn


<!-- 参考信息 -->