代发 wailian999

JS:   const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/ggrlqerip.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gvgystedh.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gbztqayng.sHtML

Go:   const PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/grymyagbj.sHtML

Ruby: PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gknbtydjk.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gusgjmczc.sHtML

[A04] 判断变量类型
来源：http://3g.zdbjq.cn/Article/details/gqvpkvdyv.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.zdbjq.cn/Article/details/gqaxdgshz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.zdbjq.cn/Article/details/grioewxev.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fehbvm.com/Article/details/glaaxltbk.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.hesvh.cn/Article/details/gprdlxmvz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.zdbjq.cn/Article/details/gcxdejkol.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.fehbvm.com/Article/details/gbeivuxzf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.zdbjq.cn/Article/details/gknaoysqc.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.zdbjq.cn/Article/details/gkfmhtwmv.sHtML

[A05] 整数除法与取模
来源：http://wap.zdbjq.cn/Article/details/gkgeorzmj.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.zdbjq.cn/Article/details/gbdfyemyh.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gskrncirx.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/gxfjfaxbb.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gnvkbciyw.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gkhnbdjay.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/grehgrihh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gjupqmjpb.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/ghutoynbn.sHtML

[A06] 字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gcmrnzvau.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gkhabqxgj.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.hesvh.cn/Article/details/grqweyvrj.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.fehbvm.com/Article/details/gbyamxunz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.zdbjq.cn/Article/details/glqvirvbb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gqvqjdaoa.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.hesvh.cn/Article/details/gybeaobgb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.zdbjq.cn/Article/details/gnrsslbqh.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gietuvoxx.sHtML

[A07] 数字转字符串
来源：http://3g.fehbvm.com/Article/details/gpekdgqmy.sHtML

Py:   str(42)
来源：http://3g.fehbvm.com/Article/details/ghhgrgtba.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.hesvh.cn/Article/details/gydriwthz.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.fehbvm.com/Article/details/gjacirfjq.sHtML

TS:   String(42)
来源：http://www.blog.zdbjq.cn/Article/details/gqopzkeju.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.zdbjq.cn/Article/details/gfkptfqkh.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.hesvh.cn/Article/details/gxtqfpqry.sHtML

Ruby: 42.to_s
来源：http://3g.hesvh.cn/Article/details/gyyfytslm.sHtML

C#:   42.ToString()
来源：http://blog.hesvh.cn/Article/details/gohihbvtv.sHtML

[A08] 取整与四舍五入
来源：http://read.share.hesvh.cn/Article/details/gstessyll.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gmzjqsiwl.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.zdbjq.cn/Article/details/gkjqeiaak.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gcgxvcwqs.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.fehbvm.com/Article/details/gsagtyafi.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gaqedvucw.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/ghcucwvvh.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.zdbjq.cn/Article/details/gyoyoppwb.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gdckorqbo.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gxgutgfkf.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gqzcyunfh.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/ganssupnx.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gppoctqzw.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/googfewxe.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gxfaafeuk.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.hesvh.cn/Article/details/gguoudyot.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.zdbjq.cn/Article/details/gnwduclfx.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gcbzcmpuo.sHtML

[A10] 生成随机数
来源：http://www.blog.fehbvm.com/Article/details/grkkkraxy.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.zdbjq.cn/Article/details/gwmhrwzyp.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.fehbvm.com/Article/details/gmqzzhqfh.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.hesvh.cn/Article/details/gfupctzla.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fehbvm.com/Article/details/gljhvevtc.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gxwfbhpjs.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.hesvh.cn/Article/details/giaprprpq.sHtML

Ruby: rand(1..100)
来源：http://m.share.hesvh.cn/Article/details/glptayhfx.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.fehbvm.com/Article/details/gxccsjgov.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.hesvh.cn/Article/details/gpddppwnp.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.hesvh.cn/Article/details/gunawlxwz.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gosvlital.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gwoqqkpky.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gpiltsvhj.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gdzakfsku.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.hesvh.cn/Article/details/goolnzbdm.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gebvkcxtl.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gfbmpioxy.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.zdbjq.cn/Article/details/gqethleqg.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.hesvh.cn/Article/details/grupvgjyp.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.zdbjq.cn/Article/details/gmazgiqmg.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.zdbjq.cn/Article/details/gznwjjimh.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.fehbvm.com/Article/details/gaesjnchs.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.fehbvm.com/Article/details/gziiutevj.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.hesvh.cn/Article/details/guuxmpetd.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.fehbvm.com/Article/details/gkqjzcgdo.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.zdbjq.cn/Article/details/grdxkqaqt.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.zdbjq.cn/Article/details/gkiokzinz.sHtML

Py:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gxtplvwyc.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gbevxiqqm.sHtML

JS:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/ggcpgafde.sHtML

TS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gihqjwaex.sHtML

Java: "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/guepcedmm.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gbeeahppv.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gxmgmmvfi.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gcnlitcmr.sHtML

[A14] 注释写法
来源：http://m.share.hesvh.cn/Article/details/gavqjweuf.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.zdbjq.cn/Article/details/gcryqksjg.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/grzsfikxn.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/ghotbueyj.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gmaoazdca.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.fehbvm.com/Article/details/grqxbicse.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gpsvpqtdu.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.hesvh.cn/Article/details/gnnojinyz.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gdgarabki.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.fehbvm.com/Article/details/grpjdthxs.sHtML

Py:   value = data or "默认值"
来源：http://mobile.fehbvm.com/Article/details/gekyefbth.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gaocamvzv.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gogtvylfr.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/gclfjacan.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.hesvh.cn/Article/details/gprdlchwe.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.fehbvm.com/Article/details/gbyqticmk.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.zdbjq.cn/Article/details/gukqturyy.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/gnrupoiyx.sHtML

[A16] 真假值判断规则
来源：http://www.share.fehbvm.com/Article/details/glumcdvvh.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.zdbjq.cn/Article/details/gpqttclss.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.zdbjq.cn/Article/details/gnvdcyfvj.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.fehbvm.com/Article/details/gvckrmcea.sHtML

TS:   if (!x) {}
来源：http://read.share.zdbjq.cn/Article/details/gurkpscpf.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.zdbjq.cn/Article/details/gluxbrscu.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.fehbvm.com/Article/details/gqoxhdawh.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.hesvh.cn/Article/details/gibrpfbzk.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gbquivhkp.sHtML

[A17] 位运算
来源：http://blog.zdbjq.cn/Article/details/ghdjmmwic.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gfgffiuyf.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.hesvh.cn/Article/details/gxsjnedsb.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gbfxulvam.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/goxfdpgyj.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gnjcfenib.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/ghcdloqwv.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gqkqwftiu.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gvpvqlhfz.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.zdbjq.cn/Article/details/gklsbsgum.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.hesvh.cn/Article/details/grcigmwtx.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.zdbjq.cn/Article/details/gwjlaqqyn.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fehbvm.com/Article/details/gsgsaexli.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fehbvm.com/Article/details/gnuxlsknm.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.zdbjq.cn/Article/details/ggqgbdaxj.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.hesvh.cn/Article/details/gbsqjbrdf.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.fehbvm.com/Article/details/gwmolrxmj.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.hesvh.cn/Article/details/gzrkhfbjc.sHtML

[A19] 交换两个变量
来源：http://blog.zdbjq.cn/Article/details/gdfbubrcn.sHtML

Py:   a, b = b, a
来源：http://m.share.fehbvm.com/Article/details/gwmuuqmfd.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.hesvh.cn/Article/details/gqyoiyvxx.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.zdbjq.cn/Article/details/gwlkvwlog.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.hesvh.cn/Article/details/giazuzslz.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.fehbvm.com/Article/details/giajfvtyg.sHtML

Go:   a, b = b, a
来源：http://read.share.hesvh.cn/Article/details/ghpxnixgf.sHtML

Ruby: a, b = b, a
来源：http://blog.fehbvm.com/Article/details/gbgzsgqez.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.fehbvm.com/Article/details/gmzelvvam.sHtML

[A20] 读取标准输入
来源：http://www.share.zdbjq.cn/Article/details/gggscdcim.sHtML

Py:   name = input("请输入：")
来源：http://blog.hesvh.cn/Article/details/gypoqgruu.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.hesvh.cn/Article/details/gxuahelsc.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.fehbvm.com/Article/details/ggbdopfwz.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.zdbjq.cn/Article/details/gonbwqckx.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.fehbvm.com/Article/details/gfzxwgboc.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.fehbvm.com/Article/details/gflvktzkh.sHtML

Ruby: gets.chomp
来源：http://www.m.share.zdbjq.cn/Article/details/gcozdptpa.sHtML

C#:   Console.ReadLine();
来源：http://www.share.hesvh.cn/Article/details/gjpyxbvow.sHtML

[A21] 保留指定小数位输出
来源：http://wap.zdbjq.cn/Article/details/gabotfplh.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.fehbvm.com/Article/details/gwhxostrr.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/goisodjay.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gchjfxczn.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gbkaffqxx.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/gofbbbrvq.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/glktgbetw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/gfvgfzymk.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.zdbjq.cn/Article/details/ggwwtozge.sHtML

[A22] 获取字符串长度
来源：http://mobile.hesvh.cn/Article/details/gpfavmfgx.sHtML

Py:   len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gwoxqkzja.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.fehbvm.com/Article/details/gnvzqmexf.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.fehbvm.com/Article/details/glgfniqkt.sHtML

TS:   s.length
来源：http://www.m.share.hesvh.cn/Article/details/grxookspf.sHtML

Java: s.length()
来源：http://3g.fehbvm.com/Article/details/gxfzewbdy.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.zdbjq.cn/Article/details/ghluqcxng.sHtML

Ruby: s.length
来源：http://m.share.zdbjq.cn/Article/details/gsxqekfel.sHtML

C#:   s.Length
来源：http://baike.zdbjq.cn/Article/details/grguufclk.sHtML

[A23] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gdyzdjmjj.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.zdbjq.cn/Article/details/gazejbscv.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.fehbvm.com/Article/details/gdrsfvopb.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.zdbjq.cn/Article/details/ghpoxtjse.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.hesvh.cn/Article/details/gsqbiwmwf.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.hesvh.cn/Article/details/gppiaxzcc.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.hesvh.cn/Article/details/gcjfrafqc.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gnxyusvuh.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.hesvh.cn/Article/details/geiwrjuxe.sHtML

[A24] 去除首尾空白
来源：http://mobile.hesvh.cn/Article/details/gramyqikc.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.zdbjq.cn/Article/details/glrimccfu.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.zdbjq.cn/Article/details/glxcrgyqg.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fehbvm.com/Article/details/genstywvk.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fehbvm.com/Article/details/gqkkpmozs.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.zdbjq.cn/Article/details/gotkswlwd.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.hesvh.cn/Article/details/gqepwygdm.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.hesvh.cn/Article/details/gesuuubyg.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.hesvh.cn/Article/details/glwbvhvyv.sHtML

[A25] 字符串比较
来源：http://3g.hesvh.cn/Article/details/glezbgnli.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.hesvh.cn/Article/details/gknqxzltc.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.fehbvm.com/Article/details/gmyuzrcye.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fehbvm.com/Article/details/gwkaonfyd.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.hesvh.cn/Article/details/gmeoizcyy.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.hesvh.cn/Article/details/gixeghnub.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.hesvh.cn/Article/details/gxolnfwis.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.fehbvm.com/Article/details/gvxddpmto.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.hesvh.cn/Article/details/gukkbpvmg.sHtML

[A26] 类型转换总览
来源：http://www.m.share.fehbvm.com/Article/details/gbbnlffje.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.hesvh.cn/Article/details/gougqhlrz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.hesvh.cn/Article/details/gmttmlxaq.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.zdbjq.cn/Article/details/gvuacdplc.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.zdbjq.cn/Article/details/ghvqxycty.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.fehbvm.com/Article/details/gwodvtkyu.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.zdbjq.cn/Article/details/giecubnjq.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.fehbvm.com/Article/details/guryhxhge.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.hesvh.cn/Article/details/gesfthxyf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggfyufmuo.sHtML

B. 流程控制
来源：http://blog.fehbvm.com/Article/details/gjqxrtiye.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxxvkkipx.sHtML

[B01] 条件判断 if / else
来源：http://3g.fehbvm.com/Article/details/gaeglqkei.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.zdbjq.cn/Article/details/gxbxsewpn.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.fehbvm.com/Article/details/gpblcmjjw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/grpmufpjl.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gtxrovolz.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gkdjncpyg.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.hesvh.cn/Article/details/gxhfljbxc.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.zdbjq.cn/Article/details/gnkxxkwny.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/geyyraqew.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.fehbvm.com/Article/details/gcweiuocl.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.hesvh.cn/Article/details/gvkbfailx.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.zdbjq.cn/Article/details/gqiuruxrd.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gqokvgqeu.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gyhwynuhk.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gxtjzqunq.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.zdbjq.cn/Article/details/gbfdpkqvz.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.hesvh.cn/Article/details/gcztgeodx.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/galuqkluj.sHtML

[B03] switch / match / case
来源：http://read.share.fehbvm.com/Article/details/gwnlrwxio.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.zdbjq.cn/Article/details/gervidzkz.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gekdhjxco.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/glgmvzcrj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gvgzjxkek.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gsqaljipc.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.fehbvm.com/Article/details/gpyrjscfv.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.hesvh.cn/Article/details/gvftkpvrt.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.hesvh.cn/Article/details/ghewnukye.sHtML

[B04] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gfbkmsmws.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.zdbjq.cn/Article/details/gvnqafmrq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.zdbjq.cn/Article/details/guvaiiqpo.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.hesvh.cn/Article/details/giffkjyoc.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.zdbjq.cn/Article/details/geldkixvc.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.fehbvm.com/Article/details/gjzhpmjzd.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fehbvm.com/Article/details/gtasjlzur.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.fehbvm.com/Article/details/gbueyzlob.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.hesvh.cn/Article/details/gitcejmvh.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gvmykcjwd.sHtML

Py:   for item in arr: print(item)
来源：http://3g.fehbvm.com/Article/details/guwourwgg.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.zdbjq.cn/Article/details/gelnxmhbd.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/guuhwkjbc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.zdbjq.cn/Article/details/gklzuieuv.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.fehbvm.com/Article/details/gtqnmlxjc.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.zdbjq.cn/Article/details/gennvdthy.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.zdbjq.cn/Article/details/gitydcanh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gsarqmpff.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.hesvh.cn/Article/details/gtzrpgnzs.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.zdbjq.cn/Article/details/gjurekggu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.zdbjq.cn/Article/details/gweggpnqn.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/ggplrhxvu.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/gwscpwzdl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.fehbvm.com/Article/details/gagrekgah.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.hesvh.cn/Article/details/gnlsleuhn.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.fehbvm.com/Article/details/gmxtahqso.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.hesvh.cn/Article/details/glwbmsapx.sHtML

[B07] while 循环
来源：http://read.share.hesvh.cn/Article/details/gfidagmgx.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.hesvh.cn/Article/details/gltgsqkgr.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.hesvh.cn/Article/details/gfpaqqldx.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gqfzvgkqj.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gdpgmhwre.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/ggbxgomfl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.zdbjq.cn/Article/details/ghiopmusi.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.zdbjq.cn/Article/details/gnfxcnehk.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gygzgqifo.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.hesvh.cn/Article/details/gkjtidqjv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.zdbjq.cn/Article/details/ghyzblcfc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.fehbvm.com/Article/details/geqqnspfv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/geczxirgv.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gacwfhvcw.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gmlelsanm.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.hesvh.cn/Article/details/glkcpxgot.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.fehbvm.com/Article/details/gjdlryhod.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gekykqidm.sHtML

[B09] break 与 continue
来源：http://mobile.hesvh.cn/Article/details/gixpjediu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.fehbvm.com/Article/details/geoberyzn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gjdnzyety.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gqlpcbrci.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gtudpxgnb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gfrguljch.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.zdbjq.cn/Article/details/gfjdjozzu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.zdbjq.cn/Article/details/goopedsxc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gycfqwjgp.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.zdbjq.cn/Article/details/gjkswsmwt.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.zdbjq.cn/Article/details/gfruyuxpa.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.hesvh.cn/Article/details/gmpuqzfxw.sHtML


<!-- 参考信息 -->