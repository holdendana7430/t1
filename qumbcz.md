代发 wailian999

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ozfgetmi.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3virtyful.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3hhphqrhj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3irwwalko.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3qjipekky.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3crybizua.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3eyayaugi.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3fwbkhyhi.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3kmmybuzv.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3sqsrpmik.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mufypcsx.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3coisoscy.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3wdglpkoe.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3fjvhpttt.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3ufeorgfc.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3aosewdbc.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ghjwmdvv.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3nhiupbfz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3zykwmjau.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ldpfglox.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rbofggwr.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ylutzjsi.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rtpkymlg.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3cleaedtk.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3jkmmxbxe.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cfqkcqvc.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3nblrrqiq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3zgahmbpa.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3vdxulfim.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3vcopzbyp.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3fenvwvxp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3dtsqwccf.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3fpfbnwlp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3cxrxvnwe.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3vvzsurik.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3uihohkfh.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3gtsqnhng.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ulysipde.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zkpjfkyl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ixogaaxj.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3twyzzdxg.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vfxpbjgz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yitejszk.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dnrpfzqi.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3dmipnzcu.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3mwolhupq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3apvjsplu.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3zuvjynli.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3jtgztcwk.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3dzqzhpgr.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3ucyjhzmi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3kbmqpuch.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3racgmkeb.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pzadkulq.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3yplujjht.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3fhyhajdl.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ovwzicrh.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3zyzgmgxq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3smuvnkem.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3yfaqyjxs.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3plebeliv.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3zgdwsshx.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3nnavqple.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3tzqgctgw.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3eadtfxpz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ynexcneb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3cxgwclpi.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3hrcgdvnu.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xrectgrv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3pvjugqwk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3obujtian.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3cyolobim.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3penvyqnd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mapfwahu.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jrdcarkn.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3piyjbhup.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vhpdnfds.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3jpicbcon.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3pniigzon.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pupzclnj.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3hxjqvpli.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3ypjrdcnq.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3laadicpz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ojdvjejz.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3xdoxwdfl.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3bjlikztu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3ltdwwgdk.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3slephlex.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3dindvfiz.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3nrsuwlng.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3rsamdpih.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mqrjluzm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3udyeozvr.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dmpwkdqe.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3eqdafypv.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3uukdnwgb.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kxmzrpnl.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vgqusnvv.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pwjvgfuk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3ytjlrbpw.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3ssfrcctf.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3hnwgrzxz.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3dbjpesqo.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3yjdqltit.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jtlyuods.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3edzwbgpm.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3gamhmanv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3vvptvmvd.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3njysbcxy.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tiknvsoy.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3duhyscqt.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ygqemhyc.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tsdgeyyu.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pjsazhgv.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3imqfeybt.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mxddbuad.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3ylrwzzjj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3wgfztaaz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3swytsyin.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rnluvtkx.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3owkrqicy.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3mbsmrjag.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3perzjotp.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3lprjjihs.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kpjieyjx.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3njujpyko.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3zcechcjj.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3nzzuwxie.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3wlfjhphz.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ysvzzzdt.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3eojdymun.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3oehuxlnd.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3wiyewhfq.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3btifpnfj.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3sprwsnmq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3dldxsrih.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3pcxgjikd.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ukavklxs.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3mpvnnobw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yxblihet.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3pwathdyq.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3wyvxxqpu.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sncicfcd.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3ujsmefmn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lnqfrtox.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nmgfxdsq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3orughvba.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3obdbboft.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ddhzrrgc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3grgkpfxl.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3trsohurn.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kpxaepwr.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3osottblh.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3chgdhbrk.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3lkqttumm.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3cfqmgfmx.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3dvxcxbul.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3ykqahfhj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3bwnlgjvo.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3zyrarusi.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3txsfljkz.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3rcvqollt.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3jbimbpkj.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3oacmgnet.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3twfmigld.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3yiojewvu.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3eoqgjwef.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3reyktkrw.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3fmlewiin.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3etimbkra.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3rbcampte.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3pnfqieio.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3urdzccby.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3ygzwmfgo.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3nnlqxylk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3slbkvgxy.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3joxsdyrc.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3ltkizmvd.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3mwbpjjxw.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3gsebbpin.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3fwqcahdj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3viqzwoir.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3soukphda.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ssiqudmg.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jfncymia.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3lryhqewn.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3geufhrtv.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3ybethlne.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3slavyqrk.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3pvuqvxvz.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3kpxjpwfc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3zwrxtuev.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3mnmufubq.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3vxbrhlzm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3kjkjlwwj.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ctivefim.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3vwawagif.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xtnisoqf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3dpioakza.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3arbbdcef.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3aytesfux.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3bxgfmzvq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3qpkxzfxh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3oyvtvgfk.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ptdepjyu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3uhwsjtai.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3ndiszaru.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3fhlnrkcl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3mnbnldck.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3farqvzqb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3tsnnrcsi.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3abeoauir.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3shxqprmb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3lhpcbqjn.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3imnqwybq.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3apfufzvw.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3grlvnvhs.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ldktrmuj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ludivgol.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3oydhmzff.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wfxmrrae.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rqyuztkw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3nihzhdmg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gdgnvfkv.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3titbeotr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3mvteqxow.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3rcbtouav.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3crnvhrgs.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3pmngtdzu.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3qjvachrf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3ipefparv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3ybcsfync.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3lwyspplk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ullwdivf.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3odnekxxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ouujhqrk.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3yjkivkeg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3pklcwdce.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3hstdtgvv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3sxlojvsh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3lziipmhk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xqiwkodn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3xrunogoz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3wrduynyp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3viwqryoh.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3cgcgaljs.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3hxgiunls.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3rjetkpma.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jpkujbbi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3uettghav.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pavucsht.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3ulngynmd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3dymfmghl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ihlihlda.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3uongaeny.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3fjznaanh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvetovdc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmktgqef.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lzibjwgk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbrbmemm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3msxjorgi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3qqunogvn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3fuxbzufc.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jzxysxfz.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vixkwdrb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3uoutgral.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3frwjecvu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3mdmzosjn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qjhprfwp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3jjrstxrw.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3yiwtjoxi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bsixkyum.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3hmmrxhkk.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ypcmycio.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3feqbyevz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pfzalrqg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3cyvwxhtn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3auchnkxn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3iimhnwxa.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3utwwcyyk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3sgondski.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3vlsdobvm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3vfsboloz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jopqsfzo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3fzmgihti.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ecliqirk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3damunius.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3plkfhenx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3mdyigwlg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3yfwgxrvk.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3pbscrkqa.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3knjbxdqj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3koghzbqh.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vvmiebmh.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bhdaquod.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ixdudzmy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3puwbjraa.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3sezohqhe.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbfvxqjo.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3mytwgmfk.html


<!-- 参考信息 -->