代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://blog.zdbjq.cn/Article/details/ghhrvyqnn.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fehbvm.com/Article/details/ghfbgaixr.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.zdbjq.cn/Article/details/gsnlfqdxc.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.zdbjq.cn/Article/details/gxxoqytum.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.fehbvm.com/Article/details/gfqxcspsc.sHtML

[A07] 数字转字符串
来源：http://m.share.zdbjq.cn/Article/details/gemmvkrux.sHtML

Py:   str(42)
来源：http://wap.zdbjq.cn/Article/details/gwihrxkjm.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.fehbvm.com/Article/details/galklodbd.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.zdbjq.cn/Article/details/grlfqmvox.sHtML

TS:   String(42)
来源：http://baike.fehbvm.com/Article/details/gaydlzkyi.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.zdbjq.cn/Article/details/ghhonmotb.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.hesvh.cn/Article/details/gqkgnmyyq.sHtML

Ruby: 42.to_s
来源：http://mobile.hesvh.cn/Article/details/gncnfkwcj.sHtML

C#:   42.ToString()
来源：http://m.share.zdbjq.cn/Article/details/ggvmarsbm.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.zdbjq.cn/Article/details/gitweggip.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gjlljtmnf.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.hesvh.cn/Article/details/gezysiwqh.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gysiigbtg.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.fehbvm.com/Article/details/gmdbzxrmh.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gzpaxmccq.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gmqydomob.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.zdbjq.cn/Article/details/giydoxoun.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gwvucjgks.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.fehbvm.com/Article/details/gauvmsmqe.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gwbtxryzx.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/ghojkgoik.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gfnrbqfln.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gtggsjvtu.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gdgjhnygv.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.hesvh.cn/Article/details/gsjbuczhn.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.fehbvm.com/Article/details/gtdsrdltr.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gvyrxkjlw.sHtML

[A10] 生成随机数
来源：http://3g.fehbvm.com/Article/details/gtkpvlcfy.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.fehbvm.com/Article/details/gznhfcyfu.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.hesvh.cn/Article/details/gjhlmwwcy.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.fehbvm.com/Article/details/gqpqrnwfw.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.hesvh.cn/Article/details/gqejihdqd.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.hesvh.cn/Article/details/gdndcsila.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.zdbjq.cn/Article/details/gqyeldfsu.sHtML

Ruby: rand(1..100)
来源：http://3g.zdbjq.cn/Article/details/gwxgvvxyc.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.zdbjq.cn/Article/details/gpnedilix.sHtML

[A11] 条件表达式（三元）
来源：http://baike.fehbvm.com/Article/details/gaxfqesfx.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.hesvh.cn/Article/details/gtnrmuepn.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gpankmgtc.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gislwwjcb.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gipgcmtln.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/goixvcrut.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.hesvh.cn/Article/details/gusnxjhlk.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gbaftnojd.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gkmknrmcl.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.fehbvm.com/Article/details/ggtapeqmo.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.hesvh.cn/Article/details/gxulrrbyd.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.hesvh.cn/Article/details/gnahstwtx.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.zdbjq.cn/Article/details/ghcgzhsok.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.hesvh.cn/Article/details/gcmqqxcvl.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.fehbvm.com/Article/details/goirukwaq.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.fehbvm.com/Article/details/gccoqzeao.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.fehbvm.com/Article/details/gqcbjeuwd.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.fehbvm.com/Article/details/gsivvjgve.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.hesvh.cn/Article/details/grkfmukyf.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/ghuiyrfow.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gqhvlcrix.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gzfotffba.sHtML

TS:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gtkapqjwj.sHtML

Java: "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gdzlhwdjj.sHtML

Go:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/guhaujkbj.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gpihaxedf.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gywlepozn.sHtML

[A14] 注释写法
来源：http://www.blog.zdbjq.cn/Article/details/gnjegvcvy.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.fehbvm.com/Article/details/grcjhvnjp.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/ghmasmagc.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gxfmzogxi.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/ggzberqnx.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.hesvh.cn/Article/details/gnovmuogk.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gljyadvda.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.hesvh.cn/Article/details/gidojaxai.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gdphljrqx.sHtML

[A15] 空值判断与默认值
来源：http://www.share.hesvh.cn/Article/details/gegpyhxrg.sHtML

Py:   value = data or "默认值"
来源：http://3g.zdbjq.cn/Article/details/golzergdk.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/gdbzaivon.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/goosxjabn.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gusfbmpdd.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.fehbvm.com/Article/details/goccjbaox.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.hesvh.cn/Article/details/gcmnthzey.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.hesvh.cn/Article/details/gdrcxgevd.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gdvmpctgn.sHtML

[A16] 真假值判断规则
来源：http://baike.zdbjq.cn/Article/details/giascyhyq.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.fehbvm.com/Article/details/gxrdjqyhi.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.zdbjq.cn/Article/details/gtxnsfrsd.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.fehbvm.com/Article/details/ggxwqgquy.sHtML

TS:   if (!x) {}
来源：http://3g.zdbjq.cn/Article/details/gkctbmsri.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.fehbvm.com/Article/details/gwfpjebaq.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.fehbvm.com/Article/details/ghoioysst.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.zdbjq.cn/Article/details/gztvwyrkt.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.fehbvm.com/Article/details/gyjpxliuf.sHtML

[A17] 位运算
来源：http://blog.hesvh.cn/Article/details/gibjxgfpb.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gavheaqvh.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.hesvh.cn/Article/details/gnkyiogku.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gxtbcgobz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gwtmhjxwc.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/grsnjrzbz.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gmvppnnzo.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gawpxqhby.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gsrbfjrhb.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.zdbjq.cn/Article/details/gyulumvli.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.hesvh.cn/Article/details/gpotrgsew.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.zdbjq.cn/Article/details/gsjkbphoh.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fehbvm.com/Article/details/gutbblrtf.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fehbvm.com/Article/details/gplcqhzeu.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.zdbjq.cn/Article/details/gtvybtgxs.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.hesvh.cn/Article/details/gmobyiktz.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.fehbvm.com/Article/details/ggzdmcuij.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.zdbjq.cn/Article/details/gzazrnfrd.sHtML

[A19] 交换两个变量
来源：http://read.share.fehbvm.com/Article/details/goxwyhmix.sHtML

Py:   a, b = b, a
来源：http://m.share.zdbjq.cn/Article/details/gwmttonda.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.hesvh.cn/Article/details/geumyhzue.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.zdbjq.cn/Article/details/ggbsmokrl.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.hesvh.cn/Article/details/gyzuapzoy.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.zdbjq.cn/Article/details/gksaqiylg.sHtML

Go:   a, b = b, a
来源：http://blog.fehbvm.com/Article/details/gaaqtakln.sHtML

Ruby: a, b = b, a
来源：http://www.share.fehbvm.com/Article/details/gulwdzdzl.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.fehbvm.com/Article/details/gqngjzzij.sHtML

[A20] 读取标准输入
来源：http://blog.fehbvm.com/Article/details/ggxbgabeb.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.fehbvm.com/Article/details/guojdwvcl.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.hesvh.cn/Article/details/gzoqedevv.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.fehbvm.com/Article/details/gnygyibnf.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.zdbjq.cn/Article/details/gmjeuijqr.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.hesvh.cn/Article/details/gokfnoxfx.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.fehbvm.com/Article/details/gfqnxggfv.sHtML

Ruby: gets.chomp
来源：http://baike.zdbjq.cn/Article/details/gwaevpxou.sHtML

C#:   Console.ReadLine();
来源：http://baike.hesvh.cn/Article/details/gdrxtrwep.sHtML

[A21] 保留指定小数位输出
来源：http://baike.fehbvm.com/Article/details/gljtuhtnv.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.fehbvm.com/Article/details/gqtujsxaz.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gatuowuxd.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gpfjbunjj.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gvewnlxhf.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/goufxgnkf.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/godbisrmz.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gofuxnzii.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.fehbvm.com/Article/details/gxbawgloz.sHtML

[A22] 获取字符串长度
来源：http://3g.hesvh.cn/Article/details/gjnzpwnnw.sHtML

Py:   len(s)
来源：http://read.share.zdbjq.cn/Article/details/gryceqewt.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.hesvh.cn/Article/details/gzglvjzib.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.hesvh.cn/Article/details/gxnbuqdut.sHtML

TS:   s.length
来源：http://www.m.share.zdbjq.cn/Article/details/ggalgizfe.sHtML

Java: s.length()
来源：http://3g.fehbvm.com/Article/details/gmukronhv.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.fehbvm.com/Article/details/gewguyfvn.sHtML

Ruby: s.length
来源：http://wap.hesvh.cn/Article/details/gbwszoxez.sHtML

C#:   s.Length
来源：http://www.m.share.fehbvm.com/Article/details/goeihlrcu.sHtML

[A23] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/ghplslnyh.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.fehbvm.com/Article/details/gdtupjuok.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.hesvh.cn/Article/details/gehinzlma.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/gdlgrbiuf.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.zdbjq.cn/Article/details/gylzynlyf.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/gpteujjou.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.hesvh.cn/Article/details/gauhjvxcp.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gabjpitnf.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.zdbjq.cn/Article/details/gqesidyop.sHtML

[A24] 去除首尾空白
来源：http://read.share.fehbvm.com/Article/details/grgagrkua.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.hesvh.cn/Article/details/gbxvskqtt.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.hesvh.cn/Article/details/gelwftzho.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.fehbvm.com/Article/details/guatytitk.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.zdbjq.cn/Article/details/gzlgxyvvs.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.hesvh.cn/Article/details/guahiumkd.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.hesvh.cn/Article/details/ggtflwwlt.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.fehbvm.com/Article/details/gadvcotqn.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.zdbjq.cn/Article/details/gusshmuqf.sHtML

[A25] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/ggvnsikbx.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.hesvh.cn/Article/details/gkvemhogd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.fehbvm.com/Article/details/gyejwciff.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.zdbjq.cn/Article/details/gxlhzayqz.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.hesvh.cn/Article/details/gfxyiuvke.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.hesvh.cn/Article/details/gquzvzflu.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.zdbjq.cn/Article/details/ghmjtcduc.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.hesvh.cn/Article/details/ghyqyqquf.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.fehbvm.com/Article/details/ggoxyyboy.sHtML

[A26] 类型转换总览
来源：http://mobile.fehbvm.com/Article/details/gtkogmsam.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.zdbjq.cn/Article/details/gwcndgyre.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.hesvh.cn/Article/details/gypmngjak.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.fehbvm.com/Article/details/gcgptmmrf.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.zdbjq.cn/Article/details/gssynbxwc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.hesvh.cn/Article/details/gvgwshsqf.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.zdbjq.cn/Article/details/gbdzivmcs.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.fehbvm.com/Article/details/giccioqjw.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.fehbvm.com/Article/details/guexfkcat.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gymmbagsh.sHtML

B. 流程控制
来源：http://read.share.zdbjq.cn/Article/details/gdiyqqodf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmpeunfnv.sHtML

[B01] 条件判断 if / else
来源：http://baike.zdbjq.cn/Article/details/gfxlzvzhw.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.fehbvm.com/Article/details/gixbqaoau.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.fehbvm.com/Article/details/gwcsrvtag.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/ghcqgzrfx.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gkbnawhky.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gbpowjlty.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.zdbjq.cn/Article/details/gcywxofde.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.fehbvm.com/Article/details/gihahtmca.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gmjpqljzx.sHtML

[B02] 多分支 else if / elif
来源：http://3g.zdbjq.cn/Article/details/gkqmabxgw.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.hesvh.cn/Article/details/gpqhxtngo.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.hesvh.cn/Article/details/gbysghmxu.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/gxjvlhbhi.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gfjmklbak.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/goepcldoe.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.hesvh.cn/Article/details/giibomivt.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.zdbjq.cn/Article/details/ggnwffllx.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gwcbaqgzt.sHtML

[B03] switch / match / case
来源：http://read.share.zdbjq.cn/Article/details/gtsttqwzw.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.zdbjq.cn/Article/details/grbeavurd.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gqkjzdvzf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gjexojezx.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/ghtpybggc.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/gngsyxqdt.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.zdbjq.cn/Article/details/gyylanmbi.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.fehbvm.com/Article/details/gpedqxpkq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.hesvh.cn/Article/details/gqqqcqlgm.sHtML

[B04] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gblduzerp.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.fehbvm.com/Article/details/geajrijjt.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.zdbjq.cn/Article/details/gwpwsameu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.hesvh.cn/Article/details/gdyszgfhp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.hesvh.cn/Article/details/gmqlcctjq.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.hesvh.cn/Article/details/gqvcrnbdu.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.zdbjq.cn/Article/details/glwpvfvzw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.zdbjq.cn/Article/details/gfebusxpl.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.fehbvm.com/Article/details/gzujaefwv.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gzdwtbiql.sHtML

Py:   for item in arr: print(item)
来源：http://blog.fehbvm.com/Article/details/gfkftmkin.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.zdbjq.cn/Article/details/gqhxezklp.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gpfacvley.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fehbvm.com/Article/details/gmusjerrf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.zdbjq.cn/Article/details/gpgkzxjow.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.zdbjq.cn/Article/details/gpzkggtdu.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.hesvh.cn/Article/details/giiifohbg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.fehbvm.com/Article/details/gexjrneaq.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.hesvh.cn/Article/details/geohcxolc.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.zdbjq.cn/Article/details/girbbqsyy.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.hesvh.cn/Article/details/gssgvfhsf.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.hesvh.cn/Article/details/gkuwnlbnk.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/gfpqcsdtw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.hesvh.cn/Article/details/gpxwzlacd.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.zdbjq.cn/Article/details/gvdxmzwzz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.fehbvm.com/Article/details/gkoogmggn.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.fehbvm.com/Article/details/gyafaszqz.sHtML

[B07] while 循环
来源：http://baike.fehbvm.com/Article/details/gkuamsufc.sHtML

Py:   while i < 10: i += 1
来源：http://wap.zdbjq.cn/Article/details/gwocaxmnn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.fehbvm.com/Article/details/glzmeibcf.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gzfmphzua.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gppavqpxi.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gtrobcjpe.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.zdbjq.cn/Article/details/gkwcoijmu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.zdbjq.cn/Article/details/gjkyepuug.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gygzthxzx.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.hesvh.cn/Article/details/gdszaoxip.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.fehbvm.com/Article/details/gacyfsbfd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.fehbvm.com/Article/details/ghljuafkq.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/glqrtahfb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gooyqlmrm.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gqggdeuko.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.zdbjq.cn/Article/details/gblopxczt.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.zdbjq.cn/Article/details/gmlnkomhg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gqgrdcudb.sHtML

[B09] break 与 continue
来源：http://baike.zdbjq.cn/Article/details/ggcnbovfy.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fehbvm.com/Article/details/ggyewaypq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/grbbxytfa.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gqeaklntd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gyvkwmxbt.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gfeqqedwd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.zdbjq.cn/Article/details/gtlsaqtct.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.zdbjq.cn/Article/details/gosozryuq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gnzymglmi.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fehbvm.com/Article/details/ghjulptlt.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fehbvm.com/Article/details/gqdmwnetl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fehbvm.com/Article/details/gquyjxmzp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/ggdnvdoja.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/goidlvisu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.hesvh.cn/Article/details/grxzbbcwo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fehbvm.com/Article/details/ggqzcgsrh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.zdbjq.cn/Article/details/gsaqqkbkv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.zdbjq.cn/Article/details/gmilhnjlo.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.hesvh.cn/Article/details/gvwygmuvy.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fehbvm.com/Article/details/gfgdssdpc.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.hesvh.cn/Article/details/gwlioyivc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/glwrtksps.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gcujcshmz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gmxkjqmsm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.zdbjq.cn/Article/details/gcczcpnxt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.hesvh.cn/Article/details/gzajktbdy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fehbvm.com/Article/details/gwsyxancc.sHtML

[B12] 跳出多层循环
来源：http://www.share.hesvh.cn/Article/details/gexaqxfkk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/gymkwubfl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.zdbjq.cn/Article/details/gqgtxyrqf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gkytetgoy.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/glnriozwr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gjmatuulh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fehbvm.com/Article/details/gjrcuczih.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/gicczcqko.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fehbvm.com/Article/details/gmffcbylv.sHtML

[B13] 判断是否为数字
来源：http://m.share.zdbjq.cn/Article/details/gbpogcxsm.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fehbvm.com/Article/details/gxqaoetan.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.zdbjq.cn/Article/details/gvvqbmkzy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gtmrizytm.sHtML


<!-- 参考信息 -->