代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3juirypvj.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3dijobqsr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3whbhkesb.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wchgcduw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pmlgtehf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3ouhjomcw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bpwlfhex.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3frgrukct.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3tbwouzfe.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3vnwzxfhf.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ggyalqlq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3xleveqpn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wqmgyzqs.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3gficaifk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zpbytdjq.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vkrieedo.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3gjbzfspf.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3adrgszmo.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3tzjqttnw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3fgedjmab.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3vdwaczcy.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3rsmhzfrl.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3sfahmofg.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3opabskzn.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3vxxytsgj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3ycmzmfkx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vmaclimz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3nsqelvcx.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3fwyvgxxs.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3xpyuvbrt.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3zqmciayk.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3hduxfybj.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zpoopbpr.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3cfjntifm.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3hzvfuodx.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vodunxdj.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3apykpndw.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xlhmizys.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dbrkmfcl.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3muuwntxo.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3svsxoryi.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wobiwneh.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3zjrtaybx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3zeqaxkjo.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3kpgtgvkm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3qsiajtiv.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ptgbnvvj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3qnflgnkc.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3qddmqfym.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3acqxamro.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3oejbrjdt.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3tjiaqweb.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3wfjaownt.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3awbmgktn.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jmdkskdh.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ydplclqz.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xrbbvuzh.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bkcbdavi.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3awfwkllj.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ltljuibs.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3vtybkbgc.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3hthpxisp.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3neqprwbv.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3lcvsuxph.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3dcuujvwo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3zwzytwkj.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3xxduqnpv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3jzkyjfsk.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3trtfblgu.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3vbgocmiu.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3dcfphqsb.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zinxltcl.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3laahafdj.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3cyqumnlf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3ngheqyhm.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3bcjokqck.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3iifidacy.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3ngbaiofb.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3kxgpuyof.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3mdxsqiig.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3gmbcykle.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3uxljnelm.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3wtnxosgh.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3pljsdvrw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3bztluczb.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3yghvndgr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dmbkuvcu.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vuzidawv.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3izbrftvm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rjpedwjf.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3eewzubod.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jnhttrgs.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kyjrezyo.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3squixuod.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3naaolvrw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ravfvmcs.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3cemprdyl.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3dvxazpvg.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3smgzvuje.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3wwdvfmfu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3sppiwjdl.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3tyiimisk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3vijevxew.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3jgtwcmdn.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3lrdetjgg.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3cmnnjnpt.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3icfsspto.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3seimywox.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3uweoliqk.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nzxbxoam.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3iupwjlss.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3iyqijmne.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3atgocpvn.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qrngnawl.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zfzuxmkv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3ykrscxbd.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3uxuckjqp.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3eaxaekvh.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3toxoflzd.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3nfbylufv.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3trhtqsat.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3jaqgrbqx.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3vnwsnlvg.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3aqqorywk.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jmjxunfg.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dmfqfdun.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dqgtifce.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3yflpxubx.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3miprwyxs.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ulpbrvyh.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zfyhwppp.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nxymuxxs.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3mhwfknew.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3xasygpug.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ammwjrrz.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qteattuj.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qlkerano.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3pteekrwz.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3adrmpzoo.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3varqcrxc.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3coqlbqak.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3djoufset.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3leoksvdj.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3konebgyg.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3znakeluz.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3uhvkyiic.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3pklnymfj.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3fwinoctp.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3vaddtdav.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3jwnjinyv.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3dtvhwkrw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3opycclcy.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3flogwcqn.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3hnvpiytg.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vopevdzp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3srkdznsi.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3kmsvsxsg.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3hkfrlplc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3gvxsreco.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3subodisz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nhbsbvpi.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lmajazyv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wjgjefdf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mnxnfkdx.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cuemkhdy.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3esbiynis.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wicbkcxe.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cyaihwhx.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3dtcsdqqf.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3lboopygk.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3wlqdqdqs.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3nvujaaqv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ajhworah.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3xxstkaiy.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3lcikoqpx.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3rfsfhesq.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3vdqosrmb.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3idlugijd.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3hqtgpeuf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3umfrnmej.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3hwkbzlur.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3jyimntrq.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3lbmgvsin.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3tpowrzoi.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3hsbhbwhv.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3ufzvenjr.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3kaciswjo.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3usgouwji.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3mtupeulx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3gcrszidh.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3btyfzgom.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3uchiqhvh.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3edsbjdyc.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3euzlwhdk.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3fmhjxyad.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3gpsexjvx.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3zszodzaa.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3nkhxaybo.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3drimvdpg.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3qqxraexi.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3govxnpnj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xnhpebuz.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3nodicztn.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3expmrfvh.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3dyiidvmj.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3antiqrfl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3uosjnxfo.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3szovypog.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3thxyznqj.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ijrqdioj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gizpryah.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vmlkinkb.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3ywpakunb.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hegfgzqu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3pwwzsmsc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3zcqdooyx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3opqrhoeg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nfgptysu.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3vazjxejy.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3iikqxaiy.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3uftgqxoy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3htnpesoi.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3qqpcchoc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3mrabfvlp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3ofworlpj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3qoqikrfg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3mjqcdnga.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3spnwistk.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3azdsxakn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3yuplmcww.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3vpndrtci.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3gthvxkbt.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3kwpcvlex.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nuvwrwha.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3crztyctq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3guddulxf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3hozfadtr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vecytbtz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3fgwrfvzn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wdifwepj.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3fugzkznq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3nagbgbsi.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3sdsbnmnz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3ofjddero.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3fguyobnw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ranycipu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3gekrgccr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3nfrzczfj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3zescsxpm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aqscinxn.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3oiowojey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gpgmroqd.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3ozrtlkol.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3koqqapqo.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxcvrduj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3edgweskc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3pejyqjfp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3owyytgnz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3bjrgktpa.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3xrvxpkak.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vweowylk.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3ljbjizpt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3isknhgkf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnszwhlj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3uzgpxrbr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gwtofbbr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rwvkfyty.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3hpdbsype.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3liuexbvt.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ankywuzi.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3honvcgkt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3btsnabhh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jhhylssn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhxqiphw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3uljyfirk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yunmzexy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hyxxtxek.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3pmiyoptf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3frqqtqhb.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3dgrqxwyv.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3tbimnujt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ewygohdv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ujtaumys.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3sxvnbafi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3mfpxddfj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3ssbvhcng.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3eqscszbw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3bbfywjfq.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wlgwkqdj.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3qdpbjwvf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3gurpbnwu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3wbvnixuv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fsddqvcz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3dtmzknfc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3jfaermpu.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3wtnucunm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mvadbpey.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3jxiurkoj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ipvuxypv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3iqolsuez.html


<!-- 参考信息 -->