代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qm.szxytkj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ak.huanxung.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ma.huanxung.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ow.nicolike.cn

[A18] 字符与 ASCII 码互转
来源：http://xo.hnjuh.cn

Py:   ord("A"); chr(65)
来源：http://eq.nszjky.cn

PHP:  ord("A"); chr(65)
来源：http://rf.wgjwhj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pd.haigaiapp.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lr.yuntaijiaju.cn

Java: (int) 'A'; (char) 65
来源：http://fq.huixinmuqiang.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pt.haigaiapp.cn

Ruby: "A".ord; 65.chr
来源：http://ii.shxzukj.cn

C#:   (int)'A'; (char)65
来源：http://up.panjiajie.cn

[A19] 交换两个变量
来源：http://pi.huanxung.cn

Py:   a, b = b, a
来源：http://yz.bookmarksfly.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://on.huixinmuqiang.cn

JS:   [a, b] = [b, a];
来源：http://rh.chemitech.net.cn

TS:   [a, b] = [b, a];
来源：http://tw.huanxung.cn

Java: int t = a; a = b; b = t;
来源：http://yh.yuntaijiaju.cn

Go:   a, b = b, a
来源：http://zc.hahajie.cn

Ruby: a, b = b, a
来源：http://gy.newstarts.cn

C#:   (a, b) = (b, a);
来源：http://ex.haigaiapp.cn

[A20] 读取标准输入
来源：http://gf.hahajie.cn

Py:   name = input("请输入：")
来源：http://fz.hahajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://cm.szsharing.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cf.jctech888.com.cn

TS:   // Node.js：readline 模块
来源：http://nf.muxihuayi.cn

Java: new Scanner(System.in).nextLine()
来源：http://lj.shtwfgs.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jf.9csxet.cn

Ruby: gets.chomp
来源：http://hp.huixiangedu.cn

C#:   Console.ReadLine();
来源：http://op.jctech888.com.cn

[A21] 保留指定小数位输出
来源：http://va.521024.cn

Py:   f"{3.14159:.2f}"
来源：http://bz.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ay.jctech888.com.cn

JS:   (3.14159).toFixed(2)
来源：http://cr.bjjhwx.cn

TS:   (3.14159).toFixed(2)
来源：http://ht.nszjky.cn

Java: String.format("%.2f", 3.14159)
来源：http://fb.muxihuayi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gi.szxytkj.cn

Ruby: format("%.2f", 3.14159)
来源：http://hi.huixiangedu.cn

C#:   3.14159.ToString("F2")
来源：http://dk.asd995.cn

[A22] 获取字符串长度
来源：http://tf.chemitech.net.cn

Py:   len(s)
来源：http://xj.jctech888.com.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://re.asd995.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sj.hahajie.cn

TS:   s.length
来源：http://mh.huanxung.cn

Java: s.length()
来源：http://km.jianghongdianzi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pa.hnjuh.cn

Ruby: s.length
来源：http://dr.wgjwhj.cn

C#:   s.Length
来源：http://sc.jianghongdianzi.cn

[A23] 大小写转换
来源：http://sw.bjjhwx.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://lz.haigaiapp.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ru.asd995.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gc.nszjky.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yz.shtwfgs.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sa.jianghongdianzi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fc.huanxung.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xc.shtwfgs.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://je.lnxyls.cn

[A24] 去除首尾空白
来源：http://dl.jianghongdianzi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sd.lnxyls.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ju.muxihuayi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gq.huixiangedu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dz.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://aq.muxihuayi.cn

Go:   strings.TrimSpace(s)
来源：http://fh.szsharing.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uo.nszjky.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lv.lnxyls.cn

[A25] 字符串比较
来源：http://ej.haigaiapp.cn

Py:   s1 == s2; s1 != s2
来源：http://hp.521024.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xd.colortex.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://oc.wgjwhj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fm.colortex.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sa.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qs.jianghongdianzi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rj.shtwfgs.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gu.haigaiapp.cn

[A26] 类型转换总览
来源：http://gz.jctech888.com.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cl.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rc.bookmarksfly.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fk.521024.cn

TS:   Number() String() Boolean() x as number
来源：http://jd.lnxyls.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kc.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yw.nicolike.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nq.haigaiapp.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ee.haigaiapp.cn

================================================================================
来源：http://qi.huixiangedu.cn

B. 流程控制
来源：http://ov.colortex.cn

================================================================================
来源：http://oe.hahajie.cn

[B01] 条件判断 if / else
来源：http://lx.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://uv.nicolike.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nd.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fn.newstarts.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fa.asd995.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qt.yuntaijiaju.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sq.szsharing.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ck.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ih.lnxyls.cn

[B02] 多分支 else if / elif
来源：http://je.haigaiapp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wc.colortex.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nq.shxzukj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mk.huixiangedu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xh.panjiajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ef.asd995.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gc.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://da.521024.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.chemitech.net.cn

[B03] switch / match / case
来源：http://eo.muxihuayi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cs.yuntaijiaju.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bc.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ky.jctech888.com.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://te.shtwfgs.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kt.nicolike.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zg.shxzukj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fl.bjjhwx.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zl.yuexingan06.cn

[B04] for 计数循环
来源：http://fh.lnxyls.cn

Py:   for i in range(10): print(i)
来源：http://hj.shxzskj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uk.shxzukj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lj.newstarts.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cd.szxytkj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ep.yuntaijiaju.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://of.colortex.cn

Ruby: 10.times { |i| puts i }
来源：http://hf.bookmarksfly.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sn.chemitech.net.cn

[B05] 遍历数组 / 列表
来源：http://lp.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://we.hnjuh.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hh.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tw.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://iq.huanxung.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fd.jianghongdianzi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tj.lnxyls.cn

Ruby: arr.each { |item| puts item }
来源：http://ly.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kg.haigaiapp.cn

[B06] 遍历字典 / 对象
来源：http://sg.bookmarksfly.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://if.haigaiapp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ed.bookmarksfly.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xg.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vy.huanxung.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tk.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://km.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ev.chemitech.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ui.colortex.cn

[B07] while 循环
来源：http://al.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://fm.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xy.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://bd.lnxyls.cn

TS:   while (i < 10) { i++; }
来源：http://tj.shxzukj.cn

Java: while (i < 10) { i++; }
来源：http://fv.hahajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://be.newstarts.cn

Ruby: while i < 10; i += 1; end
来源：http://md.panjiajie.cn

C#:   while (i < 10) { i++; }
来源：http://ao.9csxet.cn

[B08] do-while（至少执行一次）
来源：http://nj.muxihuayi.cn

Py:   # 无 do-while：用 while True + break
来源：http://qd.jctech888.com.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zj.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://mn.nicolike.cn

TS:   do { i++; } while (i < 10);
来源：http://xi.huixinmuqiang.cn

Java: do { i++; } while (i < 10);
来源：http://dv.nszjky.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pa.szxytkj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ag.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://wk.szsharing.cn

[B09] break 与 continue
来源：http://zz.bjjhwx.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zs.szsharing.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zn.colortex.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vp.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eh.jctech888.com.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wf.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gr.521024.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hq.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xf.colortex.cn

[B10] 遍历同时拿索引
来源：http://jc.nszjky.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rr.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wf.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yt.yuexingan06.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ug.nszjky.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fn.colortex.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kj.newstarts.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ba.shxzukj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vu.panjiajie.cn

[B11] 生成数字序列 / 区间
来源：http://yg.shxzukj.cn

Py:   list(range(0, 10, 2))
来源：http://bh.huixiangedu.cn

PHP:  range(0, 10, 2);
来源：http://lf.gzmigu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://un.huixiangedu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dw.huixiangedu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sc.yuexingan06.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ke.bookmarksfly.cn

Ruby: (0...10).step(2).to_a
来源：http://uc.asd995.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cy.muxihuayi.cn

[B12] 跳出多层循环
来源：http://gz.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tu.shxzukj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ww.nszjky.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gm.shtwfgs.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fp.bjjhwx.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ni.shtwfgs.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jm.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cj.yuexingan06.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vb.hnjuh.cn

[B13] 判断是否为数字
来源：http://su.hnjuh.cn

Py:   isinstance(x, (int, float))
来源：http://fw.newstarts.cn

PHP:  is_numeric($x)
来源：http://ph.newstarts.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://la.huixinmuqiang.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ub.huixiangedu.cn

Java: x instanceof Number
来源：http://hf.bjjhwx.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://md.hnjuh.cn

Ruby: x.is_a?(Numeric)
来源：http://lk.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://fz.shxzukj.cn

[B14] 判断值是否在集合内
来源：http://jy.yuexingan06.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ap.shtwfgs.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dd.huanxung.cn

JS:   [1, 2, 3].includes(x)
来源：http://hz.wgjwhj.cn

TS:   [1, 2, 3].includes(x)
来源：http://wh.chemitech.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vt.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qg.szxytkj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ot.shxzskj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://go.huixinmuqiang.cn

[B15] 布尔运算与取反
来源：http://fi.hahajie.cn

Py:   a and b or not c
来源：http://wp.nszjky.cn

PHP:  $a && $b || !$c
来源：http://ck.jctech888.com.cn

JS:   a && b || !c
来源：http://hq.jianghongdianzi.cn

TS:   a && b || !c
来源：http://aq.jctech888.com.cn

Java: a && b || !c
来源：http://wr.jianghongdianzi.cn

Go:   a && b || !c
来源：http://sk.muxihuayi.cn

Ruby: a && b || !c
来源：http://kx.jctech888.com.cn

C#:   a && b || !c
来源：http://ww.jianghongdianzi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hj.yuexingan06.cn

Py:   if not data: return
来源：http://ud.shtwfgs.cn

PHP:  if (!$data) { return; }
来源：http://jb.yuntaijiaju.cn

JS:   if (!data) return;
来源：http://gr.szsharing.cn

TS:   if (!data) return;
来源：http://tp.9csxet.cn

Java: if (data == null) return;
来源：http://pz.shtwfgs.cn

Go:   if data == nil { return }
来源：http://xw.huixinmuqiang.cn

Ruby: return if data.nil?
来源：http://ya.nicolike.cn

C#:   if (data == null) return;
来源：http://yg.shxzukj.cn

================================================================================
来源：http://yy.wgjwhj.cn

C. 函数与作用域
来源：http://fj.bookmarksfly.cn

================================================================================
来源：http://qo.521024.cn

[C01] 定义函数
来源：http://dx.shxzukj.cn

Py:   def add(a, b): return a + b
来源：http://er.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jv.shxzukj.cn

JS:   function add(a, b) { return a + b; }
来源：http://gv.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vi.hahajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ke.bjjhwx.cn

Go:   func add(a, b int) int { return a + b }
来源：http://be.haigaiapp.cn

Ruby: def add(a, b); a + b; end
来源：http://pc.panjiajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://la.wgjwhj.cn

[C02] 默认参数
来源：http://gu.jctech888.com.cn

Py:   def greet(name="World"): return name
来源：http://iv.asd995.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yy.wgjwhj.cn

JS:   function greet(name = "World") { return name; }
来源：http://jw.muxihuayi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://el.haigaiapp.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bq.newstarts.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lf.bjjhwx.cn

Ruby: def greet(name = "World") = name
来源：http://zx.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://jl.chemitech.net.cn

[C03] 可变参数
来源：http://uh.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://eh.newstarts.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yz.shxzskj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://je.bookmarksfly.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://da.shtwfgs.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ll.colortex.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pw.szsharing.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pl.shxzskj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cr.huanxung.cn

[C04] 命名参数 / 关键字参数
来源：http://ej.nicolike.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xe.hnjuh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://id.jianghongdianzi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ll.szsharing.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://aa.huanxung.cn

Java: // 无：用 Builder 模式或 record
来源：http://wp.yuexingan06.cn

Go:   // 无：用配置结构体参数
来源：http://xf.bookmarksfly.cn

Ruby: f(a: 1, b: 2)
来源：http://vg.asd995.cn

C#:   f(a: 1, b: 2)
来源：http://tg.chemitech.net.cn

[C05] 返回多个值
来源：http://wa.muxihuayi.cn

Py:   return a, b
来源：http://ok.lnxyls.cn

PHP:  return [$a, $b];
来源：http://zh.newstarts.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ri.newstarts.cn

TS:   return { a, b };
来源：http://nm.bjjhwx.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lw.szsharing.cn

Go:   return a, b
来源：http://bs.asd995.cn

Ruby: return a, b
来源：http://xz.lnxyls.cn

C#:   return (a, b);              // ValueTuple
来源：http://cy.9csxet.cn

[C06] 匿名函数 / lambda
来源：http://nz.haigaiapp.cn

Py:   square = lambda x: x * x
来源：http://eq.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tv.shxzskj.cn

JS:   const square = x => x * x;
来源：http://tw.wgjwhj.cn

TS:   const square = (x: number): number => x * x;
来源：http://ja.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jl.yuntaijiaju.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nl.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://qv.nicolike.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ie.newstarts.cn

[C07] 把函数作为参数传入
来源：http://gi.yuexingan06.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uz.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ai.colortex.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rj.muxihuayi.cn

TS:   arr.map(String)
来源：http://ab.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vj.szxytkj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kl.hnjuh.cn

Ruby: arr.map(&:upcase)
来源：http://gu.wgjwhj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://my.newstarts.cn

[C08] 闭包
来源：http://dp.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yf.asd995.cn


<!-- 参考信息 -->