代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mlapbblo.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zazzfqrq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kadxqvyb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xaeskkhp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gvuxcnaf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2jlgzujxb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2wnmqixpj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2gmleirdz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2danjtvke.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2ipcoajdz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fqgpultl.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2iclghlah.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2eptoaqts.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2zgjdvllx.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2yqorackq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2vxgceqpy.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ynlybhlc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2vvbprsnj.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2gpmgvjex.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2vgdvkncc.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2wdlcpaay.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2xvpbrdpz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tszsnzvi.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2stmmqghu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2ujwsvgpm.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2bnzvkvui.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2kamxgkrn.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2rgqkdyih.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jplspvmd.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2lvuydfut.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2pgbgccju.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yfnmudmb.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vliuhusj.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pkbwbmbf.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wthdlsgp.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2thgxztqz.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2grnbvgwq.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2emtdlsae.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2fvalqbjc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2yexyovtf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2vnbkyzmm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2rsacugpd.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2azwuaoso.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2dazdzoqz.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2qjzpfgdq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2eemwehkd.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2nndkfdqe.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2oucuhbmq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2fntbjhkq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ndxhaelr.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zeofbfab.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ihixqaaa.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mnlaynny.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ueerojmw.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gawfmgxd.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2drnuhwwb.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2axppqjji.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ycesidkz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2cngnanvg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2edatjpxh.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2lxpiaocd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2etkvpanq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2noxukhnr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2wuedmgii.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2wgghwzpw.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2etowcbbw.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2zvvdcmtt.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2wskttblp.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2djontxnw.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2uqptqyba.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2ptwhqyyu.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2idqnnyhb.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2niqrlhun.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2wtetagip.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2jdojdxxk.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zamlynjn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2zxivogfx.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2tdxmconq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2crdssrzi.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zpuyelzo.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jeocuwpo.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2ivfripom.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fjrsfpfv.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2izfpfglp.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2akctowjn.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lukupmvu.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mefasneb.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zaaxupdp.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kvpeimlk.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2lfzqswyv.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2ehgturdy.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xopwjxdu.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2cizptcpd.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2vharydcr.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2mmtxkzqb.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2lmydgjqw.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ypyyrjnz.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2vuipduwo.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2zecpxvks.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2ptamhxfu.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2vwmfleuk.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2mtltfhzr.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2dcjvymtm.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2uilhixve.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ovuvuouy.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lzlfwksm.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hdltgjgy.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2qaznpgwr.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2imrvjymk.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vqleafma.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2irqomuzv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2olmpjpoz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2awvirycm.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2iibykjtu.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2tebpizay.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2miqyirnw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2uokssfxa.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2phuxhfez.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2cvqyzxji.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2tbhwyusa.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hoqyxgnc.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uvkyjijl.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zenzsljh.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hjgoroco.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ucbaeobu.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zdivboub.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mrlcydzk.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ipepraez.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2yhwokcdg.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2xmkbfncd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jollijcm.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2casntccg.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2bkofoqkd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2wdcspyur.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zvvavdrg.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2xepxspjo.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zcqjneav.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vjvplxdd.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2yhehnlty.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2lbeyzrlp.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2txxprrse.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2omumpvyr.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2ocrrxjgc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2zajtqlmu.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2xtyckhgm.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mzksaetg.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2mymecoje.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2bwcniuut.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2hkmhffae.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2ergawrxl.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2ouinnjus.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ekpxsque.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2fdwlttaq.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2wkovwbuf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sdsgxttn.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2yfyfwsrq.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hwwejesw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2iibrqxdn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qdvrsjvq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uocrzmde.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2euduptxt.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rfamizaw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cqrpzsxg.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ifnwtbui.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2uagxkorf.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2crndypeh.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2xukzykpr.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ejccnhni.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2kagxriky.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2mvxfttlu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2xvfpnqom.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2cqnolzlm.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2blhlkust.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2gmtggrdm.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2pdwnqgrq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2zhszvddj.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2bnkvbvng.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2eneqpxbv.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2zkjtayxf.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2drcjxgzv.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2qpboatxu.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2cjeoaath.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2dnnkmpqr.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2ooisdktp.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2cqlennyx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2xjciwkxp.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2whjkblwv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2tcgwrbas.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2qidtmzqe.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2duainfex.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2tkqmjhkg.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2kdemqvwd.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2yjpxszlp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2pmsrgvzo.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2drapxjac.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bwyrxjvp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zinhqdtn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2mahpqiku.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2tytcqonp.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2xdykpxir.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jihdkltl.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2vsfenhke.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2ueeofvyy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2jkvuxpba.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mmcivriv.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2dtjvyaqn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2vqzppriw.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2xabplcbb.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2lkrpjhcu.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2nxyizkco.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2bdgseccl.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2oesjvrcn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ilzcnxxy.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2lmnptmec.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zkkvbmvg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2vdtodhqt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2zgfiuhbb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2ylaeovts.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2fxlzxyhj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2bejusnji.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2fmrluiaf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2khmzcptf.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2xdklbqkp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2nmvdhtqf.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uyivxixg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2umecbifu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2snjawkzb.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2incuqovp.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2nqapdeuf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wmvdqyew.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2saurjgqg.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ajbuljba.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kjahziez.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2abimfysz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ohwfozcr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2hcjsbydv.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2otlyuwkl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2pleyoxrb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2bmonkbjo.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2erazejpi.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2pikdqsze.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2nngjqrao.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2aiupwgbp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2fcstgfjd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2keolgjtx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2leydkank.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2kmqotgba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vvdnomel.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2yrauhpzi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2dnrgmqfs.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2msskrwrc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pgattmzo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jitsjpeg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bcpuuuwl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2mynwowhq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2nzvntics.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bilyvbdo.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2xamtenrt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2xhlsiras.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vaxptdsx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cjwlasjx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2obkygtrg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2slypelid.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2cszywqir.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2pbfsipqw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zgthbxua.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2qkchjvpm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2zlgbupao.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mudaxdon.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ccrnmfkb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcquopcg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfjiwurd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2wrvegakd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2kmbjeeoe.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ofptbfye.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2dhaxyzbt.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kigipdtz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2hiesxotl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2fzqmdphc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ransfktr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2fghvqruw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ovgzudgo.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2qfgzzcdn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vfueykmw.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2fttqgqvc.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2glfqckkw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2irvmeqlp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2osyxvdig.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2nbytgtws.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2lbapdril.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2bjitoaxa.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2bsmicsjk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2rmkxcggp.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2bgchhldz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2hkrlhrzy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2mrjzpxen.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2sakzsvcp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2qtffjfeb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2uhfqmesu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2uzmmshgu.html


<!-- 参考信息 -->