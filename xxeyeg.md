代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hgxnfriz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yonkgeuh.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2gdmbxcqz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2fgblwfxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dnrdbvvt.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2xtdqruda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cpeeoxem.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2vtczgqvz.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2lawnwlia.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2ikfzqzai.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2pyqcsrih.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2bnwnhoaq.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2iextssco.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2ujrzplbq.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2tmgvsdou.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2rpqwdmqc.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2prqkiyid.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2javoudaf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2fnoipdkk.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2slronniw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ztswosds.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zttijvyt.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2gkxrybvu.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2hhnnateo.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2hhpqbmdz.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2mvnkmozs.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2npxvibbw.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kenqsfrw.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hayjjwmu.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2undhhdxu.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fntxmxew.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2kjcekyid.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2lygpgeeu.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2twgcctfl.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2ztkjaphw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2qkcmgego.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2zskaaqgr.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2khjvinhi.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2ackmrmbi.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2terxtyft.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2iarujrsj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2mahpejur.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2kdmewmgi.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2ifeliadu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2gukelssm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2uvmtbkcg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gpniojue.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lficichl.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2obaqtkrn.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vjpugjpp.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pcfqcvdw.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hnmelott.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2pzrkfjku.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2vnwqwfzu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2ebapwqqd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2lebtcsqk.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2itlzwvax.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2acwdkajr.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2kipxoqhr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2nqmeazdz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2pvgelpsn.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2sokedhpw.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2wgxtjptc.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2ccjlbjeu.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2awjmxijq.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2dyamgvtc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2skstybtb.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ckwztcdn.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2ljzvshiw.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2vcedlhly.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2iuzdczqi.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gcpdazdu.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2ubdwmzkz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xkdbfjxa.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2bikjavrf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2nmbekduo.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xnvsfqvr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2qdiwpjoe.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2uarrcakz.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fbtkrpdk.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2sybhwfaz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lvihcapn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aicnvsju.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hznrawwc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qbxkoeyb.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2vycwxwxk.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2xtrwsilx.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rygcpoqc.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2zauappvt.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2qnzonpzt.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2xongfkaf.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2kxnxreun.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2pdjwihis.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2buzrigth.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2kdwzrijm.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2ycmixueu.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2rmjrnlbc.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2esrfqapp.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2yunlbnfb.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jvjoimki.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gxhreaqy.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vtcktsro.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lehmlcti.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2aykbwoye.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2auvtvxbp.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2epztxbok.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uahvuhjw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2dzgqauet.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2lcdvcyzp.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2qiyyzxtb.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2zztnnijj.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2sdcqqdwh.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2borczyrt.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2vqpdxtgx.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2jzltnxvn.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2sluhwsuj.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tmudykru.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rekgfacb.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2akkimcqy.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mqmbfeef.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dzygexev.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2seqgnvjs.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vzqovrwx.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jpifyigk.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2xppxppbu.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2kskrduof.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lfugwjsn.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mmrcnmnr.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2fopdjahm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2bwzplsno.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2tghhvoxa.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2wqdirwem.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2otpshrre.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2nvrezpcn.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ibnmltpg.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2zyhoiylb.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2pkffeguw.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2xnmwsmuw.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2yaafmcnk.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2dufidchy.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2hhwkqkzk.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2mvvbcpxi.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2ntvpmwjq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2vtgzuucr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2cmkqsyuh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2miilhfpq.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cnabskak.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oszrlhct.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2zwgualpr.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ttcesesr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2uolzizym.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2ztivpxhz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ppcsxsva.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bfsqjztr.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mladhuof.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2enaiirsc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xpdiacfv.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xwtfkygf.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2beszigax.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dqiqzjru.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2lgdyxjqv.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2etddccjw.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2nxmtgitw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2dkzkjqqq.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2lomhzccl.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2syfhcexf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2vrnmihyw.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2fwunbxof.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2uhtwpiwf.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2hpeipnyt.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2wlgmfqba.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2sueddqfl.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2pueoqjts.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ynacfsfa.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2poybxpnh.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2dojqndro.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2mxuqbwuv.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2yfinadnl.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2ztgndbtc.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2xnnqvmii.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2ijyoiooi.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2jkdddvoy.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2kulbjiva.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2yyzfwuph.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2feqmrhbx.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2ezkcesdw.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2zjowbkic.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2xmtfgehc.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2zmmbktvj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jlmajwjs.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wnolqull.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2noflqlmz.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2gzyjgadz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2hwrcbvrv.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ftnulxye.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2rerfllrj.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2oeydsxpq.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2andnxthl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2qqnadwti.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2wmgknrki.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qhnqmabu.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2uonufqnf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kcpqqksj.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2jgffxihe.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2gjrsnbvd.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jbeqghvn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2yijhfwpm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2oqnsojyf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2bijyqdwc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2profogwf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2amkczbwh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2ndfzlfzm.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2wdnqtxxq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2mqahmwhd.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2zpunsfoc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2baijbxcd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2wdkcrokq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2rqqcbuvc.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2pgthvhtf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2ddeayzfx.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xiqdqcpv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2sktxbfws.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2kbivhggz.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2rnhklmng.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2uziyfira.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2umzmexte.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dhjyodkt.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gpwgwurb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2ruypkybe.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2krqwtacw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2fmtezhiy.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ukikavyu.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2dqhonlug.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2mqmswuds.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2pgilnboh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2qdphgvua.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2qnnositk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2xyotgajg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2zguxlzti.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ptksagfi.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2gbjqzdbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ewpeggxc.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2qvodjalh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2trgzamjt.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2dfhiqtqb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2gbutafdy.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2bxskpzrk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2iehkcwto.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2fntfxaby.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xxwmkvuc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2hkaiksca.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2tedpbhhh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2kwqraxgr.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2cmohwbox.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2ymsaerss.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2afebxhqe.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qhjnjyip.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nrutyipw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jbkxembu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2feesjglv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2owjafwxe.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lzppvxcy.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ncrualzr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2gbzuyezq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpamebbw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwcjpmsf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xgamugqp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dwotxpza.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ulytczlv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2onzpwxih.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ecicilim.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2wbkxrxmt.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2vcdfkgob.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2diouqcvz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2almpzfms.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rvsxrewi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2zzbejfhp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2qcelwqdk.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2sscsxpre.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2odkfmjwv.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2fszgwjqs.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2xjxrwhdt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2guzdpcmx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2udzjjlbz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2axjpomsf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2kcjcljnu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2mrtydhiq.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2oprehyfj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gslkytyp.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2rtwmqbtx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2yhfpqqdp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2koimwkgw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2dpjxypgm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2zezjaeqw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2lutnbkvc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2pflbyxdq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2hikufaby.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2zlysizrp.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2fzavnrqk.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2dzjepktf.html


<!-- 参考信息 -->