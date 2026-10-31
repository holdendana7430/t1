代发 wailian999

Java: "第一行\n第二行"
来源：http://na.asd995.cn

Go:   "第一行\n第二行"
来源：http://sx.shtwfgs.cn

Ruby: "第一行\n第二行"
来源：http://av.jctech888.com.cn

C#:   "第一行\n第二行"
来源：http://sg.chemitech.net.cn

[A14] 注释写法
来源：http://pi.szsharing.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://qu.shtwfgs.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hy.bjjhwx.cn

JS:   // 单行；/* 多行 */
来源：http://nv.nszjky.cn

TS:   // 单行；/* 多行 */
来源：http://au.haigaiapp.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ud.haigaiapp.cn

Go:   // 单行；/* 多行 */
来源：http://iz.haigaiapp.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ki.yuexingan06.cn

C#:   // 单行；/* 多行 */
来源：http://vk.hnjuh.cn

[A15] 空值判断与默认值
来源：http://hc.bookmarksfly.cn

Py:   value = data or "默认值"
来源：http://kg.huixiangedu.cn

PHP:  $value = $data ?? "默认值";
来源：http://xj.shxzukj.cn

JS:   const value = data ?? "默认值";
来源：http://kl.shxzskj.cn

TS:   const value = data ?? "默认值";
来源：http://dh.huanxung.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dn.colortex.cn

Go:   if data == "" { data = "默认值" }
来源：http://kr.colortex.cn

Ruby: value = data || "默认值"
来源：http://qd.szxytkj.cn

C#:   var value = data ?? "默认值";
来源：http://lu.yuexingan06.cn

[A16] 真假值判断规则
来源：http://iq.chemitech.net.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ne.newstarts.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ik.hahajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dj.shtwfgs.cn

TS:   if (!x) {}
来源：http://un.huanxung.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kj.yuexingan06.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xy.muxihuayi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jk.huanxung.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nq.asd995.cn

[A17] 位运算
来源：http://fe.asd995.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ag.szsharing.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bb.szsharing.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ps.521024.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dr.huanxung.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rb.haigaiapp.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gq.huixiangedu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ua.hnjuh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://op.9csxet.cn

[A18] 字符与 ASCII 码互转
来源：http://lw.jianghongdianzi.cn

Py:   ord("A"); chr(65)
来源：http://so.jianghongdianzi.cn

PHP:  ord("A"); chr(65)
来源：http://fe.colortex.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iv.chemitech.net.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cq.nicolike.cn

Java: (int) 'A'; (char) 65
来源：http://hf.panjiajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ts.szxytkj.cn

Ruby: "A".ord; 65.chr
来源：http://bl.panjiajie.cn

C#:   (int)'A'; (char)65
来源：http://kb.yuntaijiaju.cn

[A19] 交换两个变量
来源：http://xw.nszjky.cn

Py:   a, b = b, a
来源：http://yf.bookmarksfly.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yg.huixinmuqiang.cn

JS:   [a, b] = [b, a];
来源：http://dy.wgjwhj.cn

TS:   [a, b] = [b, a];
来源：http://bm.gzmigu.cn

Java: int t = a; a = b; b = t;
来源：http://ii.9csxet.cn

Go:   a, b = b, a
来源：http://nv.panjiajie.cn

Ruby: a, b = b, a
来源：http://vq.asd995.cn

C#:   (a, b) = (b, a);
来源：http://ql.9csxet.cn

[A20] 读取标准输入
来源：http://nu.muxihuayi.cn

Py:   name = input("请输入：")
来源：http://ny.shxzukj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ay.nszjky.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ic.bjjhwx.cn

TS:   // Node.js：readline 模块
来源：http://st.lnxyls.cn

Java: new Scanner(System.in).nextLine()
来源：http://fx.shxzskj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gr.bjjhwx.cn

Ruby: gets.chomp
来源：http://dh.bookmarksfly.cn

C#:   Console.ReadLine();
来源：http://ry.haigaiapp.cn

[A21] 保留指定小数位输出
来源：http://fx.chemitech.net.cn

Py:   f"{3.14159:.2f}"
来源：http://mk.gzmigu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cv.nszjky.cn

JS:   (3.14159).toFixed(2)
来源：http://zv.gzmigu.cn

TS:   (3.14159).toFixed(2)
来源：http://mc.shxzskj.cn

Java: String.format("%.2f", 3.14159)
来源：http://uc.wgjwhj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zs.shtwfgs.cn

Ruby: format("%.2f", 3.14159)
来源：http://nt.chemitech.net.cn

C#:   3.14159.ToString("F2")
来源：http://zo.9csxet.cn

[A22] 获取字符串长度
来源：http://iq.szxytkj.cn

Py:   len(s)
来源：http://ac.newstarts.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xv.521024.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nl.gzmigu.cn

TS:   s.length
来源：http://xk.yuntaijiaju.cn

Java: s.length()
来源：http://eq.panjiajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ml.huixiangedu.cn

Ruby: s.length
来源：http://nh.hahajie.cn

C#:   s.Length
来源：http://ba.muxihuayi.cn

[A23] 大小写转换
来源：http://wr.szxytkj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kk.newstarts.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fu.jianghongdianzi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fp.huixiangedu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dm.lnxyls.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xx.huanxung.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://td.521024.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sf.asd995.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ds.jctech888.com.cn

[A24] 去除首尾空白
来源：http://gt.asd995.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jz.muxihuayi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://po.hnjuh.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://me.hahajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ho.jctech888.com.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mx.wgjwhj.cn

Go:   strings.TrimSpace(s)
来源：http://xd.newstarts.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mu.shtwfgs.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cw.lnxyls.cn

[A25] 字符串比较
来源：http://ib.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://yj.yuexingan06.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tn.szsharing.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ui.chemitech.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ul.hnjuh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dt.gzmigu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dy.panjiajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://uy.521024.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dy.huixiangedu.cn

[A26] 类型转换总览
来源：http://zd.nicolike.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ww.haigaiapp.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xr.hnjuh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mz.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://um.newstarts.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://by.bookmarksfly.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ed.521024.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lp.nszjky.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zu.huixinmuqiang.cn

================================================================================
来源：http://rv.wgjwhj.cn

B. 流程控制
来源：http://no.gzmigu.cn

================================================================================
来源：http://rd.bjjhwx.cn

[B01] 条件判断 if / else
来源：http://pr.huixiangedu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gl.nszjky.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nh.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pg.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vq.huanxung.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ks.huixiangedu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tz.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kz.huanxung.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bq.wgjwhj.cn

[B02] 多分支 else if / elif
来源：http://og.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hy.hahajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ki.yuntaijiaju.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fb.huixinmuqiang.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ix.nszjky.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zk.shtwfgs.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pq.panjiajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lk.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ox.huanxung.cn

[B03] switch / match / case
来源：http://ts.huanxung.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rx.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wk.wgjwhj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iw.newstarts.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ak.jctech888.com.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sq.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bk.huanxung.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zb.bookmarksfly.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sj.lnxyls.cn

[B04] for 计数循环
来源：http://fm.gzmigu.cn

Py:   for i in range(10): print(i)
来源：http://ki.hnjuh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://we.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pp.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dm.9csxet.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gu.colortex.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zj.9csxet.cn

Ruby: 10.times { |i| puts i }
来源：http://xk.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ez.bjjhwx.cn

[B05] 遍历数组 / 列表
来源：http://dj.lnxyls.cn

Py:   for item in arr: print(item)
来源：http://il.521024.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ls.nszjky.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rr.wgjwhj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sm.gzmigu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ko.szxytkj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bp.lnxyls.cn

Ruby: arr.each { |item| puts item }
来源：http://ki.newstarts.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yc.521024.cn

[B06] 遍历字典 / 对象
来源：http://kv.huanxung.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fc.szsharing.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://de.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ay.huixinmuqiang.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gw.bjjhwx.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ka.yuexingan06.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://re.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pv.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rb.hahajie.cn

[B07] while 循环
来源：http://hh.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://db.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hr.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://nf.haigaiapp.cn

TS:   while (i < 10) { i++; }
来源：http://vp.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://pd.szxytkj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hq.9csxet.cn

Ruby: while i < 10; i += 1; end
来源：http://zv.hnjuh.cn

C#:   while (i < 10) { i++; }
来源：http://wq.newstarts.cn

[B08] do-while（至少执行一次）
来源：http://xi.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://nh.huixinmuqiang.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://il.shxzukj.cn

JS:   do { i++; } while (i < 10);
来源：http://ay.huixinmuqiang.cn

TS:   do { i++; } while (i < 10);
来源：http://wr.hahajie.cn

Java: do { i++; } while (i < 10);
来源：http://wq.newstarts.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nj.jianghongdianzi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://un.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://vp.shtwfgs.cn

[B09] break 与 continue
来源：http://ps.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://eu.haigaiapp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yq.muxihuayi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fw.colortex.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pf.hnjuh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uu.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cc.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ph.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ai.nicolike.cn

[B10] 遍历同时拿索引
来源：http://zj.shxzukj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qz.huixiangedu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nh.bookmarksfly.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rs.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sj.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://la.szsharing.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://or.newstarts.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ve.szxytkj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://iq.chemitech.net.cn

[B11] 生成数字序列 / 区间
来源：http://gw.shxzukj.cn

Py:   list(range(0, 10, 2))
来源：http://ap.jctech888.com.cn

PHP:  range(0, 10, 2);
来源：http://gc.yuexingan06.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bq.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aj.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qo.shxzukj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xb.szsharing.cn

Ruby: (0...10).step(2).to_a
来源：http://ws.yuntaijiaju.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lj.lnxyls.cn

[B12] 跳出多层循环
来源：http://ck.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uq.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rh.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oe.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hf.shtwfgs.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pj.nicolike.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gb.hahajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hu.hahajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hv.yuntaijiaju.cn

[B13] 判断是否为数字
来源：http://ap.shxzskj.cn

Py:   isinstance(x, (int, float))
来源：http://ms.colortex.cn

PHP:  is_numeric($x)
来源：http://wr.szxytkj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tc.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oo.521024.cn

Java: x instanceof Number
来源：http://kr.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ox.colortex.cn

Ruby: x.is_a?(Numeric)
来源：http://gd.bookmarksfly.cn

C#:   x is int or double or decimal
来源：http://az.hnjuh.cn

[B14] 判断值是否在集合内
来源：http://qy.9csxet.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ut.jctech888.com.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lo.szxytkj.cn

JS:   [1, 2, 3].includes(x)
来源：http://vc.muxihuayi.cn

TS:   [1, 2, 3].includes(x)
来源：http://ac.nszjky.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mh.yuexingan06.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xd.jctech888.com.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zi.huixinmuqiang.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cv.lnxyls.cn

[B15] 布尔运算与取反
来源：http://jd.shxzskj.cn

Py:   a and b or not c
来源：http://ef.lnxyls.cn

PHP:  $a && $b || !$c
来源：http://rq.colortex.cn

JS:   a && b || !c
来源：http://lr.yuntaijiaju.cn

TS:   a && b || !c
来源：http://yt.nszjky.cn

Java: a && b || !c
来源：http://qe.hahajie.cn

Go:   a && b || !c
来源：http://ud.chemitech.net.cn

Ruby: a && b || !c
来源：http://ln.521024.cn

C#:   a && b || !c
来源：http://il.yuexingan06.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tq.jianghongdianzi.cn

Py:   if not data: return
来源：http://up.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://cc.muxihuayi.cn

JS:   if (!data) return;
来源：http://yk.chemitech.net.cn

TS:   if (!data) return;
来源：http://pv.yuexingan06.cn

Java: if (data == null) return;
来源：http://kc.gzmigu.cn

Go:   if data == nil { return }
来源：http://xe.9csxet.cn

Ruby: return if data.nil?
来源：http://wz.szsharing.cn

C#:   if (data == null) return;
来源：http://fp.chemitech.net.cn

================================================================================
来源：http://mx.nszjky.cn

C. 函数与作用域
来源：http://cg.jianghongdianzi.cn

================================================================================
来源：http://eh.9csxet.cn

[C01] 定义函数
来源：http://dx.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://dt.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://op.hahajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://xn.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lj.9csxet.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mt.bjjhwx.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ay.shxzskj.cn

Ruby: def add(a, b); a + b; end
来源：http://ec.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ij.hnjuh.cn

[C02] 默认参数
来源：http://od.shtwfgs.cn

Py:   def greet(name="World"): return name
来源：http://lc.521024.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dm.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://jm.szxytkj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wi.haigaiapp.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ph.asd995.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qp.shtwfgs.cn

Ruby: def greet(name = "World") = name
来源：http://ho.chemitech.net.cn

C#:   string Greet(string name = "World") => name;
来源：http://vf.jctech888.com.cn

[C03] 可变参数
来源：http://lg.newstarts.cn

Py:   def total(*args): return sum(args)
来源：http://gn.jctech888.com.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qx.shxzukj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bb.nszjky.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wr.shtwfgs.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ut.bookmarksfly.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zf.jianghongdianzi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kb.yuexingan06.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sp.gzmigu.cn

[C04] 命名参数 / 关键字参数
来源：http://wi.colortex.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gg.huanxung.cn


<!-- 参考信息 -->