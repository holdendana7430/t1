代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vh.nszjky.cn

Java: (int) 'A'; (char) 65
来源：http://xb.bjjhwx.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xz.chemitech.net.cn

Ruby: "A".ord; 65.chr
来源：http://zq.bookmarksfly.cn

C#:   (int)'A'; (char)65
来源：http://nd.huanxung.cn

[A19] 交换两个变量
来源：http://ln.colortex.cn

Py:   a, b = b, a
来源：http://cn.asd995.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ct.chemitech.net.cn

JS:   [a, b] = [b, a];
来源：http://ou.shxzskj.cn

TS:   [a, b] = [b, a];
来源：http://cs.hnjuh.cn

Java: int t = a; a = b; b = t;
来源：http://bb.nszjky.cn

Go:   a, b = b, a
来源：http://nf.huixiangedu.cn

Ruby: a, b = b, a
来源：http://ns.yuexingan06.cn

C#:   (a, b) = (b, a);
来源：http://pj.jianghongdianzi.cn

[A20] 读取标准输入
来源：http://pz.huanxung.cn

Py:   name = input("请输入：")
来源：http://tz.yuntaijiaju.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ns.jianghongdianzi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vp.szxytkj.cn

TS:   // Node.js：readline 模块
来源：http://vp.nszjky.cn

Java: new Scanner(System.in).nextLine()
来源：http://ek.yuntaijiaju.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sw.huixinmuqiang.cn

Ruby: gets.chomp
来源：http://ic.wgjwhj.cn

C#:   Console.ReadLine();
来源：http://pk.chemitech.net.cn

[A21] 保留指定小数位输出
来源：http://vz.huixiangedu.cn

Py:   f"{3.14159:.2f}"
来源：http://nh.szsharing.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rd.shxzskj.cn

JS:   (3.14159).toFixed(2)
来源：http://gf.huixinmuqiang.cn

TS:   (3.14159).toFixed(2)
来源：http://hv.shtwfgs.cn

Java: String.format("%.2f", 3.14159)
来源：http://ge.wgjwhj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ta.wgjwhj.cn

Ruby: format("%.2f", 3.14159)
来源：http://qe.gzmigu.cn

C#:   3.14159.ToString("F2")
来源：http://my.lnxyls.cn

[A22] 获取字符串长度
来源：http://fj.bookmarksfly.cn

Py:   len(s)
来源：http://dj.chemitech.net.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://oi.panjiajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mw.panjiajie.cn

TS:   s.length
来源：http://jj.jianghongdianzi.cn

Java: s.length()
来源：http://oy.colortex.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ro.shtwfgs.cn

Ruby: s.length
来源：http://en.muxihuayi.cn

C#:   s.Length
来源：http://yf.chemitech.net.cn

[A23] 大小写转换
来源：http://gc.szxytkj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://py.9csxet.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dd.huixiangedu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fm.shxzskj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hk.nszjky.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wr.asd995.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ys.hahajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jh.shtwfgs.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ob.jianghongdianzi.cn

[A24] 去除首尾空白
来源：http://bw.colortex.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qo.huanxung.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xy.muxihuayi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uc.hnjuh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dc.wgjwhj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vs.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://tn.szsharing.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://og.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://in.nszjky.cn

[A25] 字符串比较
来源：http://nn.521024.cn

Py:   s1 == s2; s1 != s2
来源：http://rv.9csxet.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ww.yuexingan06.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ap.asd995.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jz.shxzskj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://uj.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sd.haigaiapp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ja.bookmarksfly.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ij.szsharing.cn

[A26] 类型转换总览
来源：http://nn.gzmigu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xw.newstarts.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ei.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tj.yuntaijiaju.cn

TS:   Number() String() Boolean() x as number
来源：http://fb.huanxung.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dp.hnjuh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bg.hnjuh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hw.colortex.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ee.nszjky.cn

================================================================================
来源：http://eq.hahajie.cn

B. 流程控制
来源：http://gv.wgjwhj.cn

================================================================================
来源：http://aa.521024.cn

[B01] 条件判断 if / else
来源：http://ba.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ii.bjjhwx.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qd.shxzskj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zn.yuntaijiaju.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dv.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://br.yuntaijiaju.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ks.huixinmuqiang.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xm.chemitech.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cc.muxihuayi.cn

[B02] 多分支 else if / elif
来源：http://ma.szsharing.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vf.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://td.newstarts.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sp.bjjhwx.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eq.nszjky.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rn.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://aj.hahajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ou.shtwfgs.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zw.gzmigu.cn

[B03] switch / match / case
来源：http://ud.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mi.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://aa.shxzukj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eq.yuntaijiaju.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jb.haigaiapp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://co.shtwfgs.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xd.shtwfgs.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jr.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ux.newstarts.cn

[B04] for 计数循环
来源：http://wi.jctech888.com.cn

Py:   for i in range(10): print(i)
来源：http://ww.bookmarksfly.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yo.9csxet.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fj.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mq.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dq.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vh.haigaiapp.cn

Ruby: 10.times { |i| puts i }
来源：http://rq.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kq.panjiajie.cn

[B05] 遍历数组 / 列表
来源：http://ns.gzmigu.cn

Py:   for item in arr: print(item)
来源：http://gb.shxzukj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cn.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mz.newstarts.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vq.gzmigu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ia.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jz.hnjuh.cn

Ruby: arr.each { |item| puts item }
来源：http://iz.gzmigu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hs.yuexingan06.cn

[B06] 遍历字典 / 对象
来源：http://pw.szxytkj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nm.bjjhwx.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ty.shtwfgs.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ag.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cf.asd995.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://as.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ve.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bo.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ke.huanxung.cn

[B07] while 循环
来源：http://zd.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://zg.shxzukj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yh.wgjwhj.cn

JS:   while (i < 10) { i++; }
来源：http://dl.521024.cn

TS:   while (i < 10) { i++; }
来源：http://fi.jctech888.com.cn

Java: while (i < 10) { i++; }
来源：http://bm.yuntaijiaju.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wj.chemitech.net.cn

Ruby: while i < 10; i += 1; end
来源：http://ty.colortex.cn

C#:   while (i < 10) { i++; }
来源：http://gy.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://bn.nicolike.cn

Py:   # 无 do-while：用 while True + break
来源：http://kv.shtwfgs.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bx.shtwfgs.cn

JS:   do { i++; } while (i < 10);
来源：http://wp.huixiangedu.cn

TS:   do { i++; } while (i < 10);
来源：http://ix.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://kv.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yg.nicolike.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kq.9csxet.cn

C#:   do { i++; } while (i < 10);
来源：http://op.lnxyls.cn

[B09] break 与 continue
来源：http://is.shxzskj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pi.huanxung.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kd.nszjky.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://st.shxzukj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://re.nicolike.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://df.nicolike.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fb.shxzukj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pt.gzmigu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ub.yuntaijiaju.cn

[B10] 遍历同时拿索引
来源：http://wc.asd995.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vv.huanxung.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bc.lnxyls.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yn.szsharing.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pb.huanxung.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jp.hahajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ur.nszjky.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bc.lnxyls.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qd.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://dy.jianghongdianzi.cn

Py:   list(range(0, 10, 2))
来源：http://vs.huixiangedu.cn

PHP:  range(0, 10, 2);
来源：http://ye.colortex.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zb.lnxyls.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jy.9csxet.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mu.colortex.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://md.521024.cn

Ruby: (0...10).step(2).to_a
来源：http://ug.bjjhwx.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ch.szxytkj.cn

[B12] 跳出多层循环
来源：http://ql.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jb.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zt.jianghongdianzi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ra.wgjwhj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://if.hnjuh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cc.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qf.nszjky.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sa.shxzukj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yo.huanxung.cn

[B13] 判断是否为数字
来源：http://se.9csxet.cn

Py:   isinstance(x, (int, float))
来源：http://zj.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://st.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ca.shtwfgs.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://td.huixiangedu.cn

Java: x instanceof Number
来源：http://vp.yuexingan06.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qn.colortex.cn

Ruby: x.is_a?(Numeric)
来源：http://kg.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://rv.haigaiapp.cn

[B14] 判断值是否在集合内
来源：http://bf.haigaiapp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ie.yuexingan06.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oy.nicolike.cn

JS:   [1, 2, 3].includes(x)
来源：http://of.jianghongdianzi.cn

TS:   [1, 2, 3].includes(x)
来源：http://kd.huixiangedu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gr.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pr.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xu.gzmigu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://le.huixinmuqiang.cn

[B15] 布尔运算与取反
来源：http://lg.shtwfgs.cn

Py:   a and b or not c
来源：http://df.huanxung.cn

PHP:  $a && $b || !$c
来源：http://pu.szsharing.cn

JS:   a && b || !c
来源：http://ru.panjiajie.cn

TS:   a && b || !c
来源：http://xh.hahajie.cn

Java: a && b || !c
来源：http://ce.lnxyls.cn

Go:   a && b || !c
来源：http://ym.gzmigu.cn

Ruby: a && b || !c
来源：http://vo.shtwfgs.cn

C#:   a && b || !c
来源：http://kj.wgjwhj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xd.yuntaijiaju.cn

Py:   if not data: return
来源：http://lg.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://et.huixinmuqiang.cn

JS:   if (!data) return;
来源：http://bf.nszjky.cn

TS:   if (!data) return;
来源：http://mq.colortex.cn

Java: if (data == null) return;
来源：http://sc.yuntaijiaju.cn

Go:   if data == nil { return }
来源：http://nz.hnjuh.cn

Ruby: return if data.nil?
来源：http://of.jianghongdianzi.cn

C#:   if (data == null) return;
来源：http://rs.muxihuayi.cn

================================================================================
来源：http://fz.bookmarksfly.cn

C. 函数与作用域
来源：http://dq.yuexingan06.cn

================================================================================
来源：http://xe.chemitech.net.cn

[C01] 定义函数
来源：http://vs.hnjuh.cn

Py:   def add(a, b): return a + b
来源：http://ty.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eo.newstarts.cn

JS:   function add(a, b) { return a + b; }
来源：http://mb.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xh.nszjky.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jw.nicolike.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ne.bjjhwx.cn

Ruby: def add(a, b); a + b; end
来源：http://rx.panjiajie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vm.shxzukj.cn

[C02] 默认参数
来源：http://pp.gzmigu.cn

Py:   def greet(name="World"): return name
来源：http://gu.yuntaijiaju.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zo.9csxet.cn

JS:   function greet(name = "World") { return name; }
来源：http://kp.nicolike.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pr.nicolike.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://aj.haigaiapp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mp.huanxung.cn

Ruby: def greet(name = "World") = name
来源：http://ez.colortex.cn

C#:   string Greet(string name = "World") => name;
来源：http://ls.lnxyls.cn

[C03] 可变参数
来源：http://iq.yuexingan06.cn

Py:   def total(*args): return sum(args)
来源：http://uw.jianghongdianzi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ay.asd995.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ia.shxzskj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hn.newstarts.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iu.panjiajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wn.shxzukj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fv.muxihuayi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jianghongdianzi.cn

[C04] 命名参数 / 关键字参数
来源：http://eo.shxzskj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vy.colortex.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pu.huixinmuqiang.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://et.shxzukj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fw.colortex.cn

Java: // 无：用 Builder 模式或 record
来源：http://pk.chemitech.net.cn

Go:   // 无：用配置结构体参数
来源：http://og.huixiangedu.cn

Ruby: f(a: 1, b: 2)
来源：http://mk.shtwfgs.cn

C#:   f(a: 1, b: 2)
来源：http://op.yuexingan06.cn

[C05] 返回多个值
来源：http://wr.jianghongdianzi.cn

Py:   return a, b
来源：http://gd.chemitech.net.cn

PHP:  return [$a, $b];
来源：http://px.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ka.bookmarksfly.cn

TS:   return { a, b };
来源：http://zh.nicolike.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://eg.chemitech.net.cn

Go:   return a, b
来源：http://fx.newstarts.cn

Ruby: return a, b
来源：http://ne.muxihuayi.cn

C#:   return (a, b);              // ValueTuple
来源：http://xc.jctech888.com.cn

[C06] 匿名函数 / lambda
来源：http://hj.jctech888.com.cn

Py:   square = lambda x: x * x
来源：http://xu.huanxung.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qb.jianghongdianzi.cn

JS:   const square = x => x * x;
来源：http://cm.colortex.cn

TS:   const square = (x: number): number => x * x;
来源：http://re.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pb.yuexingan06.cn

Go:   sq := func(x int) int { return x * x }
来源：http://mz.yuexingan06.cn

Ruby: square = ->(x) { x * x }
来源：http://mc.huanxung.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hi.huixiangedu.cn

[C07] 把函数作为参数传入
来源：http://kl.asd995.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ci.hnjuh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://gg.asd995.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ge.asd995.cn

TS:   arr.map(String)
来源：http://ky.hnjuh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cm.szxytkj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://du.shtwfgs.cn

Ruby: arr.map(&:upcase)
来源：http://yl.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://oc.bjjhwx.cn

[C08] 闭包
来源：http://wm.yuexingan06.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://du.hnjuh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://la.gzmigu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zr.shtwfgs.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ys.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zs.jianghongdianzi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fm.lnxyls.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kg.bjjhwx.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cp.bookmarksfly.cn

[C09] 递归
来源：http://yh.huanxung.cn


<!-- 参考信息 -->