代发 wailian999

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3tpbzkzam.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3uiuyrvqc.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3gqnefgch.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fusjrtjs.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3qbwgxaaf.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ynxvvutl.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3wqjwodti.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3mzytvott.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3mclavjgk.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3flhiqxno.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3qlipvgwy.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tklhmkjv.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pvbilpty.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3neuqkvce.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jkbinaat.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ufabcezy.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3zukgmqzi.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qdyvutob.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3kmeiwpkm.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3bnxmycfq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3qisxpzqv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3htkbzucq.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3mvkrteiq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3ewuntmky.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3dwvutlrs.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3yjualcvs.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ospdbodo.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3iavbjsqo.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3eaxjqzkv.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vyyfcebp.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ozeypigf.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vddfipip.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ptsrvtgw.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ghcpmymw.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3llrsqynj.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ydnijjtx.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ljzczskt.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3dxwblngu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3jdeweteu.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3pgfpfijz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3nmnwuraq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3qaqkhxxn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3dtioomtr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3lklfpncg.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ghtewldf.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rnnlzrvc.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3xxwvovma.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3htnifhji.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3yrjppgkc.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3uvkcdoqs.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3dbuzkfsj.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rgogdqmc.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3gzpglgay.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3pzumhsvj.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3cviounpl.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zjkhqnzv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3pdvhsqdu.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3rfhtpsxs.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3ahitleic.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3pyjliead.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3rfalslfm.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3kbluvvcp.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3rkjuggdz.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3zkdpgbhw.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xnrgekzs.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dgvnzlor.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3yhhiwkso.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3askajbkb.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jgitxtpg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3ofmmpjwr.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3ufceszjb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jzbyyjxu.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3xgtsdyjq.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3udcixcjn.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3pezljdjh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3xijlnbat.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3zfygaaei.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ioppharn.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3qengvhfv.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3wcmcinfm.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3lpbyqnpv.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3ymbgufao.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tplqlvyu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3olwrkali.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ybsuytnj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ocbkihms.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3tdxyhhsp.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3tpxnfmcr.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zxoadbbf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3szjcbviz.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qxwpjobn.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3puvqlwdx.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3mnpswpea.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3rxzaxsgu.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3kkpqalan.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ofqckclj.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3sybsxxpv.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3fywkjeps.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3grcaexoj.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3iwsnqdjx.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dsprboem.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rlwyhmnl.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bwbalvsu.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ifjddffa.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vsdczhgn.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dxstwxjg.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jfzkvkje.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dwcdutcj.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3kahitbwl.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3emzickjw.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yzxynnig.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kysnuyru.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ppirrevs.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3zaibimbx.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hwhgkukb.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3smuoifwv.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3lciyyvis.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3bbwzavxl.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3tzmumdqh.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3agrbjvzl.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3detlvktb.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fcobankj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3jmfourvs.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3wrlpufoe.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3wqdauqmg.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3dtwwecob.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3ynzqezkw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3trftxcje.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3gdbcugog.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3rqetzfhe.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3akpenxaz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3uvvfryyh.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3pvmhkpsa.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ulluccjv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yahbfzhe.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3muieihph.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3eitqkkcr.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3uhlarpse.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qqkkjmnk.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vxonykic.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ailsptoq.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3faecznnf.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cdcwhaau.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ohzvkwac.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3cvixwpir.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3oovxsatt.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ocdnengh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3qzrtesni.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3yeuvrqcu.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3qtppumfs.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3gxplqgem.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3ljtrgquy.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3jtivtoee.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3wpanyeub.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3fljmkvin.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3inhfjnuh.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3hbixtytz.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3qcyariua.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3qavtphnm.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3keqpodrt.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3vwtsizej.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3ligajpmd.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3kytrcxsh.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3fyaolbwi.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3glcamkmx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3pecotefx.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3lynaqhtg.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3ulclnmkg.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3jbthyjpb.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3xdqwaerx.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3dohkzcrc.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3gqlqyjet.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3gcpvlprj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kbfgbuxl.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dutglzxu.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vvznrscz.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ndhenciv.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gjvdoasc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fcphwrsq.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3nudbkggd.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3cdpgpubn.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bmxcnkto.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3amllkxze.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3sjrtcnaj.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3swkkkftr.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rlvitmdy.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3vodhdagw.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3tuzbfsbw.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hxvxxviv.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3tjqpwiot.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3pzrfdkxj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3tosgmqwt.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ivuimrup.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3bbjfuzdl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3tzpitixu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3cykogmnm.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3bubjsten.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3avgwmjsj.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3zzfieqyn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3yvykvape.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3izeajxgd.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3rihaknih.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3nuffpkek.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3xfposolc.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3mcnnzgik.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3qfulwcxd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3vfgijukt.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vxvvxhev.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3wqjtvzmk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lvoimfds.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3aqxykbaw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mtjqhzad.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3alnvtiqu.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tmvxomvt.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3jxbbucmh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tbutegdk.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3eqsxpjff.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3britthkp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3vnlymlci.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3knddnlvw.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3ufarjwms.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3zkijsdzf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3ramxjutw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3oizijfvl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3iiuyrxko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbzbpukl.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3louwpgvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xccetjbv.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3oesxgsvs.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3mjufqatk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygmnjyjg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3orcvlhtj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ctfblhwu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ojvwhgdl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3vpcvegui.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3vwnzbrfa.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ovgbuaay.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3vdjmtneg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3gvcmnuxd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzlytijd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3aeeyueok.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vpwalspc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ihmdfiof.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3huqpgjxx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ugqzenyg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3csxlevvj.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ecywlwkb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3pavxxwgq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3uulwfdav.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvyqdyso.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zlwxfmdu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3btbwwgwd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3yxzuwhfk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3hdevesgu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3nouellih.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ltcwzgig.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3dlixszgj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ervhhkqz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3rkajifxm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bsxvvtpf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3emssezxy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3mypchpcc.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3bxlmrrrn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3nwbgsjic.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3vdfbsaue.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3mxtrfgpe.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkzbavud.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jdcjueaa.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3twmfplej.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3criskkyd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3elvvddbq.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3aekughiv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3mfcxoydy.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3rnfdgkex.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3mvgsxqxr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3xzuxpzuy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3wiibtyrf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ufhbqqfq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3zbzfcdkf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3zfjdoedb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3cppsvdrd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ewkdtqtz.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3prkcsoln.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3rpvuaphl.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3bemdlist.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhszgiba.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vtaxhajg.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3igdcqavg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3ebnvzuvz.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3lawkeduj.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xegrnywj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3cruuetlt.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3kcwqqnyv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bleohgug.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ptgdkwli.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3arjpbzib.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3syasxesh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3rbbhsvfq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3eeuyyqni.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xnyxfkpa.html


<!-- 参考信息 -->