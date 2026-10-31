代发 wailian999

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rk.gzmigu.cn

【使用说明】
来源：http://jo.jianghongdianzi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zm.jctech888.com.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fm.bookmarksfly.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ug.bookmarksfly.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://uu.panjiajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://bk.asd995.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qi.shxzukj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bn.nicolike.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ko.hahajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zw.huanxung.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wb.shxzukj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lg.wgjwhj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fk.haigaiapp.cn

【文件统计】
来源：http://iu.huixiangedu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gi.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://kd.szsharing.cn

目  录
来源：http://my.szsharing.cn

--------------------------------------------------------------------------------
来源：http://na.huanxung.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ya.huanxung.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zj.chemitech.net.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ex.jianghongdianzi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ju.szsharing.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ff.yuntaijiaju.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jx.muxihuayi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kb.gzmigu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://oh.newstarts.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rp.hnjuh.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qa.gzmigu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mg.hahajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dy.newstarts.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yz.bjjhwx.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mb.jctech888.com.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xm.asd995.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bi.newstarts.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zd.muxihuayi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://uf.muxihuayi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zk.hnjuh.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jv.haigaiapp.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://co.chemitech.net.cn

================================================================================
来源：http://oz.shxzukj.cn

A. 基础语法与类型
来源：http://th.yuntaijiaju.cn

================================================================================
来源：http://wx.asd995.cn

[A01] Hello World
来源：http://er.huixiangedu.cn

Py:   print("Hello, World!")
来源：http://hw.nicolike.cn

PHP:  echo "Hello, World!";
来源：http://xi.haigaiapp.cn

JS:   console.log("Hello, World!");
来源：http://fb.panjiajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zn.huanxung.cn

Java: System.out.println("Hello, World!");
来源：http://vv.lnxyls.cn

Go:   fmt.Println("Hello, World!")
来源：http://uu.wgjwhj.cn

Ruby: puts "Hello, World!"
来源：http://az.szxytkj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wc.9csxet.cn

[A02] 变量声明与赋值
来源：http://hm.bookmarksfly.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gz.wgjwhj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://kw.szsharing.cn

JS:   let name = "Alex"; const age = 20;
来源：http://uy.szsharing.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://br.nszjky.cn

Java: String name = "Alex"; int age = 20;
来源：http://cg.9csxet.cn

Go:   name := "Alex"; age := 20
来源：http://bq.yuntaijiaju.cn

Ruby: name = "Alex"; age = 20
来源：http://uj.hahajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://yh.nszjky.cn

[A03] 常量定义
来源：http://be.haigaiapp.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pa.hahajie.cn

PHP:  const PI = 3.14159;
来源：http://ek.panjiajie.cn

JS:   const PI = 3.14159;
来源：http://ep.panjiajie.cn

TS:   const PI: number = 3.14159;
来源：http://uc.9csxet.cn

Java: static final double PI = 3.14159;
来源：http://jt.haigaiapp.cn

Go:   const PI = 3.14159
来源：http://bw.haigaiapp.cn

Ruby: PI = 3.14159
来源：http://ef.huixinmuqiang.cn

C#:   const double PI = 3.14159;
来源：http://dj.huanxung.cn

[A04] 判断变量类型
来源：http://nb.jctech888.com.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dy.muxihuayi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://li.hahajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://le.huixinmuqiang.cn

TS:   typeof x; x instanceof Date
来源：http://oa.hnjuh.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qq.yuntaijiaju.cn

Go:   reflect.TypeOf(x).Name()
来源：http://zw.521024.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://jj.gzmigu.cn

C#:   x.GetType().Name; x is int
来源：http://qd.huixiangedu.cn

[A05] 整数除法与取模
来源：http://jj.panjiajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tj.szxytkj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zr.shxzskj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lx.9csxet.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yt.huixiangedu.cn

Java: 7 / 2; 7 % 2
来源：http://sp.bookmarksfly.cn

Go:   7 / 2; 7 % 2
来源：http://qg.9csxet.cn

Ruby: 7 / 2; 7 % 2
来源：http://yu.yuntaijiaju.cn

C#:   7 / 2; 7 % 2
来源：http://xy.hnjuh.cn

[A06] 字符串转数字
来源：http://fd.hnjuh.cn

Py:   int("42"); float("3.14")
来源：http://jk.bjjhwx.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xb.lnxyls.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://oo.shtwfgs.cn

TS:   parseInt("42", 10); Number("42")
来源：http://oy.jianghongdianzi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rf.gzmigu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kj.lnxyls.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://xu.lnxyls.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xj.huixiangedu.cn

[A07] 数字转字符串
来源：http://lf.bookmarksfly.cn

Py:   str(42)
来源：http://mj.shtwfgs.cn

PHP:  (string) 42; strval(42)
来源：http://ez.yuntaijiaju.cn

JS:   String(42); (42).toString()
来源：http://gv.szsharing.cn

TS:   String(42)
来源：http://vg.yuexingan06.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://wt.hahajie.cn

Go:   strconv.Itoa(42)
来源：http://qp.9csxet.cn

Ruby: 42.to_s
来源：http://jc.muxihuayi.cn

C#:   42.ToString()
来源：http://cl.hahajie.cn

[A08] 取整与四舍五入
来源：http://ku.colortex.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gb.gzmigu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ni.nicolike.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nb.huixinmuqiang.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jd.yuntaijiaju.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://en.szsharing.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jv.huixinmuqiang.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://xp.huixinmuqiang.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jf.huixinmuqiang.cn

[A09] 绝对值与最大最小值
来源：http://dy.521024.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://od.gzmigu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fm.panjiajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jd.jianghongdianzi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xd.shtwfgs.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wy.chemitech.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://sf.shxzukj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rz.huixiangedu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gy.jianghongdianzi.cn

[A10] 生成随机数
来源：http://lw.szsharing.cn

Py:   import random; random.randint(1, 100)
来源：http://jw.nszjky.cn

PHP:  random_int(1, 100);
来源：http://cm.521024.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://tl.panjiajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mn.521024.cn

Java: new Random().nextInt(100) + 1
来源：http://fe.yuexingan06.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cv.yuntaijiaju.cn

Ruby: rand(1..100)
来源：http://jy.szxytkj.cn

C#:   new Random().Next(1, 101)
来源：http://ry.shxzskj.cn

[A11] 条件表达式（三元）
来源：http://xq.asd995.cn

Py:   "yes" if x > 0 else "no"
来源：http://gz.muxihuayi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://hv.haigaiapp.cn

JS:   x > 0 ? "yes" : "no"
来源：http://fo.hahajie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://yb.shxzukj.cn

Java: x > 0 ? "yes" : "no"
来源：http://uq.hnjuh.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://qa.newstarts.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://oz.jianghongdianzi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://dl.jctech888.com.cn

[A12] 字符串插值 / 格式化
来源：http://tj.shxzukj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://np.shxzskj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ug.colortex.cn

JS:   `Hello, ${name}!`
来源：http://jz.jctech888.com.cn

TS:   `Hello, ${name}!`
来源：http://xd.9csxet.cn

Java: "Hello, %s!".formatted(name)
来源：http://un.shxzskj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vh.szxytkj.cn

Ruby: "Hello, #{name}!"
来源：http://ui.shtwfgs.cn

C#:   $"Hello, {name}!"
来源：http://vg.yuexingan06.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ui.521024.cn

Py:   "第一行\n第二行"
来源：http://qq.nszjky.cn

PHP:  "第一行\n第二行"
来源：http://bt.haigaiapp.cn

JS:   "第一行\n第二行"
来源：http://wa.bjjhwx.cn

TS:   "第一行\n第二行"
来源：http://de.panjiajie.cn

Java: "第一行\n第二行"
来源：http://gk.9csxet.cn

Go:   "第一行\n第二行"
来源：http://jh.szsharing.cn

Ruby: "第一行\n第二行"
来源：http://wh.jctech888.com.cn

C#:   "第一行\n第二行"
来源：http://am.hnjuh.cn

[A14] 注释写法
来源：http://vh.colortex.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://wd.lnxyls.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ws.panjiajie.cn

JS:   // 单行；/* 多行 */
来源：http://sg.yuntaijiaju.cn

TS:   // 单行；/* 多行 */
来源：http://wq.hahajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rf.panjiajie.cn

Go:   // 单行；/* 多行 */
来源：http://aq.colortex.cn

Ruby: # 单行；=begin 多行 =end
来源：http://kl.asd995.cn

C#:   // 单行；/* 多行 */
来源：http://nf.shxzskj.cn

[A15] 空值判断与默认值
来源：http://za.szxytkj.cn

Py:   value = data or "默认值"
来源：http://at.521024.cn

PHP:  $value = $data ?? "默认值";
来源：http://mu.yuntaijiaju.cn

JS:   const value = data ?? "默认值";
来源：http://id.yuexingan06.cn

TS:   const value = data ?? "默认值";
来源：http://ga.shxzskj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ij.panjiajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://ym.huixinmuqiang.cn

Ruby: value = data || "默认值"
来源：http://sy.szxytkj.cn

C#:   var value = data ?? "默认值";
来源：http://yr.panjiajie.cn

[A16] 真假值判断规则
来源：http://im.hahajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pm.colortex.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gw.521024.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tc.haigaiapp.cn

TS:   if (!x) {}
来源：http://ec.shtwfgs.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ov.9csxet.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wr.nszjky.cn

Ruby: unless x            # nil 与 false 为假
来源：http://rq.panjiajie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://si.panjiajie.cn

[A17] 位运算
来源：http://fv.wgjwhj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sn.yuexingan06.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vt.hnjuh.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mu.shxzskj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://yf.9csxet.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ys.panjiajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vv.521024.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pc.gzmigu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pt.newstarts.cn

[A18] 字符与 ASCII 码互转
来源：http://ab.hnjuh.cn

Py:   ord("A"); chr(65)
来源：http://pf.gzmigu.cn

PHP:  ord("A"); chr(65)
来源：http://bb.muxihuayi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ly.chemitech.net.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kp.nszjky.cn

Java: (int) 'A'; (char) 65
来源：http://ql.szsharing.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zz.panjiajie.cn

Ruby: "A".ord; 65.chr
来源：http://wx.gzmigu.cn

C#:   (int)'A'; (char)65
来源：http://yu.bjjhwx.cn

[A19] 交换两个变量
来源：http://nn.nicolike.cn

Py:   a, b = b, a
来源：http://uh.hahajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://el.huanxung.cn

JS:   [a, b] = [b, a];
来源：http://lz.huixinmuqiang.cn

TS:   [a, b] = [b, a];
来源：http://ni.chemitech.net.cn

Java: int t = a; a = b; b = t;
来源：http://in.huixinmuqiang.cn

Go:   a, b = b, a
来源：http://rk.nszjky.cn

Ruby: a, b = b, a
来源：http://qy.9csxet.cn

C#:   (a, b) = (b, a);
来源：http://vj.asd995.cn

[A20] 读取标准输入
来源：http://uw.szxytkj.cn

Py:   name = input("请输入：")
来源：http://et.jianghongdianzi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://bp.hahajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zy.asd995.cn

TS:   // Node.js：readline 模块
来源：http://lf.9csxet.cn

Java: new Scanner(System.in).nextLine()
来源：http://nl.szxytkj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rn.asd995.cn

Ruby: gets.chomp
来源：http://na.huixiangedu.cn

C#:   Console.ReadLine();
来源：http://tr.wgjwhj.cn

[A21] 保留指定小数位输出
来源：http://cp.wgjwhj.cn

Py:   f"{3.14159:.2f}"
来源：http://db.haigaiapp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ty.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://bj.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://nj.jctech888.com.cn

Java: String.format("%.2f", 3.14159)
来源：http://pf.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://re.shxzukj.cn

Ruby: format("%.2f", 3.14159)
来源：http://gh.asd995.cn

C#:   3.14159.ToString("F2")
来源：http://ub.colortex.cn

[A22] 获取字符串长度
来源：http://yb.hahajie.cn

Py:   len(s)
来源：http://lh.shxzukj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dh.szsharing.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://se.muxihuayi.cn

TS:   s.length
来源：http://ke.hnjuh.cn

Java: s.length()
来源：http://po.nicolike.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xa.gzmigu.cn

Ruby: s.length
来源：http://hk.shxzukj.cn

C#:   s.Length
来源：http://yu.chemitech.net.cn

[A23] 大小写转换
来源：http://jc.jianghongdianzi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kz.lnxyls.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jb.szsharing.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cq.panjiajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kx.bookmarksfly.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mj.yuexingan06.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ag.hnjuh.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ts.hahajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dc.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://dh.nszjky.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lc.szsharing.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://de.huixiangedu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vp.wgjwhj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ir.shxzskj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ku.jctech888.com.cn

Go:   strings.TrimSpace(s)
来源：http://az.hahajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sj.nicolike.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hk.shxzskj.cn

[A25] 字符串比较
来源：http://ma.521024.cn

Py:   s1 == s2; s1 != s2
来源：http://np.9csxet.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dp.lnxyls.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ov.bookmarksfly.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://en.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qi.jianghongdianzi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://px.newstarts.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ld.lnxyls.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fo.lnxyls.cn

[A26] 类型转换总览
来源：http://pf.bookmarksfly.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cv.haigaiapp.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qq.muxihuayi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bw.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://ns.chemitech.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://js.panjiajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ya.wgjwhj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://im.yuntaijiaju.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wv.gzmigu.cn

================================================================================
来源：http://qb.asd995.cn

B. 流程控制
来源：http://zb.bjjhwx.cn

================================================================================
来源：http://wt.bjjhwx.cn

[B01] 条件判断 if / else
来源：http://ch.bjjhwx.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mu.chemitech.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dl.chemitech.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fi.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pb.yuntaijiaju.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ja.muxihuayi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hk.lnxyls.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yr.colortex.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pe.yuntaijiaju.cn

[B02] 多分支 else if / elif
来源：http://ot.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kp.bjjhwx.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zw.huanxung.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ok.nszjky.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://np.huanxung.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vm.asd995.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ll.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://re.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tv.bjjhwx.cn

[B03] switch / match / case
来源：http://kh.huanxung.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://co.huixinmuqiang.cn


<!-- 参考信息 -->