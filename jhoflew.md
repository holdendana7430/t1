代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ab.9csxet.cn

Ruby: unless x            # nil 与 false 为假
来源：http://yg.lnxyls.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kq.yuntaijiaju.cn

[A17] 位运算
来源：http://uu.newstarts.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ki.huanxung.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ke.colortex.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sq.muxihuayi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://du.huixiangedu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://en.521024.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://oi.chemitech.net.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xt.bjjhwx.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yi.chemitech.net.cn

[A18] 字符与 ASCII 码互转
来源：http://ms.huixinmuqiang.cn

Py:   ord("A"); chr(65)
来源：http://mp.newstarts.cn

PHP:  ord("A"); chr(65)
来源：http://eo.hnjuh.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uq.hnjuh.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qp.jianghongdianzi.cn

Java: (int) 'A'; (char) 65
来源：http://on.panjiajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://oq.nszjky.cn

Ruby: "A".ord; 65.chr
来源：http://cm.521024.cn

C#:   (int)'A'; (char)65
来源：http://eo.nszjky.cn

[A19] 交换两个变量
来源：http://sv.jctech888.com.cn

Py:   a, b = b, a
来源：http://qz.nicolike.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tt.szsharing.cn

JS:   [a, b] = [b, a];
来源：http://wk.9csxet.cn

TS:   [a, b] = [b, a];
来源：http://ep.gzmigu.cn

Java: int t = a; a = b; b = t;
来源：http://me.9csxet.cn

Go:   a, b = b, a
来源：http://ln.9csxet.cn

Ruby: a, b = b, a
来源：http://pz.chemitech.net.cn

C#:   (a, b) = (b, a);
来源：http://hb.muxihuayi.cn

[A20] 读取标准输入
来源：http://mq.bookmarksfly.cn

Py:   name = input("请输入：")
来源：http://tz.hnjuh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qm.chemitech.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xe.bookmarksfly.cn

TS:   // Node.js：readline 模块
来源：http://mu.shxzukj.cn

Java: new Scanner(System.in).nextLine()
来源：http://co.nicolike.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ow.bookmarksfly.cn

Ruby: gets.chomp
来源：http://hk.huixinmuqiang.cn

C#:   Console.ReadLine();
来源：http://fb.shxzskj.cn

[A21] 保留指定小数位输出
来源：http://qn.huixinmuqiang.cn

Py:   f"{3.14159:.2f}"
来源：http://hr.huixiangedu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lm.shtwfgs.cn

JS:   (3.14159).toFixed(2)
来源：http://mi.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://ws.gzmigu.cn

Java: String.format("%.2f", 3.14159)
来源：http://dk.nicolike.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ay.hahajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://mh.jianghongdianzi.cn

C#:   3.14159.ToString("F2")
来源：http://zi.chemitech.net.cn

[A22] 获取字符串长度
来源：http://ud.newstarts.cn

Py:   len(s)
来源：http://df.lnxyls.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lf.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gu.huixinmuqiang.cn

TS:   s.length
来源：http://cc.hnjuh.cn

Java: s.length()
来源：http://kp.lnxyls.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ne.bjjhwx.cn

Ruby: s.length
来源：http://of.panjiajie.cn

C#:   s.Length
来源：http://wc.shtwfgs.cn

[A23] 大小写转换
来源：http://th.huanxung.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ia.nicolike.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pg.shxzskj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rn.shtwfgs.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fn.nszjky.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wa.haigaiapp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gv.wgjwhj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cx.521024.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://uv.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://ph.huixiangedu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ia.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cf.9csxet.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sa.521024.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ra.colortex.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://np.newstarts.cn

Go:   strings.TrimSpace(s)
来源：http://yv.bjjhwx.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pt.huixinmuqiang.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sh.asd995.cn

[A25] 字符串比较
来源：http://mb.wgjwhj.cn

Py:   s1 == s2; s1 != s2
来源：http://cy.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bj.jctech888.com.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vd.muxihuayi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xt.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cp.szxytkj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qp.gzmigu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://sj.nicolike.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yn.szsharing.cn

[A26] 类型转换总览
来源：http://mf.huanxung.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ct.bookmarksfly.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://by.szsharing.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qb.chemitech.net.cn

TS:   Number() String() Boolean() x as number
来源：http://fm.jianghongdianzi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wg.nicolike.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pw.wgjwhj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zd.gzmigu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gb.shxzskj.cn

================================================================================
来源：http://od.haigaiapp.cn

B. 流程控制
来源：http://fd.asd995.cn

================================================================================
来源：http://sn.muxihuayi.cn

[B01] 条件判断 if / else
来源：http://nv.shxzskj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lb.hahajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mq.shxzukj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ey.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://go.yuexingan06.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://se.lnxyls.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bk.wgjwhj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kj.gzmigu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ba.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://hu.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gl.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://od.nszjky.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hd.lnxyls.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xt.9csxet.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ee.jianghongdianzi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gy.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ly.nszjky.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yd.bookmarksfly.cn

[B03] switch / match / case
来源：http://wh.hnjuh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qd.wgjwhj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dl.9csxet.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qf.yuexingan06.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pd.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kx.bookmarksfly.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gv.bjjhwx.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pu.yuntaijiaju.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zq.shxzskj.cn

[B04] for 计数循环
来源：http://bi.hahajie.cn

Py:   for i in range(10): print(i)
来源：http://kd.jianghongdianzi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zx.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zf.szxytkj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uy.521024.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fb.lnxyls.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://aa.9csxet.cn

Ruby: 10.times { |i| puts i }
来源：http://vo.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cz.yuntaijiaju.cn

[B05] 遍历数组 / 列表
来源：http://qt.huixiangedu.cn

Py:   for item in arr: print(item)
来源：http://bb.yuexingan06.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://en.bookmarksfly.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dc.jctech888.com.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ko.hnjuh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://eu.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sc.panjiajie.cn

Ruby: arr.each { |item| puts item }
来源：http://ds.chemitech.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sp.nicolike.cn

[B06] 遍历字典 / 对象
来源：http://jb.lnxyls.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bf.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xa.jctech888.com.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ec.shtwfgs.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cz.wgjwhj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lo.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vf.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wb.yuntaijiaju.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yf.asd995.cn

[B07] while 循环
来源：http://ln.huixiangedu.cn

Py:   while i < 10: i += 1
来源：http://mt.bjjhwx.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jp.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://hz.gzmigu.cn

TS:   while (i < 10) { i++; }
来源：http://ij.yuntaijiaju.cn

Java: while (i < 10) { i++; }
来源：http://lf.hahajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://re.bjjhwx.cn

Ruby: while i < 10; i += 1; end
来源：http://mb.bookmarksfly.cn

C#:   while (i < 10) { i++; }
来源：http://is.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://ax.hahajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://vj.szxytkj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://go.huanxung.cn

JS:   do { i++; } while (i < 10);
来源：http://tq.huixiangedu.cn

TS:   do { i++; } while (i < 10);
来源：http://gh.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://mj.szsharing.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dd.bookmarksfly.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xh.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://ib.yuntaijiaju.cn

[B09] break 与 continue
来源：http://go.yuexingan06.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wf.yuexingan06.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qp.colortex.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yu.asd995.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ss.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hg.asd995.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pc.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uu.huixinmuqiang.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://st.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://iq.yuntaijiaju.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gj.yuexingan06.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ak.jctech888.com.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://th.nicolike.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cu.521024.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dd.newstarts.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://td.szsharing.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ub.panjiajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lu.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://jg.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://cz.hnjuh.cn

PHP:  range(0, 10, 2);
来源：http://uh.huixinmuqiang.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jw.szxytkj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ru.muxihuayi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://he.shxzskj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://af.gzmigu.cn

Ruby: (0...10).step(2).to_a
来源：http://jj.lnxyls.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yf.nicolike.cn

[B12] 跳出多层循环
来源：http://ma.lnxyls.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sr.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ms.chemitech.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pq.gzmigu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ne.bjjhwx.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xd.lnxyls.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ud.yuexingan06.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ba.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ah.nicolike.cn

[B13] 判断是否为数字
来源：http://ks.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://lp.newstarts.cn

PHP:  is_numeric($x)
来源：http://mi.gzmigu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vd.bjjhwx.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yb.shxzskj.cn

Java: x instanceof Number
来源：http://tv.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pn.szsharing.cn

Ruby: x.is_a?(Numeric)
来源：http://qq.hahajie.cn

C#:   x is int or double or decimal
来源：http://vp.521024.cn

[B14] 判断值是否在集合内
来源：http://hb.huanxung.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hw.jianghongdianzi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kv.shxzukj.cn

JS:   [1, 2, 3].includes(x)
来源：http://xr.szxytkj.cn

TS:   [1, 2, 3].includes(x)
来源：http://ls.shtwfgs.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ri.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ds.wgjwhj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://am.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yq.lnxyls.cn

[B15] 布尔运算与取反
来源：http://aj.9csxet.cn

Py:   a and b or not c
来源：http://pi.szxytkj.cn

PHP:  $a && $b || !$c
来源：http://rj.haigaiapp.cn

JS:   a && b || !c
来源：http://mn.newstarts.cn

TS:   a && b || !c
来源：http://vl.newstarts.cn

Java: a && b || !c
来源：http://zx.nicolike.cn

Go:   a && b || !c
来源：http://zs.szsharing.cn

Ruby: a && b || !c
来源：http://od.shxzukj.cn

C#:   a && b || !c
来源：http://pr.yuexingan06.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ie.asd995.cn

Py:   if not data: return
来源：http://hp.bookmarksfly.cn

PHP:  if (!$data) { return; }
来源：http://gg.asd995.cn

JS:   if (!data) return;
来源：http://av.nszjky.cn

TS:   if (!data) return;
来源：http://gb.huanxung.cn

Java: if (data == null) return;
来源：http://js.huixiangedu.cn

Go:   if data == nil { return }
来源：http://ks.muxihuayi.cn

Ruby: return if data.nil?
来源：http://kj.hnjuh.cn

C#:   if (data == null) return;
来源：http://af.nicolike.cn

================================================================================
来源：http://eu.panjiajie.cn

C. 函数与作用域
来源：http://un.521024.cn

================================================================================
来源：http://mz.nicolike.cn

[C01] 定义函数
来源：http://zh.9csxet.cn

Py:   def add(a, b): return a + b
来源：http://fh.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ov.hnjuh.cn

JS:   function add(a, b) { return a + b; }
来源：http://ag.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gx.szxytkj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bv.hahajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ij.szsharing.cn

Ruby: def add(a, b); a + b; end
来源：http://nt.hnjuh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tg.wgjwhj.cn

[C02] 默认参数
来源：http://rb.jctech888.com.cn

Py:   def greet(name="World"): return name
来源：http://eu.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qe.yuexingan06.cn

JS:   function greet(name = "World") { return name; }
来源：http://dr.yuexingan06.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pu.shxzskj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rm.lnxyls.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nf.newstarts.cn

Ruby: def greet(name = "World") = name
来源：http://yn.colortex.cn

C#:   string Greet(string name = "World") => name;
来源：http://yi.asd995.cn

[C03] 可变参数
来源：http://wg.shxzukj.cn

Py:   def total(*args): return sum(args)
来源：http://yg.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jy.521024.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nq.521024.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fx.bjjhwx.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ml.nicolike.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://aw.szsharing.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ea.shxzukj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uu.yuntaijiaju.cn

[C04] 命名参数 / 关键字参数
来源：http://iw.asd995.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fx.chemitech.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hh.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xe.bjjhwx.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ii.jctech888.com.cn

Java: // 无：用 Builder 模式或 record
来源：http://vu.shxzskj.cn

Go:   // 无：用配置结构体参数
来源：http://yy.hnjuh.cn

Ruby: f(a: 1, b: 2)
来源：http://yi.wgjwhj.cn

C#:   f(a: 1, b: 2)
来源：http://cb.yuntaijiaju.cn

[C05] 返回多个值
来源：http://jp.yuexingan06.cn

Py:   return a, b
来源：http://gj.szsharing.cn

PHP:  return [$a, $b];
来源：http://ao.huixiangedu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ws.hahajie.cn

TS:   return { a, b };
来源：http://mt.muxihuayi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bx.muxihuayi.cn

Go:   return a, b
来源：http://dz.yuntaijiaju.cn

Ruby: return a, b
来源：http://ir.bookmarksfly.cn

C#:   return (a, b);              // ValueTuple
来源：http://pr.shxzukj.cn

[C06] 匿名函数 / lambda
来源：http://vm.nicolike.cn

Py:   square = lambda x: x * x
来源：http://qi.gzmigu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://va.colortex.cn

JS:   const square = x => x * x;
来源：http://ee.chemitech.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://da.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ss.panjiajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://cl.szxytkj.cn

Ruby: square = ->(x) { x * x }
来源：http://br.hnjuh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://eb.lnxyls.cn

[C07] 把函数作为参数传入
来源：http://qi.wgjwhj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wq.bjjhwx.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ct.huanxung.cn


<!-- 参考信息 -->