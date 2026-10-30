代发 wailian999

Ruby: 42.to_s
来源：http://blog.fehbvm.com/Article/details/gjphxezcn.sHtML

C#:   42.ToString()
来源：http://blog.hesvh.cn/Article/details/gyrkiepxa.sHtML

[A08] 取整与四舍五入
来源：http://www.share.fehbvm.com/Article/details/gwoxdubcb.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/ggckdpuhw.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.zdbjq.cn/Article/details/gqhdrkdav.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gbuzhsvcl.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.fehbvm.com/Article/details/gdrigisyt.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gxidmykqg.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gixuamecy.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.zdbjq.cn/Article/details/gdrchnaoo.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gvdkdnoij.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.hesvh.cn/Article/details/guxbirqpp.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fehbvm.com/Article/details/ghtrkpatk.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gprsdgjmg.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.fehbvm.com/Article/details/gtrnrjwmx.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gpegjsbqj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gpvzcizcn.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.fehbvm.com/Article/details/guygemkht.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.fehbvm.com/Article/details/ghthggmhs.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.hesvh.cn/Article/details/gjblclqbz.sHtML

[A10] 生成随机数
来源：http://m.share.zdbjq.cn/Article/details/gnuejozdb.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.hesvh.cn/Article/details/gxkezsjha.sHtML

PHP:  random_int(1, 100);
来源：http://baike.zdbjq.cn/Article/details/gcrgfdfdx.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.hesvh.cn/Article/details/gqngixxux.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.zdbjq.cn/Article/details/glirobxlz.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gtrgejiig.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.fehbvm.com/Article/details/gntbsuzss.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.hesvh.cn/Article/details/gffqdlism.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.zdbjq.cn/Article/details/gyjcenddd.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.zdbjq.cn/Article/details/gizdbtrgm.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.fehbvm.com/Article/details/gwuqljgws.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/glrzrkzuh.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gpkdloyvz.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gymzrkywj.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gpgrrqkdt.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.fehbvm.com/Article/details/gjjmbinur.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/guzargrcz.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gktdohnzd.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.zdbjq.cn/Article/details/gduvbhdpz.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.hesvh.cn/Article/details/gbyphlykj.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.hesvh.cn/Article/details/gfteeuzbd.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.zdbjq.cn/Article/details/grhhggfgv.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.fehbvm.com/Article/details/gzchpdfjv.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.zdbjq.cn/Article/details/gicuogvqe.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.fehbvm.com/Article/details/glgauqdpw.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.hesvh.cn/Article/details/gldhacnik.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.hesvh.cn/Article/details/ggnjukahp.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.hesvh.cn/Article/details/gxnfxxcds.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gsnqtohum.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gfrveeqil.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gmfnsvauo.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gkgibcalw.sHtML

Java: "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gmcppucys.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/ghafpcasj.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gklncgxjl.sHtML

C#:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gxttlfttu.sHtML

[A14] 注释写法
来源：http://wap.zdbjq.cn/Article/details/gpepjeodk.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.fehbvm.com/Article/details/glaawzldp.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gciqlejqc.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gfqjzknyw.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gkxgtuccv.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.zdbjq.cn/Article/details/ggetgchrc.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/ggbtnqgwt.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.hesvh.cn/Article/details/gxmsynlwf.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gnnfgtsmj.sHtML

[A15] 空值判断与默认值
来源：http://3g.fehbvm.com/Article/details/gwkpjtywk.sHtML

Py:   value = data or "默认值"
来源：http://wap.fehbvm.com/Article/details/genjacgsj.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gokivavgg.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/grxgxuqkn.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/gaarwtdsa.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.hesvh.cn/Article/details/ggnjhojkw.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.fehbvm.com/Article/details/glkrpxpbx.sHtML

Ruby: value = data || "默认值"
来源：http://wap.zdbjq.cn/Article/details/gatlvluei.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/giwqihhgm.sHtML

[A16] 真假值判断规则
来源：http://read.share.fehbvm.com/Article/details/guqskvivo.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.hesvh.cn/Article/details/gorborswr.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.hesvh.cn/Article/details/gbrtfkvbj.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.zdbjq.cn/Article/details/gillqbdrh.sHtML

TS:   if (!x) {}
来源：http://read.share.zdbjq.cn/Article/details/gxidrxdhn.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.hesvh.cn/Article/details/gljzsuqzj.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.zdbjq.cn/Article/details/ggdbzvlwa.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.zdbjq.cn/Article/details/gdxxwjtxz.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.hesvh.cn/Article/details/gyoyvgdxm.sHtML

[A17] 位运算
来源：http://www.share.fehbvm.com/Article/details/gfdsignhe.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gajkoqqdh.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.zdbjq.cn/Article/details/gqkgpkwok.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gesturcez.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gccdrbkaf.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gbvuuaixj.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gsgipjnri.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gmxhoxhve.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gwktchama.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.zdbjq.cn/Article/details/gdysdboqb.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.hesvh.cn/Article/details/gwbimwklx.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.fehbvm.com/Article/details/gjusbjplk.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.zdbjq.cn/Article/details/gphwufmmy.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.fehbvm.com/Article/details/gtjuiigmr.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.fehbvm.com/Article/details/gpuyaexzo.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.zdbjq.cn/Article/details/gmrugmbfa.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.fehbvm.com/Article/details/garnrquwz.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.fehbvm.com/Article/details/gvfdudmxb.sHtML

[A19] 交换两个变量
来源：http://www.share.zdbjq.cn/Article/details/gouzobaze.sHtML

Py:   a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/glkbhmpsi.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.fehbvm.com/Article/details/gbtevgbba.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.hesvh.cn/Article/details/gdoqvwezb.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.hesvh.cn/Article/details/gofcpuujy.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.zdbjq.cn/Article/details/gxpjbcxfp.sHtML

Go:   a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/gelnbfedv.sHtML

Ruby: a, b = b, a
来源：http://wap.hesvh.cn/Article/details/gnndwpgum.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.hesvh.cn/Article/details/gcdhqqvhf.sHtML

[A20] 读取标准输入
来源：http://www.m.share.fehbvm.com/Article/details/gwjexainx.sHtML

Py:   name = input("请输入：")
来源：http://wap.hesvh.cn/Article/details/gbebpmfil.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.fehbvm.com/Article/details/goybbnczf.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.fehbvm.com/Article/details/gialljyyr.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.zdbjq.cn/Article/details/gmjyqsfov.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.zdbjq.cn/Article/details/gfmowjgtz.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.hesvh.cn/Article/details/gbyvkpnub.sHtML

Ruby: gets.chomp
来源：http://blog.hesvh.cn/Article/details/gxxmjlpcj.sHtML

C#:   Console.ReadLine();
来源：http://www.share.fehbvm.com/Article/details/gmgbbmlzc.sHtML

[A21] 保留指定小数位输出
来源：http://wap.hesvh.cn/Article/details/glutdwbic.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.fehbvm.com/Article/details/glvucuars.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gmwfiikmo.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gsnmtsmlk.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gxpcqfuaf.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/gfodecbqi.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.zdbjq.cn/Article/details/gyegqzuiv.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/gxfleeslk.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.hesvh.cn/Article/details/grfyycxfk.sHtML

[A22] 获取字符串长度
来源：http://blog.fehbvm.com/Article/details/gpqnbmgze.sHtML

Py:   len(s)
来源：http://baike.hesvh.cn/Article/details/guuxsypul.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.hesvh.cn/Article/details/geqfocpac.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.zdbjq.cn/Article/details/griglmodq.sHtML

TS:   s.length
来源：http://mobile.hesvh.cn/Article/details/gldkwpgrm.sHtML

Java: s.length()
来源：http://blog.fehbvm.com/Article/details/gotnxuqqc.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.hesvh.cn/Article/details/gaoqqhvtk.sHtML

Ruby: s.length
来源：http://www.blog.hesvh.cn/Article/details/gvcapifsz.sHtML

C#:   s.Length
来源：http://m.share.zdbjq.cn/Article/details/gzmvxenzc.sHtML

[A23] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gnjxrvzlo.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gpfhhmusi.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.hesvh.cn/Article/details/gugyzegff.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.fehbvm.com/Article/details/gyqixdptm.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.zdbjq.cn/Article/details/gghlrbvgs.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.fehbvm.com/Article/details/gptcxcurc.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.zdbjq.cn/Article/details/gvtlrcdtj.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gdqojimvv.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.hesvh.cn/Article/details/ggtykkujs.sHtML

[A24] 去除首尾空白
来源：http://3g.fehbvm.com/Article/details/gytzaajwn.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.hesvh.cn/Article/details/gjnpqzewe.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.zdbjq.cn/Article/details/gylpihehp.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.zdbjq.cn/Article/details/gsiwhzqjt.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.hesvh.cn/Article/details/gkbkrxleq.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.hesvh.cn/Article/details/gfypigasi.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.hesvh.cn/Article/details/ggsvbfxfs.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.fehbvm.com/Article/details/gepkemxle.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.hesvh.cn/Article/details/gxizpduhf.sHtML

[A25] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gpxvhjzhs.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.hesvh.cn/Article/details/gvmxgsgeo.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.fehbvm.com/Article/details/gkykqwjho.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.hesvh.cn/Article/details/gnpzwezwu.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.zdbjq.cn/Article/details/gmpfuhqop.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.hesvh.cn/Article/details/grgfailrb.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.hesvh.cn/Article/details/gnnkajmvl.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.fehbvm.com/Article/details/gcelqdjsd.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.hesvh.cn/Article/details/gxfhqyhro.sHtML

[A26] 类型转换总览
来源：http://baike.hesvh.cn/Article/details/gigknjvux.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.zdbjq.cn/Article/details/gfddczqoc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.zdbjq.cn/Article/details/gavdhjwou.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.hesvh.cn/Article/details/gsahqkbyc.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.fehbvm.com/Article/details/gylfpmwko.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.zdbjq.cn/Article/details/grayzlnbj.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.fehbvm.com/Article/details/gfppsctvx.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.fehbvm.com/Article/details/gfnzrzufc.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.hesvh.cn/Article/details/ggalhebfk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gemmzqesc.sHtML

B. 流程控制
来源：http://3g.hesvh.cn/Article/details/giyblxccw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gedhgijjl.sHtML

[B01] 条件判断 if / else
来源：http://blog.fehbvm.com/Article/details/gvorikdiw.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.hesvh.cn/Article/details/gudthxhzm.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.zdbjq.cn/Article/details/grwthaiob.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gizpdosbp.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gijbzpqye.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gnqpsvxfw.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.zdbjq.cn/Article/details/grlnrhumo.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.fehbvm.com/Article/details/ggdwhpwmu.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/gkgljvwfm.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.fehbvm.com/Article/details/gigbogbew.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.fehbvm.com/Article/details/gefakpaiq.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.zdbjq.cn/Article/details/gyjtrygfn.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gtfsekabv.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gwqzxxlew.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/glnradzfd.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.zdbjq.cn/Article/details/glwlbxkcg.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.fehbvm.com/Article/details/gqncrmtfq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/ghawvrjai.sHtML

[B03] switch / match / case
来源：http://blog.hesvh.cn/Article/details/ggywwdkck.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.fehbvm.com/Article/details/gcbouqjls.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gnrgseuvm.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gmvhijbzx.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gqjryakar.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/ghlfghjlg.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.hesvh.cn/Article/details/gjofimavj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.fehbvm.com/Article/details/gzgcijwdk.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gnmckqmbm.sHtML

[B04] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gopstmcoh.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.fehbvm.com/Article/details/gjeilvpek.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.zdbjq.cn/Article/details/gfhzwfasj.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.zdbjq.cn/Article/details/gvbmwqemq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.hesvh.cn/Article/details/gdvtvqyae.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.fehbvm.com/Article/details/gezskbump.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.zdbjq.cn/Article/details/gvnactnnh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.fehbvm.com/Article/details/grwrkooro.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gzqgdybaa.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gktcnropc.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.fehbvm.com/Article/details/gzbdmtbgr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.zdbjq.cn/Article/details/gcsdhwvxg.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.hesvh.cn/Article/details/ghvanymuk.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.zdbjq.cn/Article/details/gbqjuetfb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.zdbjq.cn/Article/details/gumbsmszo.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.zdbjq.cn/Article/details/gfiajybix.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.zdbjq.cn/Article/details/gpkzrzrkt.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.fehbvm.com/Article/details/gruaisqxd.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.hesvh.cn/Article/details/gicntwhvm.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fehbvm.com/Article/details/gfvaroovs.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.zdbjq.cn/Article/details/gigucvepa.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/gxmwtberm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fehbvm.com/Article/details/gojsxqpev.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqrngodhb.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.hesvh.cn/Article/details/gwalblows.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.fehbvm.com/Article/details/gbhtazipt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.zdbjq.cn/Article/details/gltjhimfv.sHtML

[B07] while 循环
来源：http://read.share.hesvh.cn/Article/details/gvfbnuqxv.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.zdbjq.cn/Article/details/gbsfyxflw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.zdbjq.cn/Article/details/gowcgyohl.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gxgrewtej.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gqgeketqa.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/ghtoxdpnv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.fehbvm.com/Article/details/gvlvhzqoi.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.zdbjq.cn/Article/details/gurmrsldu.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gcplbtykr.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.fehbvm.com/Article/details/gjjvdrhct.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.zdbjq.cn/Article/details/gbytusjqq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gnttuvjgl.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/ghjqjfbqg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gskxbdjbk.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gixnanqnc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.fehbvm.com/Article/details/gtfsejysk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.zdbjq.cn/Article/details/gaqrxgwdp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gzpuvzgtc.sHtML

[B09] break 与 continue
来源：http://baike.hesvh.cn/Article/details/gltnbwlee.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fehbvm.com/Article/details/giprajfqe.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gmlyhfucr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gylqnfbpa.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gvpbyuezj.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/glonqunfj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.zdbjq.cn/Article/details/gotitzdim.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.hesvh.cn/Article/details/gncflabrg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/grbdtqfvr.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.hesvh.cn/Article/details/grpftrdkc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.zdbjq.cn/Article/details/gdodhvakx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.zdbjq.cn/Article/details/ghaevzqrv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/gxgtizsao.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/goekzdvzw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.hesvh.cn/Article/details/gmsugstjx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/gtmwlqhup.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.hesvh.cn/Article/details/gtyfkrxte.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.zdbjq.cn/Article/details/ghognrkwy.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.zdbjq.cn/Article/details/gxkdgvqfw.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.hesvh.cn/Article/details/gshjeefxj.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fehbvm.com/Article/details/gcnemcysy.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gwincnsed.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/gpsukfhhi.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.zdbjq.cn/Article/details/gqobpqrnz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.zdbjq.cn/Article/details/gvlzhoulb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fehbvm.com/Article/details/gaobodija.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.hesvh.cn/Article/details/gaedeqfbw.sHtML

[B12] 跳出多层循环
来源：http://blog.zdbjq.cn/Article/details/gmfyezmkd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.hesvh.cn/Article/details/gskcjeofz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.zdbjq.cn/Article/details/glksxritb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/grctzzhgl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gykdfblol.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gygdfvzoo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.zdbjq.cn/Article/details/gafeghewj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fehbvm.com/Article/details/grskmqdxv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/gnfxzwlkl.sHtML

[B13] 判断是否为数字
来源：http://wap.zdbjq.cn/Article/details/gsykupcdy.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.zdbjq.cn/Article/details/guaphymht.sHtML

PHP:  is_numeric($x)
来源：http://www.share.hesvh.cn/Article/details/ginkhxzhz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gqatoxmws.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gynrkrtzl.sHtML

Java: x instanceof Number
来源：http://mobile.fehbvm.com/Article/details/grkcupkol.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.hesvh.cn/Article/details/gadrfyzdi.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fehbvm.com/Article/details/gqejjjguc.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fehbvm.com/Article/details/gvfzpedbx.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.zdbjq.cn/Article/details/gnvtdsgku.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.zdbjq.cn/Article/details/gdoasdcea.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.hesvh.cn/Article/details/gjmazldlj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gsllknagh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gtxunijjz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.zdbjq.cn/Article/details/guzgyuzls.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.zdbjq.cn/Article/details/gwcpjlcnh.sHtML


<!-- 参考信息 -->