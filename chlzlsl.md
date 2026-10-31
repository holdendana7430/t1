代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://he.huanxung.cn

Py:   ord("A"); chr(65)
来源：http://se.wgjwhj.cn

PHP:  ord("A"); chr(65)
来源：http://xb.wgjwhj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wz.shtwfgs.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vh.hahajie.cn

Java: (int) 'A'; (char) 65
来源：http://xb.shtwfgs.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qe.shtwfgs.cn

Ruby: "A".ord; 65.chr
来源：http://ul.colortex.cn

C#:   (int)'A'; (char)65
来源：http://ol.yuntaijiaju.cn

[A19] 交换两个变量
来源：http://is.bookmarksfly.cn

Py:   a, b = b, a
来源：http://fn.shxzukj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://rd.yuexingan06.cn

JS:   [a, b] = [b, a];
来源：http://jp.asd995.cn

TS:   [a, b] = [b, a];
来源：http://ga.chemitech.net.cn

Java: int t = a; a = b; b = t;
来源：http://iu.9csxet.cn

Go:   a, b = b, a
来源：http://dr.huixiangedu.cn

Ruby: a, b = b, a
来源：http://vv.bjjhwx.cn

C#:   (a, b) = (b, a);
来源：http://qg.jianghongdianzi.cn

[A20] 读取标准输入
来源：http://jr.yuntaijiaju.cn

Py:   name = input("请输入：")
来源：http://ig.szsharing.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://sn.nicolike.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xe.nicolike.cn

TS:   // Node.js：readline 模块
来源：http://wz.newstarts.cn

Java: new Scanner(System.in).nextLine()
来源：http://is.jctech888.com.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ot.szsharing.cn

Ruby: gets.chomp
来源：http://um.yuexingan06.cn

C#:   Console.ReadLine();
来源：http://ls.9csxet.cn

[A21] 保留指定小数位输出
来源：http://pu.shxzskj.cn

Py:   f"{3.14159:.2f}"
来源：http://bt.yuntaijiaju.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ti.nicolike.cn

JS:   (3.14159).toFixed(2)
来源：http://qg.hnjuh.cn

TS:   (3.14159).toFixed(2)
来源：http://sr.shtwfgs.cn

Java: String.format("%.2f", 3.14159)
来源：http://ba.yuntaijiaju.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qy.asd995.cn

Ruby: format("%.2f", 3.14159)
来源：http://fc.panjiajie.cn

C#:   3.14159.ToString("F2")
来源：http://hr.haigaiapp.cn

[A22] 获取字符串长度
来源：http://pz.asd995.cn

Py:   len(s)
来源：http://cu.jctech888.com.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hj.nicolike.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lp.panjiajie.cn

TS:   s.length
来源：http://cl.szsharing.cn

Java: s.length()
来源：http://av.huixiangedu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bb.chemitech.net.cn

Ruby: s.length
来源：http://lx.hahajie.cn

C#:   s.Length
来源：http://ou.chemitech.net.cn

[A23] 大小写转换
来源：http://gg.chemitech.net.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rq.nicolike.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kk.muxihuayi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pe.nicolike.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pb.jctech888.com.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rs.asd995.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sr.hahajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://et.521024.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hu.muxihuayi.cn

[A24] 去除首尾空白
来源：http://jv.asd995.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gs.shtwfgs.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://uf.asd995.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gd.asd995.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://va.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sv.muxihuayi.cn

Go:   strings.TrimSpace(s)
来源：http://ez.shtwfgs.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dt.nszjky.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lp.wgjwhj.cn

[A25] 字符串比较
来源：http://uq.shtwfgs.cn

Py:   s1 == s2; s1 != s2
来源：http://bu.lnxyls.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ew.colortex.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://oq.gzmigu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sy.bookmarksfly.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jq.chemitech.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rk.huixiangedu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://dm.521024.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://im.szxytkj.cn

[A26] 类型转换总览
来源：http://hb.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pj.yuexingan06.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fo.nszjky.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rk.hnjuh.cn

TS:   Number() String() Boolean() x as number
来源：http://kx.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lw.szsharing.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vp.jianghongdianzi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ma.hahajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zx.wgjwhj.cn

================================================================================
来源：http://bk.panjiajie.cn

B. 流程控制
来源：http://vb.huanxung.cn

================================================================================
来源：http://bq.hnjuh.cn

[B01] 条件判断 if / else
来源：http://ii.nszjky.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dn.muxihuayi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zv.asd995.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://na.huixinmuqiang.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pd.yuntaijiaju.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://yw.jctech888.com.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cg.szxytkj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cx.muxihuayi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://na.huixinmuqiang.cn

[B02] 多分支 else if / elif
来源：http://bn.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://te.huixiangedu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://do.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hl.gzmigu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yf.jianghongdianzi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dh.nicolike.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zb.panjiajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ab.wgjwhj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pe.colortex.cn

[B03] switch / match / case
来源：http://ep.yuntaijiaju.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://br.nicolike.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cg.yuntaijiaju.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wk.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ag.bookmarksfly.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pf.yuexingan06.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pa.huanxung.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yf.muxihuayi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ep.wgjwhj.cn

[B04] for 计数循环
来源：http://tb.521024.cn

Py:   for i in range(10): print(i)
来源：http://yy.hnjuh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fg.bookmarksfly.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fx.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yx.521024.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rr.shxzukj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ux.huanxung.cn

Ruby: 10.times { |i| puts i }
来源：http://pp.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fu.521024.cn

[B05] 遍历数组 / 列表
来源：http://ep.huixiangedu.cn

Py:   for item in arr: print(item)
来源：http://yq.asd995.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mc.asd995.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yp.huixiangedu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://or.bookmarksfly.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cg.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rt.shtwfgs.cn

Ruby: arr.each { |item| puts item }
来源：http://ql.shxzukj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bd.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://ws.gzmigu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mo.huanxung.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mi.bookmarksfly.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xi.hahajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oj.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zg.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ky.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://or.muxihuayi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vr.panjiajie.cn

[B07] while 循环
来源：http://yn.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://jc.bjjhwx.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ic.9csxet.cn

JS:   while (i < 10) { i++; }
来源：http://zh.lnxyls.cn

TS:   while (i < 10) { i++; }
来源：http://rt.huixinmuqiang.cn

Java: while (i < 10) { i++; }
来源：http://xs.haigaiapp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wo.panjiajie.cn

Ruby: while i < 10; i += 1; end
来源：http://em.bookmarksfly.cn

C#:   while (i < 10) { i++; }
来源：http://qd.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://nw.9csxet.cn

Py:   # 无 do-while：用 while True + break
来源：http://os.bjjhwx.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rq.hahajie.cn

JS:   do { i++; } while (i < 10);
来源：http://lj.colortex.cn

TS:   do { i++; } while (i < 10);
来源：http://hl.yuntaijiaju.cn

Java: do { i++; } while (i < 10);
来源：http://uy.panjiajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qy.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zw.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://ur.gzmigu.cn

[B09] break 与 continue
来源：http://og.wgjwhj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tj.nszjky.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qv.9csxet.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cu.newstarts.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vr.shtwfgs.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ch.szsharing.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qa.nszjky.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bf.nicolike.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zv.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://eg.wgjwhj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jw.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ly.haigaiapp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jn.bookmarksfly.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://iu.wgjwhj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vv.asd995.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xu.nicolike.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://td.szsharing.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gh.huixinmuqiang.cn

[B11] 生成数字序列 / 区间
来源：http://wg.hnjuh.cn

Py:   list(range(0, 10, 2))
来源：http://oy.asd995.cn

PHP:  range(0, 10, 2);
来源：http://em.bjjhwx.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vp.huixiangedu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tz.shtwfgs.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ms.gzmigu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ap.lnxyls.cn

Ruby: (0...10).step(2).to_a
来源：http://lw.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xf.szxytkj.cn

[B12] 跳出多层循环
来源：http://wv.bjjhwx.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uu.bookmarksfly.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gj.chemitech.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vv.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yy.nszjky.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ol.huixiangedu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bp.huanxung.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fk.bjjhwx.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dq.gzmigu.cn

[B13] 判断是否为数字
来源：http://wk.shxzukj.cn

Py:   isinstance(x, (int, float))
来源：http://dr.521024.cn

PHP:  is_numeric($x)
来源：http://rp.yuntaijiaju.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aw.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nx.gzmigu.cn

Java: x instanceof Number
来源：http://da.jianghongdianzi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cw.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://ua.newstarts.cn

C#:   x is int or double or decimal
来源：http://qe.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://gp.bjjhwx.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ya.huanxung.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jt.521024.cn

JS:   [1, 2, 3].includes(x)
来源：http://bs.panjiajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://zj.nszjky.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://uq.hnjuh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cl.9csxet.cn

Ruby: [1, 2, 3].include?(x)
来源：http://um.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zy.nicolike.cn

[B15] 布尔运算与取反
来源：http://oi.szxytkj.cn

Py:   a and b or not c
来源：http://iu.wgjwhj.cn

PHP:  $a && $b || !$c
来源：http://fz.shtwfgs.cn

JS:   a && b || !c
来源：http://mh.521024.cn

TS:   a && b || !c
来源：http://mk.nicolike.cn

Java: a && b || !c
来源：http://vk.shxzskj.cn

Go:   a && b || !c
来源：http://lx.9csxet.cn

Ruby: a && b || !c
来源：http://vj.haigaiapp.cn

C#:   a && b || !c
来源：http://is.szxytkj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vj.shxzskj.cn

Py:   if not data: return
来源：http://bg.shxzukj.cn

PHP:  if (!$data) { return; }
来源：http://ta.yuntaijiaju.cn

JS:   if (!data) return;
来源：http://yt.huixiangedu.cn

TS:   if (!data) return;
来源：http://ss.gzmigu.cn

Java: if (data == null) return;
来源：http://tz.szxytkj.cn

Go:   if data == nil { return }
来源：http://ko.newstarts.cn

Ruby: return if data.nil?
来源：http://kb.shxzukj.cn

C#:   if (data == null) return;
来源：http://jd.gzmigu.cn

================================================================================
来源：http://xa.szsharing.cn

C. 函数与作用域
来源：http://bg.yuntaijiaju.cn

================================================================================
来源：http://pe.shxzskj.cn

[C01] 定义函数
来源：http://qp.chemitech.net.cn

Py:   def add(a, b): return a + b
来源：http://ce.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tk.521024.cn

JS:   function add(a, b) { return a + b; }
来源：http://ir.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xh.jctech888.com.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://et.521024.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zb.haigaiapp.cn

Ruby: def add(a, b); a + b; end
来源：http://jo.nszjky.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ev.szsharing.cn

[C02] 默认参数
来源：http://wx.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://uk.nicolike.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pv.shxzukj.cn

JS:   function greet(name = "World") { return name; }
来源：http://qy.yuexingan06.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://sn.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zj.szxytkj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ao.shxzskj.cn

Ruby: def greet(name = "World") = name
来源：http://do.yuexingan06.cn

C#:   string Greet(string name = "World") => name;
来源：http://fr.bookmarksfly.cn

[C03] 可变参数
来源：http://mh.hnjuh.cn

Py:   def total(*args): return sum(args)
来源：http://fh.szsharing.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tz.panjiajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sb.9csxet.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hi.newstarts.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vu.9csxet.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xw.hahajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vr.gzmigu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zl.lnxyls.cn

[C04] 命名参数 / 关键字参数
来源：http://wo.newstarts.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bf.521024.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yp.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://za.9csxet.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oz.nicolike.cn

Java: // 无：用 Builder 模式或 record
来源：http://fk.szsharing.cn

Go:   // 无：用配置结构体参数
来源：http://ge.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://ry.huixinmuqiang.cn

C#:   f(a: 1, b: 2)
来源：http://uz.yuntaijiaju.cn

[C05] 返回多个值
来源：http://ng.shtwfgs.cn

Py:   return a, b
来源：http://kq.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://dx.bjjhwx.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ct.yuntaijiaju.cn

TS:   return { a, b };
来源：http://tx.panjiajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ew.huixiangedu.cn

Go:   return a, b
来源：http://tk.huixinmuqiang.cn

Ruby: return a, b
来源：http://gj.muxihuayi.cn

C#:   return (a, b);              // ValueTuple
来源：http://lq.asd995.cn

[C06] 匿名函数 / lambda
来源：http://ma.huixiangedu.cn

Py:   square = lambda x: x * x
来源：http://so.yuexingan06.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ae.gzmigu.cn

JS:   const square = x => x * x;
来源：http://pd.nszjky.cn

TS:   const square = (x: number): number => x * x;
来源：http://oi.szsharing.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uo.panjiajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bh.wgjwhj.cn

Ruby: square = ->(x) { x * x }
来源：http://ow.jctech888.com.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ut.newstarts.cn

[C07] 把函数作为参数传入
来源：http://ku.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ql.haigaiapp.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lc.huixinmuqiang.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ov.szxytkj.cn

TS:   arr.map(String)
来源：http://oc.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mm.szsharing.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dl.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://ou.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cm.jctech888.com.cn

[C08] 闭包
来源：http://aj.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yn.9csxet.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rp.shtwfgs.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dj.lnxyls.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://iv.jianghongdianzi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nm.chemitech.net.cn


<!-- 参考信息 -->