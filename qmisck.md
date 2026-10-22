代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uluprjdv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xbqiystz.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jolluzch.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nqvsyuvj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bunkhqij.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2mvsgsyun.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ghycjprm.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wzifbuaf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2xzbuxaxv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fevszjwu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2wqxjgkhs.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2pguyrgug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dvnzupnn.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2aggyhwds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bhpnuufr.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kvzoyhsy.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2axbjfjom.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2icwgzsln.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2afdiyppl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2cbhcwcuf.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2otkqocpe.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2xymcnjgk.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2tvclnzrw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2guemcjbv.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2byytnxyg.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2uqllbynp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2adyijukh.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2fpihodei.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kbqpyztq.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2fcaxplnq.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2nwehbuug.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2zdnktqmv.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2pudzbpeb.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2eificmou.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2pjrcjuqa.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nhodverx.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wilsmogf.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vxdgkazt.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2akbtpbom.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2gywmmvpz.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2jiweaeos.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2enpsrvjy.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2bancogxo.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2sdbhgcta.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2mozeozxx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2bmhkguuo.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2oovqqaqc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2szxufjri.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2hydrqhfb.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2fwmlevuu.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2aiirtzjo.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2vmyulbvm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2zuutozyt.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xgcpcaov.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2yfmauqtd.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2layztvpb.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qjjsfibu.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2chflcwam.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2aqgabncv.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gobjclhz.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ljgplsng.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2xhvgtgvy.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2sagnikxk.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2fzgqanlc.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ewfrniys.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2yyrwumix.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2qbhwvbqj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2xseqzkxh.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2oaderrjo.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2elxtcwod.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2abuvqyda.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ytsybbng.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2xfyuvxue.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2gulezocp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2evdmiudj.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xiteublz.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2lqllkzxj.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2dirwyhjg.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2wedajanv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vdttvnzu.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2bvxjzqzd.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xfiyfmiy.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2homdilho.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nfooigqj.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ecuhtacm.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2ddlcsabr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2iexybgja.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2nayuuodr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gpxndzte.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wjgkrkup.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tgovinch.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wwcbyepm.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2snnjposd.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2vbqfelrf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2wigszodf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mcwbdzlo.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2tgumhnuv.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2vnpjfoag.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2skclpecm.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2abjqzlff.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2xponwzzp.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2evhdgojc.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2zmqqvedl.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2bwhwxcsw.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2kpsirpfa.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2gwxjqwwh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ofccmxhs.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gnuocpdm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fpydlsry.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qucmlijr.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jemwineh.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2ebfgurzx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hmukwpkp.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2tnfrmbyp.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2aorvjeic.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2tzcxlqld.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2bjwpnsms.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2lmaivkgh.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2plcfoqcm.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2apztoatp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2smfhugok.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2nmqdvffz.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2bvyifyuh.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2msmmdovk.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lpwakjlv.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zijfgdsn.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tfrwvzfp.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2sqswarry.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ifxyruxm.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yenzufoc.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zqeimrml.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tlybrmpq.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2nmszcony.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2cycuplac.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zdywsbjg.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vaaxfjpm.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yjtttpmm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2avofwytn.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2sahmvmrh.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2xtqlngzd.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2bmnwckro.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2phlzrmgb.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2gpywmyml.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2plfsfqbx.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2pmhzlqne.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2gtvdkldi.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2ncjlphmk.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2aviyiqnm.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2cnkytzbu.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2lppoawod.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2twewvozt.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2yvntztcc.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2aeichbma.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2jmnxayai.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ucccblqi.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wcpeiauq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2xmjhorvp.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2lfqqgrhi.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2refdaywi.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2ualhyorw.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2azrgyifm.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zuebxrme.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bfprbxkv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bhunallc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tgmmjgue.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2prrmhzwt.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ldcryfku.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2oonflosi.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2ejmgpmjq.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2rucpgupw.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2kxeppawq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ivvwrcwh.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ykbyrbbr.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2dquhpuvz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2ymxxgxbt.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2xtdoaxqj.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2fpshtcva.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2poucphzk.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ayvtphph.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2qmhziaef.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2rksoiewq.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2uxqxxvxm.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2dwyhuhqh.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2prsmbtyq.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ynyojnhb.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2yxnrlqpr.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2bslcvovc.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2vkhicocg.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2eyliwmco.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2ycwwjxtl.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2lvjisojs.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2zmnywlpp.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2sjedgqqe.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2uqlydncj.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2cxnaikre.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2ukoybrtq.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2zfzzwwwr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2najbnwav.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2czfbyszr.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2igxbxwel.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2lztwfnyz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ebhvlyjw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jzyxoity.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2grcitcyb.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vfalkprm.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2fxopaniy.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2ctffmrli.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2teqhijkn.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2swbsppfh.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qxpnhpop.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hbvqekky.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pnfeiemy.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2edmbhsna.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ossqyrdt.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2spvfivme.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2jnyvubhu.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zmrxbuvj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wajqhbky.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2opuxuzga.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2dyqduuuz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2mblcnead.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2zfxsukue.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2vrxpcope.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2qilhaoxi.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2memfxtsb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2uochcgvx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2scqbaffd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2nxtoskal.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2khihuhzy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2lzoshbrv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2opkjnzil.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ixeoulcx.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2fmzllnru.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2rgbffslu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mbplucng.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xygvudjx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tqpugmsn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2knggykht.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2epnlcvdv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nijnwmwy.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2buochvmz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2nhcolfql.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ukiufoui.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2smtjsyzf.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2tltcxylw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2opgpgekd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2jaxiahkz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nslghagd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2yxjhvkqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2emvhwwcp.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2nztcuves.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tmgorlce.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2nutgmcxg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2yqlgtwsh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uoweeztv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jsjuvhdm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2gswtxsbl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rikacqae.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2rnwqlpfd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2nnytcxsz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jajtzwbi.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2xzdwccfp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2nsxyyyet.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2nbuckjyp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2sxbhvnhj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hmbsegbj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tkffhzgu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2pvcnptpr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2boeqbjfr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2falqvrsr.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2cvczhcpx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2swgahthf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2istghmao.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pcidnlqw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wntiipal.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wysxenjn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ovqgpmnm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2pcckvrxa.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2jjlxzviv.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2iajlbgma.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2eegnqwkf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2cffdgprg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2hxiebwuq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xugjlbia.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2lnvhfwdc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2mlfaolvm.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2jmwqaxxc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vuvbobxn.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ogwxprfh.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2orntcbdb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhgnfiek.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2rmulbebt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2sotwqrwg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2xlletygx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2xlxpqmne.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2bmvgdomw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2shjluogh.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2dornydwy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2nndajusn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2imkupybz.html


<!-- 参考信息 -->