代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rjqmysqo.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rntqwdwg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2pqxaqjqe.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2uisyyzzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pkduyaug.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2kxdcitry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pzsfdxhn.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2msuiavrk.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2dvfshria.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2hdvrgteh.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2jgxbgaza.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2nlttrvgs.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ghghaezb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2nmdlzthw.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2dtriymhl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2onhanrvl.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2otchsrvz.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2ivtwrfnn.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ydfegztc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vvfabpbe.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2gzmyfzuw.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2sbtyjhpg.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2nyjpqugi.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2sqjofqom.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2lkpmnvui.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2imbkrmxp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2owopkjsj.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2adqzrdls.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fwxsjkzt.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2szwtuqsm.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gvzvnsdh.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2txkccftm.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2obuyfdas.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gcxnhjax.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2thbaqthm.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2cgkcdyjg.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2gntnrgmi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2wslepfcg.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2pvhsarfh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2ipuykofi.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2hyelqsuu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2cjmcejxv.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2ddtievoz.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2gwpsjxgu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2beyvmtjc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2welyyjbn.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rpfrngws.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2axskqkvb.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kbvnjvml.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ckwufgax.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hcqtvgcr.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ejevmqip.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2nsahntoj.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2nrjqcsyd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2uhkxxxgx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2oruzqipg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2cbiwgllk.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2hzwtuhan.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2fxdlfwem.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2eewcdbuy.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2valegjqj.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tpqnedyz.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2nugvtlpe.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zirvxkis.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2xoixhggs.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fyrnrmbf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2erdknwim.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2kcsajrdz.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2bfjgboqy.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ckbppsrv.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2bybjcnnu.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jhaeacex.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2hrxvkxbi.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ovbejkdx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2zejclipv.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2eoctuxeh.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ncruxtbl.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2bqmijtqq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2qskfijiy.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zobstrfy.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mliqfvum.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2plzmddpd.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jelwzrlg.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2egdosnes.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fqaqexsh.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2usyirddr.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2axmpffxs.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rlqummwm.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2zkietkzk.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2etxftaul.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2cwhgykbx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2drjkkliu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2zezimbie.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2zlibobey.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2oaxwjnka.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2kuwwgjhz.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2opakifmz.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2votvydyx.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2lcjnexqo.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2eaoyefxq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ynzrapbt.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jaerjcsa.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2adcdyhqr.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2ahsfepgt.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2emvfvxwm.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gkmugmkg.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2sqinozos.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2ldmvokwa.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2cuqahywp.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2qnctfygd.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2jxlzjrwo.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2xnsbrzwp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2cdxzbskg.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2yukjntrp.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2bfpvlzpu.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2srgnonua.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uzxnbqas.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tvvmjqmq.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jrqywymg.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pubwrznh.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pghrywxs.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hsppydbp.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mviyowah.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nkqfaqzf.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2kaodbgeg.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2djknqwkc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2whwkubic.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2opwdaahh.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2cbmewixq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2frdtkupb.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2isvrirwd.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2ckuimomm.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2bnbwjprl.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2zkmejagz.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2fanvkyrj.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2luflphsz.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jckuyzcl.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2lsqctqkv.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2xvlytqqq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2kjyzpuqx.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2yjtcorgi.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2sxwdnlpu.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2yszucihr.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2tmvrynlg.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2ofilrhsb.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2gfwjjgsk.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yjkodlsd.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2erugxquz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2xzwtljjo.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2hrcpcyrm.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2sttsqmsd.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2tcieuisz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pachwqeu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lbroljle.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2iemqgcky.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wievtkxh.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qgzukmzk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xfzrumxk.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cnrhrkgi.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2eqezvkls.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2kmimckyf.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ngdmksqs.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2shkopxev.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ecnyrkwc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ynhqhrlv.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2keifyqye.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2oqwfwpnn.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2zoqqjttv.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2ptnwfwbr.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2gqxxrqvg.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2drevjyua.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2qyybzzle.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2gaolidxm.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2xzzfnaln.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2ecowgwqy.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2jyayaxlq.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2yzybhqih.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2stnfzjpu.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2lluuaasz.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2sqktuken.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2lkeldgse.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2tltfvvmf.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2mcsvzrel.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2djphttkg.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2xomlhwht.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2tmbibttv.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2mjnwpjap.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2inznjxum.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2qcfklary.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gieeygxi.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2zsrkucsn.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hkyfyczk.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jhxicawi.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wkgfdjgy.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ldordjtr.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2hekixcgo.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2oyuvcgxo.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lqmgnoea.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2wlsqqvth.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2yfyynqsk.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ririhlkk.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2vramnham.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2istknkdz.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nwxocxlk.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2jnglcrjl.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2wktuiqhv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2uuemzsjd.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2kuvxihft.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2sepwpkyj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2pdfyabqu.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2agwfibop.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xrzponth.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2rtkenhiu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2wafskroc.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2cofayoyu.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2ttegkman.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2nxysjuer.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2cgjsivyz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2zgjhxilu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2dnpqsgpz.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ksazxrme.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2ybxpmlbd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2lwfgkdpk.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mgnumzze.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2kmwtpdue.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nlilhdwi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2leekedtw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qfutrufc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nsiofhfg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2odbqftlk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2btvrmyxh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2wypckteu.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2ltrrpzjc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2qzglmmau.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2yhksjqae.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2qnqoqngt.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2wgugcjbw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2fmcmnlan.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2vchrxydm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ovbmtvtp.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2hpskucwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lbqzlziw.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2pfcxbhpt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gzmndmqt.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2jqnpqzol.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2brkzidwj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqiedoul.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2tbcnzqma.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pfblnmfb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dmjmuekr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2dnuumkie.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2muaoarau.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nacwtuvh.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2wliqwmrc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2mttxqoes.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2jlnreggz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2miqhgafl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ahuoghrp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2uaavefnr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2zlsuxccu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2kfvyajmi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2poldodyn.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2gzupgggi.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2cejalzjx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2twcebafb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2twxykrax.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ikbawwbh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2egrynaba.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2vczozbfu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2icxegajt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2qeurrpfh.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2cisnfwwn.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2khhvltmx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2haqwkfar.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2djkaxtka.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2gpwildtr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qpfqdmyj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2tmctknhu.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2vhbfxhsi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2uadygosj.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2stgjzbfo.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2duvaveyy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ezscubkj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2hnkrhayx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2bygmrkrd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gdqlpfrx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2kspyitmd.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2eisrfjky.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2tjjqiolt.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2vxpfvoek.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2oqrmfaww.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdaprirf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2eupxmlxw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2mhigvsks.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2cqpntxom.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2oblvvvsh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2jupowerx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2nkctpmgo.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2chppllca.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2qlubrbzb.html


<!-- 参考信息 -->