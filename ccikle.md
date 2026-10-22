代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2evpgstmi.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gkimtgdz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2tfawcaxq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2jldvskcn.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2gqdmvqzd.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eftmnuwe.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2wxwkhpbl.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2vxvnwsle.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2odswzjug.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2jbrrtnmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sebghmsn.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2rygkrjsr.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2jvgjnssz.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2pdsxsqix.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2sppveelv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2xcafgzqt.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ekkczrlk.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2xphwrmzv.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2ytdlnazf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ylzcurck.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2nanhgjim.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2gstdzqqp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kxcgumho.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zgeaadzz.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2dsurjons.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2cvpihmjz.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2xbdnltej.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2gfencxow.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2itrziftl.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2erqqvlvq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2qhwnaygn.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hmflcxqs.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wyyptnho.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uewyyqvh.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qpuzdmwp.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2fdwcnixx.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ofidezge.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mkyimugs.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2qzejxwmc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2xxvhvsrm.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2gmpbddrz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ugfjbesp.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2rtimducr.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2dqjxrwlr.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2qriheuhx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2qcdpobrl.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2qoptekly.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2ehofjvcu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2vpfmjkxd.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2steadvqd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ymcfovwz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jilhbkzg.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zlyolfhb.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zigripdb.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ogpatscm.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ilstkisp.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2xokywpge.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2gjeruaha.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2aqymjokf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2dflfxrxu.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2esboscyi.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2baailnjw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2bvpabtar.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2txvesgtm.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2gdgexmpx.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2naunxgfn.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zzxxwbrf.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2ailmzfmb.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2xakcdjgc.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2ugrjrvhb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2pupapuph.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2yosdmnaa.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2fnvyjoax.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2bmoehqyn.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2lisiauod.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jqwhaaiq.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2fqcrdpuc.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fgfdougo.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2zsfgnmdm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2bcglsxly.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2boqjnhsh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2wzlyzamx.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nutuibih.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2tkljaczd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xrufmnow.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2eazxvihy.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tfbintyg.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lpnphkmc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nzvmadsx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2tbtuydqv.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2intbuoul.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zdyqpdfl.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2xrywfwcj.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2tdlephcv.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2vsayrthk.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2bocacoms.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2qczottsw.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2bmglmbxb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2pkyqalem.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2vggrpmet.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2hpnywyen.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2zcmevhhk.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2apmuflis.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ixtsdphe.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xpuzmdfq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hzqchrtz.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2oehsabmf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2jpaqwrnx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qcpafuuz.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rqhguivw.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ahfnvqpc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2mfgccebe.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2edwvomhk.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ntugvpjy.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2phktggkr.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2layynnwl.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2ufgodjym.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2uutsjbpw.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2imaizyxt.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2uwzelfaf.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ydyisbum.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vbtqyntd.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ufnafjog.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fotbhtcg.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qvbcoqaa.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qzcsiiuz.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xcppftbb.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mjpbctfp.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2zrrssgtn.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2lunypcwg.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ncyevrjb.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2awatrvkw.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2egydjgns.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2fsqrpwhc.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pkwcfclj.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2yfdkomqr.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2uicorftl.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2lpttojcn.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2deohaywz.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2lloztyzs.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2goguwkdd.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2agmxtybl.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2kpgiymbl.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2ihpccuqm.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2kiqwudmj.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2aocoedrn.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2yyvnatck.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2nbvmneov.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2gewzmeam.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2gkewyxop.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2onkxlpuc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2vsewvzmr.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2sutbodcx.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2nfvwzwaq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lhnhsdlw.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2vyftngst.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jiitqyae.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gnxoderl.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hpxabafe.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jobnnduy.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ztfddyis.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dwztlihg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pvmjhtln.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kfkghaju.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2giajorvp.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2uzsisnbe.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2utrbauoe.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2jbvyruza.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bmxpvnqk.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2ynkewehb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2uxiddtyd.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2yqzyitjt.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2cqlalteu.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2egdqfryw.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2kcymdeap.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2txkwryxs.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2dtimmsub.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2odwsvpzt.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2aruaywtl.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2nihtbtei.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2hgvgcblp.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2uoixlqto.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2rokylwjs.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2bxodukkb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2daawmyjz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2pcsortgh.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2zhjovgey.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2mdjjigsi.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2tcigebrm.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2ixkecllc.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2ewrsezzb.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2gedutoqu.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2chueiqgq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2adpmoqwv.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pcqgbhqj.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2roripopb.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2rsugbfya.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2llsnujrh.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2awpuzkoa.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2bsrdbthh.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2gwbamnne.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vjvzlwot.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2cvoktczi.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2mkamdxqb.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vzzmlwmq.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2egmemcgr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2jcnrskyb.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2geigkqgw.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2cujvcuef.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mfvcxzgo.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ikwqjslx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2adgwrnxf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2rlllepfr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wognqltc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2spajgmoo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2mbbwpjoz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2xxernrdt.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2lyeezkix.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2eityzvsr.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2roqokcvm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2nbueskgu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2yiearkls.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2odissqdv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2anzubjqw.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2icidvvis.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2dlfhqkan.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2eegjmeru.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nxerjmng.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2dvgogkej.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lzdgphyw.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rjtyleqi.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2znwupuux.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2mzdzrvqv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2xwlihlik.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2kvzinlix.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2hzmlzfku.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2wrjqmxkt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2bgavyxgo.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2gjufonhz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2rrnijbtv.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2jzqzufip.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2pvyejquf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2bxnfgbof.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2huadxeio.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2eboajirp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vlpnmzme.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2rvducqak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wzprlwws.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2bcofiefs.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2uwpluzcr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2behrycjc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ytqrkkrd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2urenqeoa.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pvjauckt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2tyycobkn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2qunpepmx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qmxfeuom.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2wcjhevfh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2elhuktuu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgdiicrl.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fqfkpjbe.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2bcnoeelr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nxtfffly.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2jxuuldgj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2vujqhjba.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2cnhlrihk.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2wilcembb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2cqdrjudm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cahqbmja.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijxzrzmz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dffbvrdq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrkmroby.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2heyvxqxa.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2aionfokh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2xwbbjdwp.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2nqzcxwpe.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2petbxlmt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2prjfcybm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2uyciddxs.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vzmlxoyz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2nzbodvqc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2tqinhipb.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2lkeegvwz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2sllvrlps.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2xnrcbvzb.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2bwrbwdtr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2oyslzqmi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2dtufzqjp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2oeulspet.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tfkjbdwq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2pycqwjcf.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2yzicetgx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jqvuwxmu.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2efcduskv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2jfzofugf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2vgjcmxau.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ngurjmtv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2wfloblkf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ugnxrfra.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2eoxrenvx.html


<!-- 参考信息 -->