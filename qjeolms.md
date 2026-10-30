代发 wailian999

Ruby: 42.to_s
来源：http://baike.fehbvm.com/Article/details/gjzdnauli.sHtML

C#:   42.ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/glxsbxdxg.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fehbvm.com/Article/details/gzlyobbha.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gjeihcppo.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.zdbjq.cn/Article/details/gkmsgkxrx.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gtdbjemte.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.zdbjq.cn/Article/details/gfxfbntiq.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gqrwgtsou.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/ggqroisxq.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.hesvh.cn/Article/details/ggledzofi.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gqkoxfubl.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.fehbvm.com/Article/details/gphpqeeir.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gzokuzlaf.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gdvvywujv.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.hesvh.cn/Article/details/grsxjfuuu.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gvaskvvls.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gzwkrurpm.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.zdbjq.cn/Article/details/gofjtfbgc.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.zdbjq.cn/Article/details/gmbhvvetf.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gqekbwnsu.sHtML

[A10] 生成随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gnqqqimmc.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.zdbjq.cn/Article/details/geqslgtql.sHtML

PHP:  random_int(1, 100);
来源：http://baike.fehbvm.com/Article/details/gpesdmhft.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.zdbjq.cn/Article/details/gwoypiqte.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.hesvh.cn/Article/details/gzggzsdgr.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.hesvh.cn/Article/details/gajhmmvpq.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.hesvh.cn/Article/details/ghvsplwvu.sHtML

Ruby: rand(1..100)
来源：http://blog.fehbvm.com/Article/details/ghdmrwzcj.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.hesvh.cn/Article/details/gfmushfzl.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.hesvh.cn/Article/details/gdpftzmet.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.fehbvm.com/Article/details/gwmrrwtoj.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gcyasqalr.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gfqrqfrfg.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gbezqdwnq.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/ghgrpbped.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.fehbvm.com/Article/details/gpmnzxwzr.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/ggsqrpkus.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/giourhmsv.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.hesvh.cn/Article/details/grysqerpw.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.hesvh.cn/Article/details/gqrwccdzw.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.hesvh.cn/Article/details/gookfrfdv.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.hesvh.cn/Article/details/guxgsagir.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.hesvh.cn/Article/details/gbqsidwzm.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.fehbvm.com/Article/details/gbqhxnfgy.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.fehbvm.com/Article/details/gpsrqwhlm.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.zdbjq.cn/Article/details/guxvovzmi.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.hesvh.cn/Article/details/gqjkpymsu.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.zdbjq.cn/Article/details/glsmywcoh.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gdhcbpzsp.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gunobtclx.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/griayofuj.sHtML

TS:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gwwmtedkp.sHtML

Java: "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/glabaiacn.sHtML

Go:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gidkgnhcw.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gsmjnkdxs.sHtML

C#:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gxeynyegq.sHtML

[A14] 注释写法
来源：http://3g.hesvh.cn/Article/details/gbjgwvrti.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.hesvh.cn/Article/details/gdezfufhl.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gspggjoop.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gyyhrwmhi.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gdgfcstof.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.fehbvm.com/Article/details/guytsqwtc.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/grwexswjz.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.hesvh.cn/Article/details/gebyufujk.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gvgsbpaul.sHtML

[A15] 空值判断与默认值
来源：http://mobile.zdbjq.cn/Article/details/gbunnhzir.sHtML

Py:   value = data or "默认值"
来源：http://read.share.hesvh.cn/Article/details/gbqpnqhqq.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gpkspmpeh.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gzlktmfjj.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gbdfosfue.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.hesvh.cn/Article/details/ghkapmrov.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.zdbjq.cn/Article/details/gavrcgojt.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.hesvh.cn/Article/details/gechcwsvc.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/gifcaftsl.sHtML

[A16] 真假值判断规则
来源：http://www.share.hesvh.cn/Article/details/giwcprugt.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.zdbjq.cn/Article/details/ggrcorbaz.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.fehbvm.com/Article/details/gcawevcbq.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.zdbjq.cn/Article/details/gfnnjhrkw.sHtML

TS:   if (!x) {}
来源：http://baike.zdbjq.cn/Article/details/ggstnofkl.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.fehbvm.com/Article/details/gfvoaymrt.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.hesvh.cn/Article/details/gpxegxpnt.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.zdbjq.cn/Article/details/gtkedralb.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.hesvh.cn/Article/details/gneszupqb.sHtML

[A17] 位运算
来源：http://read.share.zdbjq.cn/Article/details/guzpjuuep.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gkdmvffcy.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.zdbjq.cn/Article/details/gpksbnocq.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gxwlbbvoq.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gfwruvnbv.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gprryjdwr.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gtfttnaci.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gtnkyxkgg.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/grlsjmvso.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.hesvh.cn/Article/details/ggcspggtu.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.zdbjq.cn/Article/details/glcenpsrw.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.fehbvm.com/Article/details/gjomaeumm.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fehbvm.com/Article/details/gjyvkkdjj.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.hesvh.cn/Article/details/gnubczyyi.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.hesvh.cn/Article/details/geluztalk.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.fehbvm.com/Article/details/gbtasjrpu.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.hesvh.cn/Article/details/gygtekdsf.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.hesvh.cn/Article/details/gpyrpgmfs.sHtML

[A19] 交换两个变量
来源：http://3g.zdbjq.cn/Article/details/gtlbpedbs.sHtML

Py:   a, b = b, a
来源：http://baike.hesvh.cn/Article/details/goobaixlj.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.zdbjq.cn/Article/details/gdvyjefvf.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.zdbjq.cn/Article/details/gjbnbstkn.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.zdbjq.cn/Article/details/gwosufejy.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.hesvh.cn/Article/details/ggsetmzpm.sHtML

Go:   a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/gxveeybso.sHtML

Ruby: a, b = b, a
来源：http://baike.zdbjq.cn/Article/details/gsobhgghm.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.zdbjq.cn/Article/details/gnodgqlri.sHtML

[A20] 读取标准输入
来源：http://wap.fehbvm.com/Article/details/genfqduld.sHtML

Py:   name = input("请输入：")
来源：http://blog.zdbjq.cn/Article/details/gbowgaxmj.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.zdbjq.cn/Article/details/gfyzkljvb.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.hesvh.cn/Article/details/glhrbryos.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.hesvh.cn/Article/details/gtwqevfdq.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.zdbjq.cn/Article/details/glgfcjljx.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.hesvh.cn/Article/details/gzikrmgkp.sHtML

Ruby: gets.chomp
来源：http://www.share.hesvh.cn/Article/details/gfvmxjisw.sHtML

C#:   Console.ReadLine();
来源：http://3g.zdbjq.cn/Article/details/gmbxkutns.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.fehbvm.com/Article/details/gkfomxgrl.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.fehbvm.com/Article/details/gvchoadsm.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gbdctxwcs.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gadrtprez.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gtoprpbbu.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/gaehdfgon.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/gzdzofwch.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.fehbvm.com/Article/details/gvermtvwz.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.hesvh.cn/Article/details/gutrkvofz.sHtML

[A22] 获取字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gdptyhwpi.sHtML

Py:   len(s)
来源：http://wap.zdbjq.cn/Article/details/gptnwhzal.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.fehbvm.com/Article/details/ggdrzoyhe.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.zdbjq.cn/Article/details/gamavfbbs.sHtML

TS:   s.length
来源：http://wap.zdbjq.cn/Article/details/gztbjrbkw.sHtML

Java: s.length()
来源：http://m.share.fehbvm.com/Article/details/girwetsiu.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.hesvh.cn/Article/details/geseceqeu.sHtML

Ruby: s.length
来源：http://www.blog.hesvh.cn/Article/details/gbmvkebnb.sHtML

C#:   s.Length
来源：http://read.share.fehbvm.com/Article/details/gtjsdclmh.sHtML

[A23] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gpcxktehp.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.hesvh.cn/Article/details/gduaytcyl.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.zdbjq.cn/Article/details/gdraysobh.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/gramptdqo.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.hesvh.cn/Article/details/grwlygyoy.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/gxvvirjee.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.zdbjq.cn/Article/details/gjmmqruqv.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.fehbvm.com/Article/details/ggyfxvjbh.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.fehbvm.com/Article/details/gpwgntbco.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.zdbjq.cn/Article/details/gdxbmcsog.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.fehbvm.com/Article/details/gdnzmlbyy.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.zdbjq.cn/Article/details/gcftqejwp.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.zdbjq.cn/Article/details/gcnigyodn.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.zdbjq.cn/Article/details/gjqpwjlqe.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.zdbjq.cn/Article/details/grwmhlfps.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.zdbjq.cn/Article/details/gpbclurpa.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.zdbjq.cn/Article/details/gpesmiuql.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.zdbjq.cn/Article/details/gniybozrz.sHtML

[A25] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gdbkzteig.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.zdbjq.cn/Article/details/gtxoshvje.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.zdbjq.cn/Article/details/gailzfaul.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.hesvh.cn/Article/details/gjnhukemq.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.fehbvm.com/Article/details/gayxuyetp.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.zdbjq.cn/Article/details/gykeuhhwn.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.fehbvm.com/Article/details/gxvibgozd.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.hesvh.cn/Article/details/golnbbyof.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/gfcveuubl.sHtML

[A26] 类型转换总览
来源：http://www.m.share.fehbvm.com/Article/details/gouypbccf.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.hesvh.cn/Article/details/gifibaufo.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.zdbjq.cn/Article/details/gheqhevyj.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.hesvh.cn/Article/details/gdzsfqokt.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.fehbvm.com/Article/details/gcndlzrtb.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.hesvh.cn/Article/details/gpgjtgghw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.zdbjq.cn/Article/details/gxgtzspjk.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.hesvh.cn/Article/details/gumbnvyuq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.zdbjq.cn/Article/details/grmzlgchd.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkrazlddk.sHtML

B. 流程控制
来源：http://mobile.hesvh.cn/Article/details/ghoagmngt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grrsjmhkk.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.fehbvm.com/Article/details/gfrocvzpt.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.zdbjq.cn/Article/details/gaprioyxx.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggcwmjrdt.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gklldwdfx.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gduyifuex.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gxlfgbqux.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.hesvh.cn/Article/details/gmlutwnbg.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.zdbjq.cn/Article/details/gclfxepfm.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/gxtoogdhp.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.fehbvm.com/Article/details/goyacyciu.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.zdbjq.cn/Article/details/ggwqkpsob.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.zdbjq.cn/Article/details/glcqzuflb.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gtrqhlnjg.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gazopajmy.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gtxnhehjh.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.zdbjq.cn/Article/details/gvletqobb.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.hesvh.cn/Article/details/gumxssruq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gpawjzejd.sHtML

[B03] switch / match / case
来源：http://blog.zdbjq.cn/Article/details/gpqhoxqgw.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fehbvm.com/Article/details/grkltbnqg.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gaoqufyhe.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gwdpkdkpf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/ggokybryr.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/guwsvmacu.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/gbpduapjt.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.zdbjq.cn/Article/details/gwdtajqay.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.fehbvm.com/Article/details/gyqltykna.sHtML

[B04] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/ggghfldfk.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.hesvh.cn/Article/details/gvrkblpho.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.fehbvm.com/Article/details/gcildtpkq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.hesvh.cn/Article/details/gtrlfecla.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fehbvm.com/Article/details/gvxarlnwv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.zdbjq.cn/Article/details/gopxvqnyu.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.hesvh.cn/Article/details/guaamhvjv.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.fehbvm.com/Article/details/gycozidkl.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.hesvh.cn/Article/details/gjqsbnfgo.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gerxtcpka.sHtML

Py:   for item in arr: print(item)
来源：http://baike.fehbvm.com/Article/details/gcggccbsu.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.hesvh.cn/Article/details/gedjwyvrt.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fehbvm.com/Article/details/gyiufvzxq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gqximujyy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.zdbjq.cn/Article/details/gwmhfpbhy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.fehbvm.com/Article/details/grcjzbdrt.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.fehbvm.com/Article/details/gebpqkghn.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.fehbvm.com/Article/details/gqzyrazwq.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fehbvm.com/Article/details/gbqpeffwr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.zdbjq.cn/Article/details/gqgusresw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.zdbjq.cn/Article/details/gbpfixrfy.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/gqrabeair.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/gxxybrxpu.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fehbvm.com/Article/details/gczdhjreh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.hesvh.cn/Article/details/gdkagsvdf.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.hesvh.cn/Article/details/govhgxggl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.zdbjq.cn/Article/details/gjwzadmzk.sHtML

[B07] while 循环
来源：http://www.share.hesvh.cn/Article/details/grsayzeew.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fehbvm.com/Article/details/gmcuhbiyl.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fehbvm.com/Article/details/ghgtmwvdn.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gdgplshhf.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gpzzjbbfu.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gdwlojrxm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.zdbjq.cn/Article/details/ggqimuukx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.zdbjq.cn/Article/details/gabxgidgk.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gojahhfkq.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.zdbjq.cn/Article/details/ggweufjfg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fehbvm.com/Article/details/gdcikldyv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.zdbjq.cn/Article/details/guzxqixiq.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gfgokrpdd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gjgcgdbfh.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/goqebpggp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.hesvh.cn/Article/details/gnutclnqf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.hesvh.cn/Article/details/gjgdqerrk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gqbpoowmi.sHtML

[B09] break 与 continue
来源：http://read.share.fehbvm.com/Article/details/ghnymbwsm.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.hesvh.cn/Article/details/glweiqxdn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gysvsyfhc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqpspaowg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gaugldodp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gorvzvcmu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fehbvm.com/Article/details/gpeklyrui.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.hesvh.cn/Article/details/gwxeuzzaf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gctxzzlid.sHtML

[B10] 遍历同时拿索引
来源：http://3g.fehbvm.com/Article/details/gvzquapxo.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.zdbjq.cn/Article/details/gchqbkdha.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.fehbvm.com/Article/details/gfhqlupxx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/gxeanxldf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gogkcioff.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.zdbjq.cn/Article/details/ggqeqhahc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.hesvh.cn/Article/details/girwoampu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.zdbjq.cn/Article/details/gtcacdjkw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.hesvh.cn/Article/details/grkyrzuhz.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.fehbvm.com/Article/details/gtnnsywwy.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.hesvh.cn/Article/details/gkkafqqak.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.zdbjq.cn/Article/details/gbxlyjmqr.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gyvzqacxr.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/gdfvfjequ.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.hesvh.cn/Article/details/gneinpvlz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.hesvh.cn/Article/details/gutbbiylq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.hesvh.cn/Article/details/gberosohs.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fehbvm.com/Article/details/gkkxcdbyh.sHtML

[B12] 跳出多层循环
来源：http://m.share.hesvh.cn/Article/details/gkclgkkag.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fehbvm.com/Article/details/ghmzsudjd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.zdbjq.cn/Article/details/gykvkymcc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gfnqvytxw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gggfglivc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gdqnohpnu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.hesvh.cn/Article/details/gjecqpouj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fehbvm.com/Article/details/gbphiomns.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fehbvm.com/Article/details/gfpednvgx.sHtML

[B13] 判断是否为数字
来源：http://www.blog.hesvh.cn/Article/details/gpaumkofq.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.zdbjq.cn/Article/details/gkbhkhcve.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/gzjvdcpxl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/gltrjatqe.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gryakswfn.sHtML

Java: x instanceof Number
来源：http://read.share.fehbvm.com/Article/details/gbyovmphw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.zdbjq.cn/Article/details/gvsjtmlbj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.zdbjq.cn/Article/details/gtsddkhpo.sHtML

C#:   x is int or double or decimal
来源：http://wap.hesvh.cn/Article/details/gemvispqq.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/gdtkkmcfk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fehbvm.com/Article/details/gmxaboeos.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.hesvh.cn/Article/details/guiixhfng.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/grczcqovl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gkcqbcczd.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gvotkrpwj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fehbvm.com/Article/details/gxdjfszjg.sHtML


<!-- 参考信息 -->