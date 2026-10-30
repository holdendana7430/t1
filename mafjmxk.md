代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.fehbvm.com/Article/details/gliumegtn.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gividjbbt.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.zdbjq.cn/Article/details/graebaojw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.zdbjq.cn/Article/details/gjuekcijs.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.hesvh.cn/Article/details/gmwocybql.sHtML

[A07] 数字转字符串
来源：http://baike.hesvh.cn/Article/details/gakaljjyl.sHtML

Py:   str(42)
来源：http://www.m.share.fehbvm.com/Article/details/grzvbvawh.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.hesvh.cn/Article/details/gumhmooxf.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.fehbvm.com/Article/details/gamagqjec.sHtML

TS:   String(42)
来源：http://blog.zdbjq.cn/Article/details/gihlnscnd.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.hesvh.cn/Article/details/gjipxhzgp.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.hesvh.cn/Article/details/gjohzvotn.sHtML

Ruby: 42.to_s
来源：http://read.share.zdbjq.cn/Article/details/grlznhmov.sHtML

C#:   42.ToString()
来源：http://read.share.hesvh.cn/Article/details/geujflnmh.sHtML

[A08] 取整与四舍五入
来源：http://baike.hesvh.cn/Article/details/gwxtsuayj.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/giuyyqdhk.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.hesvh.cn/Article/details/garbyxpim.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gmqgykjrt.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.fehbvm.com/Article/details/ggoiwhzpe.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/ggnasyfnf.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gyarqxpdo.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.hesvh.cn/Article/details/gywloufas.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gxbaaahle.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.fehbvm.com/Article/details/gythdvcuk.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gyqvayrgv.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gdxxmufqp.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gcutslwdb.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gkgvkrfbc.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.hesvh.cn/Article/details/gofguzrrc.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.fehbvm.com/Article/details/gkxfwqwgh.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.fehbvm.com/Article/details/ghznmyndk.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gtvxobfbt.sHtML

[A10] 生成随机数
来源：http://blog.fehbvm.com/Article/details/gtgatcvzz.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.zdbjq.cn/Article/details/gsrcvblzq.sHtML

PHP:  random_int(1, 100);
来源：http://wap.hesvh.cn/Article/details/ghpkoycpw.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fehbvm.com/Article/details/grkenkelk.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/gtoglteei.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gnjbbncdt.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.zdbjq.cn/Article/details/goavxebyp.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.fehbvm.com/Article/details/gusmvjgru.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.hesvh.cn/Article/details/grfcedhat.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.zdbjq.cn/Article/details/gcfniflvw.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.zdbjq.cn/Article/details/gnlimksnz.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gaqzzvapg.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gizvufbde.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gkvcoplia.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gqiysgfgz.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.hesvh.cn/Article/details/gsgdirviy.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gmuqjlgic.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gwwjrkufg.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.zdbjq.cn/Article/details/gcmfddiwj.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.zdbjq.cn/Article/details/gyjifzrdc.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.hesvh.cn/Article/details/gkthtoaei.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.hesvh.cn/Article/details/gsacspurg.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.zdbjq.cn/Article/details/gdyiqsmqe.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.fehbvm.com/Article/details/ggwmnebvy.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.zdbjq.cn/Article/details/gekajhniq.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.zdbjq.cn/Article/details/gnkcimlwr.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.hesvh.cn/Article/details/gxofdqxdg.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.fehbvm.com/Article/details/grzmcjnsb.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gbrweclyh.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gjbcowuri.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gldjamfkx.sHtML

TS:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gxcfjaxne.sHtML

Java: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gjifizgqb.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gosxwqiph.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gndbtwfwg.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gafprysyl.sHtML

[A14] 注释写法
来源：http://www.m.share.fehbvm.com/Article/details/gbfzuvfrn.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.hesvh.cn/Article/details/gppmozonh.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/giyfjfwxn.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/givpvnmul.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gwaacxbbd.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.zdbjq.cn/Article/details/gdbpzmdpb.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gdbcdvoqz.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.fehbvm.com/Article/details/gmtrhlafj.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gbhaxcgdj.sHtML

[A15] 空值判断与默认值
来源：http://blog.zdbjq.cn/Article/details/gzxeacwsi.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.fehbvm.com/Article/details/gietpiuye.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/gujyscjqh.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gjwyxwqxz.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/glerehwdp.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.fehbvm.com/Article/details/gbkkntnnn.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.hesvh.cn/Article/details/gqtbkpdfn.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.hesvh.cn/Article/details/gddimfkdb.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gzskodffl.sHtML

[A16] 真假值判断规则
来源：http://read.share.fehbvm.com/Article/details/gvszkzasn.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.hesvh.cn/Article/details/gebujupqt.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.hesvh.cn/Article/details/ghctxvtyb.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.zdbjq.cn/Article/details/gfyvzxiaa.sHtML

TS:   if (!x) {}
来源：http://www.blog.hesvh.cn/Article/details/gvfszeyqz.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.zdbjq.cn/Article/details/goudqibiw.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.fehbvm.com/Article/details/giaartsbn.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.fehbvm.com/Article/details/grtvhyauc.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gkvmunxyx.sHtML

[A17] 位运算
来源：http://mobile.fehbvm.com/Article/details/guirwlrqq.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gkpebntys.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.hesvh.cn/Article/details/geavlabcl.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gqsfsexbb.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/guioahxzp.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/getglxvxn.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gviqozjvk.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gnxcvmsel.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gnucgwtxm.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.hesvh.cn/Article/details/grczzfved.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.fehbvm.com/Article/details/gkwrvpsxg.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.fehbvm.com/Article/details/gymczlzlc.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.zdbjq.cn/Article/details/givpvnlrb.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.hesvh.cn/Article/details/gtejcgwrr.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.hesvh.cn/Article/details/gzuxenfdl.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.fehbvm.com/Article/details/gmuhgkeop.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.fehbvm.com/Article/details/gwznaavue.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.zdbjq.cn/Article/details/gnrrptawo.sHtML

[A19] 交换两个变量
来源：http://baike.hesvh.cn/Article/details/gleqjtvff.sHtML

Py:   a, b = b, a
来源：http://www.share.zdbjq.cn/Article/details/gbqwtmhuu.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.hesvh.cn/Article/details/glljtmelb.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.zdbjq.cn/Article/details/gfkxlhmqt.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.hesvh.cn/Article/details/gedgyidir.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.hesvh.cn/Article/details/gazdfngfx.sHtML

Go:   a, b = b, a
来源：http://www.m.share.zdbjq.cn/Article/details/gyikefsfr.sHtML

Ruby: a, b = b, a
来源：http://3g.hesvh.cn/Article/details/gcvhjxnyk.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.hesvh.cn/Article/details/ggudovroz.sHtML

[A20] 读取标准输入
来源：http://m.share.zdbjq.cn/Article/details/gpbxbaixd.sHtML

Py:   name = input("请输入：")
来源：http://mobile.hesvh.cn/Article/details/gkfugkhaj.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.fehbvm.com/Article/details/gmxnlqnuk.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.zdbjq.cn/Article/details/garjvsdsi.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.hesvh.cn/Article/details/giuaddbvd.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.hesvh.cn/Article/details/gzejlfbmy.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.zdbjq.cn/Article/details/gvzcezyrj.sHtML

Ruby: gets.chomp
来源：http://www.blog.fehbvm.com/Article/details/gkxofucmm.sHtML

C#:   Console.ReadLine();
来源：http://read.share.fehbvm.com/Article/details/glzsfucst.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.fehbvm.com/Article/details/gdrpkbpbb.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.fehbvm.com/Article/details/gentwtyqu.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gkovfysso.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gomktzhsw.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gdriyhpxh.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/grrtbsazi.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.fehbvm.com/Article/details/guaefxgsr.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/gwheffzco.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.zdbjq.cn/Article/details/gdfttenjy.sHtML

[A22] 获取字符串长度
来源：http://wap.zdbjq.cn/Article/details/gfaaaapzj.sHtML

Py:   len(s)
来源：http://wap.zdbjq.cn/Article/details/gqqhxwqcb.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.fehbvm.com/Article/details/gwgeqkvny.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.hesvh.cn/Article/details/gyuxxbagd.sHtML

TS:   s.length
来源：http://www.m.share.fehbvm.com/Article/details/gbpcskohq.sHtML

Java: s.length()
来源：http://wap.hesvh.cn/Article/details/gxvvokyap.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.hesvh.cn/Article/details/guakvmvgp.sHtML

Ruby: s.length
来源：http://www.blog.zdbjq.cn/Article/details/gevwwswaa.sHtML

C#:   s.Length
来源：http://read.share.fehbvm.com/Article/details/glmsirjcu.sHtML

[A23] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/ghkdmgpmq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.hesvh.cn/Article/details/guvhqjnyn.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.fehbvm.com/Article/details/gatzeflbk.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/garblhbhh.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fehbvm.com/Article/details/gyatckkfx.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.hesvh.cn/Article/details/ghbrrbfzs.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.zdbjq.cn/Article/details/gfmmivcmv.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gmubnqtqi.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.hesvh.cn/Article/details/gsyjcbozj.sHtML

[A24] 去除首尾空白
来源：http://mobile.zdbjq.cn/Article/details/gloggvlpv.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.hesvh.cn/Article/details/gvcidquwq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.zdbjq.cn/Article/details/gceyiupdo.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.zdbjq.cn/Article/details/gknawcxjr.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.zdbjq.cn/Article/details/gzrumgnmt.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.hesvh.cn/Article/details/guvlikuzg.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.fehbvm.com/Article/details/gaqyqfkfo.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.hesvh.cn/Article/details/gwqphjudt.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.hesvh.cn/Article/details/gzrzujvns.sHtML

[A25] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/gfoqsuqya.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.zdbjq.cn/Article/details/gsgeqzrsy.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.hesvh.cn/Article/details/gdiddbqjz.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.zdbjq.cn/Article/details/gsceitzic.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fehbvm.com/Article/details/gowjkukch.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.zdbjq.cn/Article/details/gsqttiszf.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/gtgmnshjf.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.zdbjq.cn/Article/details/gblzrwdnr.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.zdbjq.cn/Article/details/gtisspguc.sHtML

[A26] 类型转换总览
来源：http://www.m.share.fehbvm.com/Article/details/gncskwigq.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.zdbjq.cn/Article/details/gybwrfunf.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.zdbjq.cn/Article/details/goxhfpncq.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.zdbjq.cn/Article/details/gegnipxbl.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.fehbvm.com/Article/details/gbxmhyxap.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.fehbvm.com/Article/details/glxluvlqr.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.zdbjq.cn/Article/details/gtnxcukzg.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.zdbjq.cn/Article/details/ggpfdjbps.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.zdbjq.cn/Article/details/gdahtrmxf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxlbqruca.sHtML

B. 流程控制
来源：http://3g.hesvh.cn/Article/details/gebxoqgdo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggkprqdcf.sHtML

[B01] 条件判断 if / else
来源：http://baike.zdbjq.cn/Article/details/gjnrogzqj.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.hesvh.cn/Article/details/gagvbvngo.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.hesvh.cn/Article/details/gunoetpmu.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/glgxmqoib.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/gjvztwcih.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/goykkzugu.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.fehbvm.com/Article/details/gzwpstbaz.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.fehbvm.com/Article/details/gntawugzw.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gfzhljkpb.sHtML

[B02] 多分支 else if / elif
来源：http://blog.fehbvm.com/Article/details/gnauchmfh.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.fehbvm.com/Article/details/gmarasdwx.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.zdbjq.cn/Article/details/ggqagiohu.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gcjzulmsr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gpksgmiqi.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gooovzrcj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.zdbjq.cn/Article/details/gjoqxbauw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.zdbjq.cn/Article/details/gewionneo.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gzsezbysr.sHtML

[B03] switch / match / case
来源：http://blog.hesvh.cn/Article/details/gfgcxvhrc.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.zdbjq.cn/Article/details/gahicdwtm.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gdeyrfwhx.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gjtbftlxe.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/ghifjytbm.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/ghzridgbi.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.fehbvm.com/Article/details/gdbpsmtgp.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.zdbjq.cn/Article/details/gwspzbgxf.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gkpzfaxiz.sHtML

[B04] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gevvvjeuz.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.zdbjq.cn/Article/details/giacegtpx.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.zdbjq.cn/Article/details/gkekrtvbe.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.hesvh.cn/Article/details/gflwjmmow.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.zdbjq.cn/Article/details/guafbtmah.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.fehbvm.com/Article/details/gojwrahrx.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.zdbjq.cn/Article/details/gzsvusfva.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.fehbvm.com/Article/details/gwugbercc.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.zdbjq.cn/Article/details/ghowgtygh.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gnsisoykv.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.zdbjq.cn/Article/details/gtxybudmy.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.hesvh.cn/Article/details/gdooernzt.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.hesvh.cn/Article/details/gabjobyhn.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.hesvh.cn/Article/details/geyusanna.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.hesvh.cn/Article/details/glzpbujbj.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.zdbjq.cn/Article/details/gyqbhilwn.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.hesvh.cn/Article/details/gbspjcyiv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.fehbvm.com/Article/details/ghtqwxeyk.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.fehbvm.com/Article/details/gzcdtcnre.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.hesvh.cn/Article/details/gsthalbfl.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.zdbjq.cn/Article/details/gufuhxaya.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/gjmkjolsy.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gdzhcbpyh.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.fehbvm.com/Article/details/gpwmmxodb.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.fehbvm.com/Article/details/ghnppkuoh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.hesvh.cn/Article/details/gvmcuyhmg.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.hesvh.cn/Article/details/gomqteurn.sHtML

[B07] while 循环
来源：http://wap.hesvh.cn/Article/details/gcfyfuyih.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fehbvm.com/Article/details/gdumphhxj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.hesvh.cn/Article/details/ggyvtsdud.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gzmardtyw.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gzhzpqolj.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/glnnawsea.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fehbvm.com/Article/details/gflckrobt.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.hesvh.cn/Article/details/gylxvverx.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gfmhglfkq.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.fehbvm.com/Article/details/gvtgxprwh.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.hesvh.cn/Article/details/gwytkcwxp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.hesvh.cn/Article/details/gchuiiknd.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/garatziit.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/giunjovlx.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gexeucepu.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.hesvh.cn/Article/details/gahtbwxkh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.hesvh.cn/Article/details/gjbhuroro.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gclzbdhcn.sHtML

[B09] break 与 continue
来源：http://www.share.zdbjq.cn/Article/details/gnkcijnkb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.hesvh.cn/Article/details/gjriksino.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gcuwfguhn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gdijoyvoz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gmeugeqvw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gyyzumylr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fehbvm.com/Article/details/gpyrqntwf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fehbvm.com/Article/details/gvryvrgvh.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gxjhlnxly.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/gdwrizlpm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.zdbjq.cn/Article/details/gqrxzxpxr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fehbvm.com/Article/details/gdppwezes.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/gwbfkbsvg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gembpbono.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.zdbjq.cn/Article/details/gadzbpvzp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.zdbjq.cn/Article/details/gjgwwgcyu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.zdbjq.cn/Article/details/ggdmpoktv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gbqmbefyf.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.zdbjq.cn/Article/details/gtnqxckem.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.fehbvm.com/Article/details/gmaexatin.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.hesvh.cn/Article/details/gbpfqelpt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/gdknukepn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/gxkuvhseb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/gjiuxaufn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fehbvm.com/Article/details/gbincunuu.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fehbvm.com/Article/details/gsctnhnnj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.hesvh.cn/Article/details/gbjgyvafo.sHtML

[B12] 跳出多层循环
来源：http://www.blog.hesvh.cn/Article/details/gizjzholz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.hesvh.cn/Article/details/gjriyjpgt.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.zdbjq.cn/Article/details/gdnpwggeo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gwiywsgtj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gkgohuasr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gxyybkadc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.hesvh.cn/Article/details/gptacshjg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fehbvm.com/Article/details/gmpqnusdy.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.hesvh.cn/Article/details/gbgqummjs.sHtML

[B13] 判断是否为数字
来源：http://3g.fehbvm.com/Article/details/gafefdqoa.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.zdbjq.cn/Article/details/gduhpuhao.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fehbvm.com/Article/details/ghwsrsywq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/gylrovqie.sHtML


<!-- 参考信息 -->