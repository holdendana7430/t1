代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2crrbdiys.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mtdcklcl.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pbbugoma.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2pedevqqs.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ztsjlbfh.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2zlxdvbrh.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2pimgcqwk.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2xgjudbyb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2tvspqcfb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2lhcaatys.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2inrpmgha.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2snqkmovu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wiiczaux.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2nzvwevok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zubdewbu.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jjhrecah.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2ldektlfn.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2bzkgsxqn.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ghxcevqj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2jzytyjwm.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2fayelxdo.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2lxyqxsel.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2exjkjckh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2mktjeccl.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2joajcdhl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2vmxsxwve.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wnykrxut.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ghcbmczi.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2iwanfmrh.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2qiemmhnx.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2vxgwpjcg.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2unvybaho.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vwbamocb.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2kusarirc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2melqyxtn.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ourhpssv.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kxutjdro.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2oasdlxop.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jptpbsbb.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2pvxmudik.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2hxmzelwk.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2eiqzjghk.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2meidnzno.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2pftzyebj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2jninzebs.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2yhsrbhlw.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2mgxvfgnt.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2nuzbzlku.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2arxaczud.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2qncoojyn.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2bjenvodw.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2svwtkwij.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2zhvuamre.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fpeiksxi.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2oikljosm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2yboctiie.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xzaygeeo.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nqfczftw.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jmtbhmhn.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2azaoiqdx.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2jurntemi.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2sougopms.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2slcogdpx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2zyeotgye.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ghpudlvh.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2suqkbbyl.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2ugrgqdbi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2ioozvjwn.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ffxlndob.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2exmnezsm.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2vadcezva.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2qrgxzuvm.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hsyppajx.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tisspnay.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2pyzksbsa.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2ibirkvhn.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2otpzlkxt.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2xnfwefpa.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2ummsxwra.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fqzymqch.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2yharxbbj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2btlqwjih.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2qcbtbjic.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2qdcdszvd.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qcnoyliy.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2rlxjtmgm.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hunmghai.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2xivlvdgn.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gtsphakr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fjefycma.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nmygabjk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qyxajkhn.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qwvbewdk.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2icrczsks.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2dukxomzg.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fqfjwhwv.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2pprlcmhl.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2hhrrojhv.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2ofmkihfn.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2wnilghpy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2bjytiath.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2oifekmne.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2xfbhbqvl.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2zicwsivk.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2tgwglhzc.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2wlwfpuuq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2uzcglxll.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mvwahfme.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ovcwwvqg.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2pdyadhov.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gehabsth.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2ehidjfyl.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2yrkludfd.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ptdbhkcb.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2sqptoidg.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2ysdzfqzv.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2btwxipnh.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2cpbqvckj.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ygijowmw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2fohzamuf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2aerauxma.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2rjlzaxco.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2hamsuart.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2fqnnmjor.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dhbyiyeu.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rlerjubs.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dfwocxdg.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2caroywyp.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ynuisxks.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vofjxlnt.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zdsmtkkl.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fbnnffrs.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2scneqfme.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2rjdxdzma.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kuvmkqnh.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ohwilqhe.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wvkezsnd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2bhojklrv.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2oybdrpgx.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2mfghbbnd.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yqywixyd.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2owwfykmi.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2nkyvpnmd.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2zjiffbdt.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2xldxouam.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2sayldvoa.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2tlmowylj.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2tmhsengn.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2slvkjlwr.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2tkjitsmj.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2skmexxib.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2txqibiuq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2mdlylwsb.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2olvjgrjb.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yorotrid.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iuogsvgn.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2ekoefjyw.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2sokbtrfl.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2cstmnvtk.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2vdnjehxk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kggnbpqi.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xttxymyb.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jdsyveam.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xklnnjce.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ggwrbhgv.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2junuqdnb.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2etsqxset.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nulszmsl.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2gzleumhm.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wxifjjfk.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2fkmdjxov.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2tnloikdm.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2qnceuxtd.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2mqrtolar.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2hbvpweaf.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2atelphmw.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2pluxafjw.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2irowlqbk.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2oplzxvks.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2quuwdiax.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2uxewwnsb.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2hmiynxph.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2wmdarxvw.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2lvjothvz.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2wkylhacw.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2psaaxubw.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2insdszdk.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2vlgxnhxz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2uwyhyssb.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2viapucku.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2wfwvzwwa.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ewtrmdlj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2bncbjmhm.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2uukmknww.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2xzporyos.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2dwacljiu.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2fkznwbom.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2kbrgmupd.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nxyprboe.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ysvizuhx.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2npctovwa.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2sjmqqxpd.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qlurigob.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2agxhqcfj.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ahvthqxy.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2ddoyhuus.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2itklbxut.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ugurosfo.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2riwawcsr.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2vjodqyfj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2awxqyucy.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2rzpvyaaq.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2rgdlqzcu.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2pdtzhamw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2xdaxfgcr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2calrvwbw.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2rycztzsn.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2tlydzaak.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2qouaxgej.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eiazaqav.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2wectsbzd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2djadrcmp.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2hgagnbul.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2mgobdava.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2tfqrlyae.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2rgbdmsse.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2klkbllct.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2tgnghsfz.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2qvjypcoc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2lsvhfzkk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xvggsaev.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2qizefgzo.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2mbhbvvmm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wlngkuli.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2hkuwaoqu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xsmwqcen.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2esvsiqeq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qolookbm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2ouwcvkpd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jfxwhcib.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2ygmrmrvl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2aieekipr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2dhubnfvn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2nzixkaby.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2kykeslgb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2dbnlofbg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2bbaklylv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mxrgbmfl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2augerlde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2spzehrlf.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2qdzegwej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vlfkdrbf.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2cmiqhwpx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ymjygeqq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zllidbxj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2iicfyame.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ocycgcpk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2czcyljqj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2umxaibll.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2hvuzhghk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2lqlvnnhl.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2tucdzbqj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2npvgispb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2izjvsrzi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ljjbdspy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2chkbmlbj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kdagsfkh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2sulaypzd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2ebsrpczj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2txxucmjn.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2cpacgpzs.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2sakaxwsk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ngutsjcv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ymctlmrm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wviztcls.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwfchzua.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2wicodycb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2vcbkzwwx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2huhcsrop.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2jifkaeka.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2oxgvsdwc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2lpnqwdhp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2lycsxqun.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2invwljux.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2zliojaou.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2rhdnjsvd.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2kbvtocwo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2kmjxinex.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2jhrtbshc.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2tinoostq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2twhrwtyw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2giozffwu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2outvjcgc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2akyaxyld.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2jqxwnnis.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2uklcrxgj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qrrkceih.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2gmdkgexf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2buynpacm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfixlizn.html


<!-- 参考信息 -->