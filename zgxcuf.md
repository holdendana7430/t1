代发 wailian999

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3bbiadloc.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3pfkthzmm.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3noiahvqh.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3iszjfucg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3zychyisp.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3fqqfwnlr.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3wwhsafqt.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3jehknzyp.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3usxpqlgt.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3kkqxkuek.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vwabifay.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3axvlqqat.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3wpmyqcmz.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jwblrqcl.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3hhfmbsro.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3aglbhmrf.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3lziodels.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3vhfbfcqr.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3nunbfcce.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lchutaxs.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3xqmbtrvz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3yjflqkhv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3tydmkaif.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zaoabote.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jwhliula.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3idtqavcj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3modwnexh.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3dsvrbfpc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3szbkgwug.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gdgtprlu.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dtfwxkic.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zfvacvqh.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pdajrxpy.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3csgkhnfb.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3tyuopaxf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3shypqbit.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3fpxkdako.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3pkncatgk.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3eepsfhjt.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3bbhjrajb.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3agpalhhk.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3augmweee.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3hpkjnawr.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3cwzapbvo.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3bptjvrru.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3timhuxap.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3yxviufbr.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3aanpgysh.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3tvxayozi.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pdrxtalp.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3cuwuvujl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3lsoqaujf.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qwmciaij.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qhnnwxdz.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3jautkatn.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3tkcdoeao.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3uttqlgbf.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ashxmfpo.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ykvkehzb.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3tnbtofnw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3vrlabrrf.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3rgzvjntv.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3zrdmdlkp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3noxzerhq.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kwzvcfpp.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ajutbels.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ibkzedwr.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3enhgezsl.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vmjujeok.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3upjxyozw.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lcfpnsrz.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hforhgjk.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3mbotmwkj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3rftylnbh.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3crunuvsr.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3gfbmadlf.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3oicsnjon.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3rztruyjs.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3iiuzzovp.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3vqaouvfz.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xqipgkgl.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3bgzgpqcr.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3nkgaezdn.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xxuavfwe.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3mgkrdpcx.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hgbcbmxr.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3nmwtebto.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3vijsmiwc.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3krsdmpip.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rjklrpjb.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3njvyyhzj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3uvlkqirs.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3uahedkhm.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3jzqcrhfn.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3paeiytmj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lcvwxhxg.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3piztcezb.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3nyggxzrk.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3putnswii.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3taxdvcdj.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ejkiaail.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nufyujyn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nodedhpo.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ccummwch.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3utmwhwft.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mzgzhubj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hxntgvhy.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3opmpbftx.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3tgvedukq.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kkilwndn.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3fjsdobyc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3rjlplzyu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3lsthoojo.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3kkujepwx.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3lrgcljbh.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3mbrcfedg.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3kjqrrlcj.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3xnhxhvta.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3vruqqern.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3leckaqhs.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3kqywioxe.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3mmmmelqm.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3abnesdss.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3kdtndwbg.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3kpfndsme.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3sqvyufwg.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3mfgyjjrw.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3riujbasf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3ercqgfnn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3fngvilkq.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3qccjffnm.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3ykqghkkf.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3oylweljj.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3xzirlnne.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3nmkirulg.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3zqimuoqf.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3kjsgdhnv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3hdkrqitv.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3sjxgyetb.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3kcgbjtdu.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3bbcotmgo.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3zjelcyau.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3knwfneud.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3bfzrzfpx.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mbdnljzl.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mbbudxaz.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3tnseekou.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3lsayjnjc.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3xgsjzvom.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3vdoopepn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3uwzopmfb.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3nnxcplqe.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3pgjoylgp.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3tekuvmpy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3ycaxfvzq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3scdeveut.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ehdtdjjb.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3rnvlfsqv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3somtsidh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3excwxwzy.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3iwguadzc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3kmpcxbwq.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3xzxeirjb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3mtzvxced.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ijuqmkuz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3pujwzqsy.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ysvizvjs.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3nmpjaili.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3igsqpulk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3jkuzufpb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3vfkjsmcx.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3iytfbzdt.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3injsfgiw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zcbynvrd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ljrxaohm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kheybnou.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3aozvpzlr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3vkpufbge.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3sqhkjmzn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3yissepbf.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3sfqajcwq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3rdbxasdf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3hyeeikhb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3ivozfyap.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3viqitfxb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3plxaiphi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3onxavxvg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tuuwgegq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3sldlbhba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mlzeqioc.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3lbnzpasc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ucydtmlu.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3ozzeosgi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ktuwoboh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3mewdbznb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3wrlhyohg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kgdvchpg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qfubgmwr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3yqenyree.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3nwparmgr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vfhjfgqn.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3dgegebex.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ttxqjkrh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfsyxhmu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xfirtwef.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3iwkrnngo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wnttgooe.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3jasszwls.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3uzmxxbxc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3djwibcuj.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3neodejog.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3sgvlrsnl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3csqcnfxb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3stezljnh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3azaxifng.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bkjzptas.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ihggulsv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3wunopqek.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3fbmyugul.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3cyyiccqg.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qyjpwezp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3gfrleggz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ohsaytat.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3zmircqbl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3yczwoelm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3hwbogsld.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3njniwjpt.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3cveztbej.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3dguyolum.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3sltbszzm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjvtrbdr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vkzuxoad.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yygcyolg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3hjqcayte.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3ynxcxmtu.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3zvdyuzbw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ltqtsdmi.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3rycpcchj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3rthtloum.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ywkksmvl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3zbdxzzga.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3iukdxqmu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3tqpzxnpg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3qgwsxqfj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3lvyshycr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3bnikcvyi.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3czimtgkt.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3hwdrywyt.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ihurchav.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dunpcsnm.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpifervc.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3erzhrhai.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3wlqbirxw.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3hmrmjenw.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tprzwtti.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3dwykqznz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3lafmdoft.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vfyrashx.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3krgydgbg.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3akkwjadq.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yvvendes.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3wnnvfprw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3bogrnfhk.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3cmvvufvv.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3rkynflbs.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3hprkwnxn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xjgeqoqn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vthujkni.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqolyjih.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lllzxpwi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ftloauwv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3nvwbxtrh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3afregdbi.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3gtdgjqmw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3ehkwalsl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3lofuiwil.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3nlfvkrqh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3yjyhkhsb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3xapuydhb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3wstzkspg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3dwyllinw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3lvuranuf.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ljbqmlob.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3jvcuiqga.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fjrarhyt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pbowhewd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zrkfiwzi.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jeftorqe.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3tzvkqbnr.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3xsfiubhv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3wrtgjsbq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3wqzkwrkn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3fbgcixdo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3lpcqndtk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3pajcxevy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qtvkehon.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qsdcvdas.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3upolinos.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3norituay.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3eltqkgqb.html


<!-- 参考信息 -->