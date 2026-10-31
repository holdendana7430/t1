代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ro.jianghongdianzi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pk.chemitech.net.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xn.szsharing.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ax.muxihuayi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pd.newstarts.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qf.newstarts.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tc.nicolike.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bb.9csxet.cn

[A18] 字符与 ASCII 码互转
来源：http://te.colortex.cn

Py:   ord("A"); chr(65)
来源：http://ow.gzmigu.cn

PHP:  ord("A"); chr(65)
来源：http://so.shtwfgs.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pu.chemitech.net.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bz.newstarts.cn

Java: (int) 'A'; (char) 65
来源：http://rs.colortex.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gw.yuntaijiaju.cn

Ruby: "A".ord; 65.chr
来源：http://lz.lnxyls.cn

C#:   (int)'A'; (char)65
来源：http://uy.9csxet.cn

[A19] 交换两个变量
来源：http://pb.jctech888.com.cn

Py:   a, b = b, a
来源：http://jy.huixiangedu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://xu.wgjwhj.cn

JS:   [a, b] = [b, a];
来源：http://zi.nicolike.cn

TS:   [a, b] = [b, a];
来源：http://my.huanxung.cn

Java: int t = a; a = b; b = t;
来源：http://fa.chemitech.net.cn

Go:   a, b = b, a
来源：http://tg.newstarts.cn

Ruby: a, b = b, a
来源：http://qd.asd995.cn

C#:   (a, b) = (b, a);
来源：http://tn.szsharing.cn

[A20] 读取标准输入
来源：http://xk.szsharing.cn

Py:   name = input("请输入：")
来源：http://na.yuntaijiaju.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rz.haigaiapp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lu.yuntaijiaju.cn

TS:   // Node.js：readline 模块
来源：http://qu.newstarts.cn

Java: new Scanner(System.in).nextLine()
来源：http://mg.huixiangedu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://er.szxytkj.cn

Ruby: gets.chomp
来源：http://et.9csxet.cn

C#:   Console.ReadLine();
来源：http://nf.haigaiapp.cn

[A21] 保留指定小数位输出
来源：http://ge.asd995.cn

Py:   f"{3.14159:.2f}"
来源：http://tk.yuexingan06.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://aq.szsharing.cn

JS:   (3.14159).toFixed(2)
来源：http://qa.lnxyls.cn

TS:   (3.14159).toFixed(2)
来源：http://tl.asd995.cn

Java: String.format("%.2f", 3.14159)
来源：http://kz.huanxung.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mn.shxzukj.cn

Ruby: format("%.2f", 3.14159)
来源：http://lc.bjjhwx.cn

C#:   3.14159.ToString("F2")
来源：http://vt.gzmigu.cn

[A22] 获取字符串长度
来源：http://wg.szsharing.cn

Py:   len(s)
来源：http://cc.gzmigu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tl.chemitech.net.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ey.yuexingan06.cn

TS:   s.length
来源：http://cb.hnjuh.cn

Java: s.length()
来源：http://eu.huixinmuqiang.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ht.huixinmuqiang.cn

Ruby: s.length
来源：http://ud.521024.cn

C#:   s.Length
来源：http://jh.panjiajie.cn

[A23] 大小写转换
来源：http://vp.shxzukj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qd.shxzskj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://km.huanxung.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wo.colortex.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lk.nszjky.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gc.chemitech.net.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lv.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bq.9csxet.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jy.szsharing.cn

[A24] 去除首尾空白
来源：http://as.chemitech.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://oc.panjiajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nq.lnxyls.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://it.nicolike.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dd.huixinmuqiang.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wz.bookmarksfly.cn

Go:   strings.TrimSpace(s)
来源：http://sn.nszjky.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://so.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nf.bookmarksfly.cn

[A25] 字符串比较
来源：http://rb.szsharing.cn

Py:   s1 == s2; s1 != s2
来源：http://xe.huixinmuqiang.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fb.hahajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rc.huixiangedu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pq.shtwfgs.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wf.jctech888.com.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ll.szxytkj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bx.huixinmuqiang.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pk.newstarts.cn

[A26] 类型转换总览
来源：http://lx.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ng.asd995.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hf.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pb.hnjuh.cn

TS:   Number() String() Boolean() x as number
来源：http://dh.hahajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jw.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://er.huixinmuqiang.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://le.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rd.asd995.cn

================================================================================
来源：http://xv.muxihuayi.cn

B. 流程控制
来源：http://bv.colortex.cn

================================================================================
来源：http://gv.hahajie.cn

[B01] 条件判断 if / else
来源：http://mg.shxzskj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pe.colortex.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dj.chemitech.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xc.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vu.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hn.wgjwhj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://re.bjjhwx.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gp.huixinmuqiang.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ak.9csxet.cn

[B02] 多分支 else if / elif
来源：http://op.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lf.nicolike.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xl.shtwfgs.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fw.nicolike.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wb.shxzskj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sb.gzmigu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://at.gzmigu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://iw.huanxung.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lu.nszjky.cn

[B03] switch / match / case
来源：http://zu.9csxet.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kg.chemitech.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oc.jctech888.com.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bz.szsharing.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dh.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://go.bookmarksfly.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xl.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dm.asd995.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hm.bjjhwx.cn

[B04] for 计数循环
来源：http://xe.9csxet.cn

Py:   for i in range(10): print(i)
来源：http://pn.colortex.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kx.shtwfgs.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cw.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qz.szxytkj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wi.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sn.wgjwhj.cn

Ruby: 10.times { |i| puts i }
来源：http://eb.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zj.huanxung.cn

[B05] 遍历数组 / 列表
来源：http://ow.jianghongdianzi.cn

Py:   for item in arr: print(item)
来源：http://cs.huixinmuqiang.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ch.szxytkj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ly.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gc.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cn.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xm.shtwfgs.cn

Ruby: arr.each { |item| puts item }
来源：http://ra.bookmarksfly.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jc.asd995.cn

[B06] 遍历字典 / 对象
来源：http://wz.gzmigu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://de.shtwfgs.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ru.shtwfgs.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oo.9csxet.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pz.lnxyls.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zz.yuntaijiaju.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wk.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mw.shtwfgs.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wr.521024.cn

[B07] while 循环
来源：http://pw.asd995.cn

Py:   while i < 10: i += 1
来源：http://ld.shxzukj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mw.hnjuh.cn

JS:   while (i < 10) { i++; }
来源：http://cc.jctech888.com.cn

TS:   while (i < 10) { i++; }
来源：http://zx.hahajie.cn

Java: while (i < 10) { i++; }
来源：http://ih.yuntaijiaju.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xo.lnxyls.cn

Ruby: while i < 10; i += 1; end
来源：http://uo.shtwfgs.cn

C#:   while (i < 10) { i++; }
来源：http://od.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://fp.muxihuayi.cn

Py:   # 无 do-while：用 while True + break
来源：http://uh.muxihuayi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xo.colortex.cn

JS:   do { i++; } while (i < 10);
来源：http://jy.panjiajie.cn

TS:   do { i++; } while (i < 10);
来源：http://kd.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://qx.panjiajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://la.panjiajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mj.lnxyls.cn

C#:   do { i++; } while (i < 10);
来源：http://tj.shtwfgs.cn

[B09] break 与 continue
来源：http://xh.yuexingan06.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ax.szxytkj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pd.asd995.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bc.huixiangedu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wu.jctech888.com.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gg.colortex.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xb.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zy.huixinmuqiang.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ti.huanxung.cn

[B10] 遍历同时拿索引
来源：http://no.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nd.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://il.jianghongdianzi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zu.shxzskj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bb.chemitech.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ni.shtwfgs.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jn.szsharing.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cf.shxzskj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ga.haigaiapp.cn

[B11] 生成数字序列 / 区间
来源：http://ch.nicolike.cn

Py:   list(range(0, 10, 2))
来源：http://dy.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://cx.521024.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ea.hahajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mi.panjiajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vx.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ju.hahajie.cn

Ruby: (0...10).step(2).to_a
来源：http://zy.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bn.shtwfgs.cn

[B12] 跳出多层循环
来源：http://ey.hahajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ha.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bc.muxihuayi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hv.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yf.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zp.huanxung.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yx.bookmarksfly.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tb.bookmarksfly.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bz.521024.cn

[B13] 判断是否为数字
来源：http://et.lnxyls.cn

Py:   isinstance(x, (int, float))
来源：http://id.yuexingan06.cn

PHP:  is_numeric($x)
来源：http://ue.jianghongdianzi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ds.shtwfgs.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fk.nicolike.cn

Java: x instanceof Number
来源：http://gm.panjiajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ej.nicolike.cn

Ruby: x.is_a?(Numeric)
来源：http://rl.muxihuayi.cn

C#:   x is int or double or decimal
来源：http://iq.521024.cn

[B14] 判断值是否在集合内
来源：http://uu.wgjwhj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wg.hnjuh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ru.yuexingan06.cn

JS:   [1, 2, 3].includes(x)
来源：http://ue.nicolike.cn

TS:   [1, 2, 3].includes(x)
来源：http://cl.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://uu.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fk.yuexingan06.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jg.newstarts.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://if.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://nu.yuexingan06.cn

Py:   a and b or not c
来源：http://dq.jianghongdianzi.cn

PHP:  $a && $b || !$c
来源：http://lw.lnxyls.cn

JS:   a && b || !c
来源：http://mo.shtwfgs.cn

TS:   a && b || !c
来源：http://zr.bookmarksfly.cn

Java: a && b || !c
来源：http://ce.huanxung.cn

Go:   a && b || !c
来源：http://fu.szxytkj.cn

Ruby: a && b || !c
来源：http://at.szxytkj.cn

C#:   a && b || !c
来源：http://ev.huixinmuqiang.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rj.shtwfgs.cn

Py:   if not data: return
来源：http://es.chemitech.net.cn

PHP:  if (!$data) { return; }
来源：http://dd.nszjky.cn

JS:   if (!data) return;
来源：http://yr.521024.cn

TS:   if (!data) return;
来源：http://ry.colortex.cn

Java: if (data == null) return;
来源：http://vc.shtwfgs.cn

Go:   if data == nil { return }
来源：http://ui.huixinmuqiang.cn

Ruby: return if data.nil?
来源：http://he.huixinmuqiang.cn

C#:   if (data == null) return;
来源：http://gk.yuexingan06.cn

================================================================================
来源：http://pz.wgjwhj.cn

C. 函数与作用域
来源：http://pf.lnxyls.cn

================================================================================
来源：http://ud.yuntaijiaju.cn

[C01] 定义函数
来源：http://sb.nszjky.cn

Py:   def add(a, b): return a + b
来源：http://nc.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rn.lnxyls.cn

JS:   function add(a, b) { return a + b; }
来源：http://op.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://np.huixiangedu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jg.hnjuh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wc.panjiajie.cn

Ruby: def add(a, b); a + b; end
来源：http://zt.hnjuh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sz.yuexingan06.cn

[C02] 默认参数
来源：http://kt.hnjuh.cn

Py:   def greet(name="World"): return name
来源：http://bi.nszjky.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xa.muxihuayi.cn

JS:   function greet(name = "World") { return name; }
来源：http://th.bookmarksfly.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://uu.bookmarksfly.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ta.szxytkj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fa.newstarts.cn

Ruby: def greet(name = "World") = name
来源：http://ki.wgjwhj.cn

C#:   string Greet(string name = "World") => name;
来源：http://yp.lnxyls.cn

[C03] 可变参数
来源：http://fh.yuexingan06.cn

Py:   def total(*args): return sum(args)
来源：http://jq.shtwfgs.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nh.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pt.bjjhwx.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hg.bjjhwx.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sb.bjjhwx.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zu.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ud.shtwfgs.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vh.panjiajie.cn

[C04] 命名参数 / 关键字参数
来源：http://iw.huanxung.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cx.yuntaijiaju.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kl.wgjwhj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vg.yuexingan06.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rz.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://ip.hnjuh.cn

Go:   // 无：用配置结构体参数
来源：http://ab.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://kx.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://lr.521024.cn

[C05] 返回多个值
来源：http://hh.jianghongdianzi.cn

Py:   return a, b
来源：http://sx.9csxet.cn

PHP:  return [$a, $b];
来源：http://yi.huanxung.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vb.bjjhwx.cn

TS:   return { a, b };
来源：http://ie.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://un.chemitech.net.cn

Go:   return a, b
来源：http://ht.huixiangedu.cn

Ruby: return a, b
来源：http://zs.haigaiapp.cn

C#:   return (a, b);              // ValueTuple
来源：http://jo.bookmarksfly.cn

[C06] 匿名函数 / lambda
来源：http://lh.szxytkj.cn

Py:   square = lambda x: x * x
来源：http://gp.wgjwhj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://dm.nszjky.cn

JS:   const square = x => x * x;
来源：http://op.szxytkj.cn

TS:   const square = (x: number): number => x * x;
来源：http://ee.shxzskj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vr.bjjhwx.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ca.bookmarksfly.cn

Ruby: square = ->(x) { x * x }
来源：http://ph.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://te.colortex.cn

[C07] 把函数作为参数传入
来源：http://qd.bjjhwx.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qu.huixiangedu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://sl.gzmigu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://to.hnjuh.cn

TS:   arr.map(String)
来源：http://sa.shxzskj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://je.lnxyls.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://oh.shxzukj.cn


<!-- 参考信息 -->