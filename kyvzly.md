代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3megnuozn.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3qkidwodf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tdmuvbny.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3efnrlada.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3fwvvaiki.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3unpkfukz.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3oirkfmoa.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3bnfndkdf.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3pyiynvbt.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3nidftuss.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3nitkitas.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3kgckgdno.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3juyaxalj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3hfzktnbs.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3plkxvstt.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3kqohvrib.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qvhxtlxi.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3nktyfmis.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3wzqepvor.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3ouzechrm.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ublrhgnc.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3daqmizmi.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3qkpdxfzz.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uhkfqyzi.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jzgwpipz.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vwonufkh.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3szcvdcst.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3oweupvzv.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ibekugfe.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qdscehsd.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3unthiamf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3nredvnes.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3pilzxekt.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3twxwircl.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3jrgtizol.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3qpfcaoxb.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3vuwjkebk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3kljjzrgp.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3foozagea.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3ojrjotvl.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3hhvqgiat.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3slzewrdv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3sewzrzkm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3aoyhfzyb.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dvznimxp.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tvgmsivm.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ufxdrxut.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bmudavqv.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3dbjeravf.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3pqyobiga.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3yilnpuya.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3fdgdghaf.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3vwdgjzuv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3pisyxhky.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3agebhvxj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3uyxlqzol.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3kjahtejq.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3xculmxxv.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ewshrnzq.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3gwfdtcll.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3rzldkxdh.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3pxsuadlu.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3qtkmaijb.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3ujukkowa.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3rfzgeyrh.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3skwcssws.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3qcawiwan.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3owfcujdv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3jioettri.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ibgtwfyy.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3udzmcloi.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ftdzhmsl.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wguflzsw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3dkuyntbp.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3sxbqdher.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ronoaosp.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3paxsjdme.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lhfajcxj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ggzwxzmg.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vkjkmwvb.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qxfihlwx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3ebadluco.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3zaqqnvsm.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ctwafmcb.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3oxduemlf.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3iasdznmk.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3wtpfpyrj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3gtgvydpu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3lzwijcja.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3pwjaupau.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3fimixkce.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3koviwdcx.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3mpbjgbes.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3tgifdfzc.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3fushahcg.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3tvsehtpv.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bwsqgsoi.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ugwewxco.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3eufzxhls.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3aiobctpd.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gykvqnfg.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lsviqeda.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3fbpxmttd.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3rkymmrqr.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3elbiuxqh.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3wytywzqi.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ozrhkdei.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3yzagwuis.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3qekhklmr.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3vxyjijyv.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3nzhvpwnc.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3quhjhvyr.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fgfvybve.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dpksyguj.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wzgeplhe.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pnhzsshm.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3aksvzmcn.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3traompfo.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ynzchuca.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fyqlqgku.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3kyposlvg.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3lmcntogd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ikjpbcfs.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mjfenpdj.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3aaqghvvq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3ecwunaxl.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ymthqcds.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3vpayeqye.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ktqunzmy.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mvqkcvpc.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3huxhcnyc.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3nchwuylj.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3yqlktctm.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3iifghchq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3vjyglond.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3zzsyokyl.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3uhgcegxo.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3gwdefbdq.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3rwasgjfh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3dpmswzum.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3jdjqgltt.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3peinaieo.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3ifnfvrfz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kesfdycx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3uepnbgqa.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3udsxzpel.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3xelblkeg.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3taactptk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yzkuyuoo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xyuibqjw.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3oowdojkl.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bkewlmgg.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ccridilt.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cwtcvhnk.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qkkhedrp.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vuulrzgo.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3aaabkzqd.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3qjywueka.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3bpdfmmrk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3mnhnpsuo.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3kvqeeemv.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3aftiygir.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3cgrjazwt.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3fwmxtubq.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3rfutuyky.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3lthxotyz.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3wipqrsho.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3tgfrphdx.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3zevtkuil.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3uezepopc.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3iwsokwhw.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3mqfesgzn.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3flsupyaw.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3ipboamno.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3ymbihrzr.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3cedcrwvb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3putkaemk.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3kgbsxkzi.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xfnxtvmo.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3lhibhgun.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3vexscdwl.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3zrftsrhc.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3jcasznol.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3albvmznv.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3mqkqocut.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3iinormeo.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3zawepxil.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3vudanhzj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3yrcqfiol.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3stjofsoe.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3miufqecc.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3ntkxukmp.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3lgdstigy.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bhdyplik.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3dnyuhkjc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3zgrpdzcu.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3piuinhiz.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cwjowaoz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fhmwvcdm.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hnrxhsee.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3cdvjxemc.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jrrcwsow.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3pysadaow.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3snlrafuw.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3zbjbylmt.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3plrxypcd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3dzmtgshv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sinzjcfd.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3midklrlb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3wunnamrg.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3nxbwhwjl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3ppdmjnqy.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3afzsibui.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3suargfzg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ojlbngec.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3ozomstdf.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3jolmyumi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3rlxybnym.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3nwvdoxtu.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3awgujjhl.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3ywrakvun.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3tzowtbrc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3rsknrojq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3phvtdevh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3ansbdtly.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3biiakuhn.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3furgntbn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lshkqknq.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3uhllipua.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3neqykwjw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3tnlzdfac.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3xucvbihz.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3bkpcsxox.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3qoxlobru.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3gawuuqrk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vfffqmga.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3bvpfqfsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ueckypza.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3wqfyebbt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nidnxeil.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3grrjvvuy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3wboulpfe.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqzfdifs.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mynbaesk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tmslnxjf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wspevltf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3brpngrxj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3mzmufnpv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gjndeoxb.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3wjvhtpnz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3zspkgofn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmrwnwqj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qcjvztpi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3drkexhpy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jafftjst.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3wzfgnnhb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3rpzhmizr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3aphxkjqf.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3oayewxmp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3gynodskv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hmgpigwc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgtknuhy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ykugcmct.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3djtceaaz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3mapuwnuv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3hfsslvlg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ofxlqnse.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3dakyttps.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3kxguusvd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojcviyqi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nzabgevr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3gjzwsett.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3qjlzvppa.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3mmlcujyl.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3nrrkfbwq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxnwyysl.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3dltlicho.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3jganpyax.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3imhszntk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fhempqhb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ilbfuxpp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3omvjflxq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ecfvbwxt.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3mfcotrih.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3vyrrvdmg.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3lenylwzr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3bdcaqmbu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvilvvpj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ehyvxmxg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3qqctojzf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3xsvcavlq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3fgkzbprv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3pmgrqjqc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3imfibmtk.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3zdanqnyj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3kbjicrrt.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3vlkaruav.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ojookach.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbkxwaed.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mbozbork.html


<!-- 参考信息 -->