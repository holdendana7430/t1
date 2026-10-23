代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3tvdktxkd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rsbxlpuw.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ouxlaufb.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wyzewntb.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3vrozqgyg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3capjvnxj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3atdlcomt.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vjlosaiu.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yhpkbxtb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3qwqpdxzx.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3qpysucpd.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3swgionhp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hipvsvrd.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3faopzfrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xuiknmic.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dptwrfql.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3wiyftphv.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3rotyszyf.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3fagtthoy.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3wqmlyiwe.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3qaugptih.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ujthnlxh.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3wowdfzgs.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3zfaayfrx.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3uktaieos.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3waawxlve.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3odvghlns.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3rdbqxldu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3aqiqmbed.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3sgpqpeib.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3zwbqxnju.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3jnmxmeqr.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wyfbkfgw.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3inlucjok.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3cjuvqqff.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3byfzkqgh.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ovagffpn.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3powkilhx.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uopooshk.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3cfnpdcec.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3lctjybyt.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vjrxttqh.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3qxlyxamu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3cwpffnef.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3rkgwybla.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3uwxdnitl.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3xhktnkph.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3vepnhiko.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3vsffrojm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3zxmkbjla.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3elueridb.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3kgyfnldi.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3rgufpkms.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3oxntrntb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3psfpofsf.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ryrqibbt.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hopjolmp.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hnjbhffz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cfqkqyic.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3aljlitbo.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3tjwiuyue.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3adtqpald.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3hyjxhgeu.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ncavamln.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3eetbpqfx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3khwofctv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3nrmizjwy.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3onjbdcft.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3fwlkxyxr.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cmmzesbu.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3nefpacnh.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3idlbgpgy.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gfzzxsvi.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3soichnmg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3yvfpvjwd.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3qgegjwuh.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3bxhcmheb.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3pktntxgj.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3sljqctie.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mgqpaipl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3bjnfczen.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ilerruvj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3cqvjierm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jhyfepcd.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3sddgsrpy.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3znfhwtcw.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3bqorfrtb.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3innueuxj.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3eaeyknot.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hdrkswuh.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mrgyxjvi.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sbhdkpfv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bioqrcqg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3lqadxcdg.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3uxjwcgek.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3eqomtlfc.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3tllivtgc.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3lfblgtuc.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3eyuorkky.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3qwwwqgbd.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3cmbplzms.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3stxjxdjc.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3lppkoyxk.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3kbvlirzr.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3dfujubpp.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3gnfygfyv.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mjyrptre.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rajbkiug.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3uxlthigg.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rymxpjse.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kikhujrt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3kgdzbnpz.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3athfvewg.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kwbrqkaz.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3oquagxqk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3yzqoiqtu.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3hqnxewyu.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3lheeddas.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3raiqfxhf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3uccbztcr.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3wpdfmbel.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3xsjkpnlb.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ydnticfg.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3bntvdohz.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mortgbfu.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ouplbokl.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3yqujbznv.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3peqdntns.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gsofksra.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zdgcseio.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3abdiwfvn.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3alzlszmp.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3vhtbtyrl.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3amaankza.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ecreykoz.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3nososbzz.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3inuwtlsz.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3poicsqsj.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3keyaannz.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3qwrjuscd.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3cbfzbtcn.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3pkckruoc.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3jzthlmpn.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3wfjptuwf.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3jkgzmbec.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3zobbsnxe.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3qztahery.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3vquladtn.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3wdzczgiu.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3yemquahg.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3geyfoylp.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3rgfcwrpj.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3encppiea.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3xfwcmqnn.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3wdhpryri.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3tdvczmfu.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3gwdfkhks.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3szzdomzw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3czjqsyua.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3kjylbaxr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vncuafgs.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zjussypr.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3sxohuaei.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3obzxlbjs.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3egzmzxnz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3sgasjznt.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3imlcbmqx.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lkiqrbhu.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3sbxztysy.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3upkxohid.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hvlejlnp.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3qfyleajq.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3czzjeown.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3cyxvjzzl.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3njmxxrux.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3jmghihmt.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3bdvgjuld.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3ohzsqrai.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ekdknjvu.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3yvhrhlfu.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3wfpmvrkr.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3qujogjsa.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3nsupezwn.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3vmffbkza.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3bqqonloc.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3xusirkwa.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3mplsudgh.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3wxpbekya.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3bcnltbgj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3jxmytzcn.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3tfrlmbot.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3lglhtmdd.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3kvfnvsxk.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3emblmaql.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3gfwiiics.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3iftcdwdh.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3qkpnmype.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3dtgdpehc.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3frqzvmjc.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3sqfpmmqp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ycxwggdw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3fkceadut.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3bvgkmcsl.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3zoirrxtj.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3iyvckfds.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nuhsetxe.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3pgrcbvdr.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3pmkjciuc.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mvxjvkoc.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cfkannmq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3jvcogige.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pvlzqjpc.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rxtzwirr.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3yvxyvkwm.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3gqwdxefz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3jkhxpffx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ehwpigrx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3bmamtmff.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3oalldreo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zabfmjbq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3rsivsjtk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3wabrmrfg.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3yegphjle.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ryvswpqx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3fkoazgst.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3yakwotar.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3hqhjiyxg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3gealsvam.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3alsolkyw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3nwwrkymp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3tqgkgbvz.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ccogujnp.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3dvfwftqd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3hlbbnygs.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ycgguhpu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3zsjacsoz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3sthsjcfq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3gdvtseyx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3dzmattrm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ynnmrust.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3ooqaluxb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3tutkcmrb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3odhvokxy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3jycpsmgq.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3nvtxnkfb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3htsdfdgo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3fycdurbt.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3vjmqrhem.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3zwlbjizc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qkulqppy.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3yzgxfxse.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vdsuudze.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3lmctaiuv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3eajdptyg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxxczgdw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jrsebufk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3tadrisys.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3irxjcgtv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3yrennuwu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3gfqptqum.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3oevcareq.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3fqdnfpuw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3egwbqyez.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3cqtsizis.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jaxpszdi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3onfiluzr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3dugxsfkc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3xiixnlas.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3uwnwclwr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3sjuhxrqg.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3wxtqepnm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3bodujcds.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zdvmluiv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zyueldzs.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3snyoqgsl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3arobwqca.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3gbrurmom.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3tqllyefj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3xbtvnciu.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3czcpewjb.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3rqkfwvue.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3egoonczt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3tsaxaats.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xwlqssna.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ystpiydm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3jpnloufk.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3tfmehdze.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3xdhzvcdt.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3alefubmq.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3sarvsugc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3opokbcxd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lsjnjowa.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3namjnrzp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hslkjcsk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3vchacyhl.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ueokxmnw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3gvzmpdeo.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3vbzdvirs.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3skxpaffw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fchjhhoa.html


<!-- 参考信息 -->