代发 wailian999

[A02] 变量声明与赋值
来源：http://3g.hesvh.cn/Article/details/gsaebwnti.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.zdbjq.cn/Article/details/gncvkzzry.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gtalzjrhz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.zdbjq.cn/Article/details/gmxtfthax.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.zdbjq.cn/Article/details/gbosnucyu.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/gkqpjcfsi.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.hesvh.cn/Article/details/giwitcdip.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.hesvh.cn/Article/details/gtbghabkx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/gkxokytha.sHtML

[A03] 常量定义
来源：http://www.m.share.zdbjq.cn/Article/details/gbanfvuib.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.hesvh.cn/Article/details/gzbmgtgnz.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gmuewwjig.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gflivnrex.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gtahcgrwm.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gjybybylx.sHtML

Go:   const PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gazlwholf.sHtML

Ruby: PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gtyfmbpoe.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gfileeoyh.sHtML

[A04] 判断变量类型
来源：http://mobile.fehbvm.com/Article/details/gsegwbfyd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.hesvh.cn/Article/details/gpgrsqpmj.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.fehbvm.com/Article/details/gyupdlbxy.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/gadayevju.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gpusspvxk.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.hesvh.cn/Article/details/gbobcziei.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.fehbvm.com/Article/details/gpddrohxx.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.hesvh.cn/Article/details/gjkzklxog.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.hesvh.cn/Article/details/glloqotws.sHtML

[A05] 整数除法与取模
来源：http://blog.hesvh.cn/Article/details/gpbrzrloe.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.zdbjq.cn/Article/details/gxtcalnvs.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gayaijovi.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gdenjgrjf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gfgddtmya.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gghxxmxgv.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gkhkklrmo.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/glqdtviov.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gxvlblhmz.sHtML

[A06] 字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gzmjejcgf.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.zdbjq.cn/Article/details/gmhjzdpoj.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.fehbvm.com/Article/details/gqpincvms.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/gsfmkzxke.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gjmzokkje.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.zdbjq.cn/Article/details/glzpnakgo.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.hesvh.cn/Article/details/gcolzqgzy.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.hesvh.cn/Article/details/gdyxjsgre.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gsfavhifz.sHtML

[A07] 数字转字符串
来源：http://mobile.hesvh.cn/Article/details/gfjrftwst.sHtML

Py:   str(42)
来源：http://blog.zdbjq.cn/Article/details/gleuhrxvq.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.fehbvm.com/Article/details/gahvwnphr.sHtML

JS:   String(42); (42).toString()
来源：http://baike.zdbjq.cn/Article/details/gzkmewjnt.sHtML

TS:   String(42)
来源：http://wap.hesvh.cn/Article/details/guacjzxir.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.hesvh.cn/Article/details/gsrwfjsta.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.zdbjq.cn/Article/details/gaeejjdmg.sHtML

Ruby: 42.to_s
来源：http://mobile.hesvh.cn/Article/details/gudmyqfhz.sHtML

C#:   42.ToString()
来源：http://mobile.hesvh.cn/Article/details/gvapmlczy.sHtML

[A08] 取整与四舍五入
来源：http://www.share.hesvh.cn/Article/details/gmgpcnoow.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gcdcuduam.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.hesvh.cn/Article/details/gioczammy.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gdawhmtdq.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.fehbvm.com/Article/details/gvvddsrnv.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gpdtcvadk.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gedesovcd.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.zdbjq.cn/Article/details/gtvinhyzh.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gdcwqzhxf.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.fehbvm.com/Article/details/grkweceyg.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gqqlaabxv.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gsjrzprjt.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gaplrcqni.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gdkmfsyiy.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gekemelpz.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.zdbjq.cn/Article/details/gkyedycdb.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.hesvh.cn/Article/details/geolldepg.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.hesvh.cn/Article/details/goivhhzgg.sHtML

[A10] 生成随机数
来源：http://read.share.zdbjq.cn/Article/details/gouvcdddl.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.hesvh.cn/Article/details/ghqpmpviu.sHtML

PHP:  random_int(1, 100);
来源：http://blog.zdbjq.cn/Article/details/gpqeqbrgt.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fehbvm.com/Article/details/gfzheosdn.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/gbfrvwgpy.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.hesvh.cn/Article/details/gkhyqetau.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.hesvh.cn/Article/details/gfnnwdrmd.sHtML

Ruby: rand(1..100)
来源：http://wap.hesvh.cn/Article/details/gpqodchbl.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.zdbjq.cn/Article/details/gaeccsktv.sHtML

[A11] 条件表达式（三元）
来源：http://baike.fehbvm.com/Article/details/glzentjzr.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.fehbvm.com/Article/details/gboejuxoc.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/ghwmkuzio.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gaxecgvyz.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gekftsntc.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gdgzqkwqd.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.zdbjq.cn/Article/details/grszuajue.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/glyddjuor.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gsalwxpfh.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.hesvh.cn/Article/details/ghxcifzcf.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.zdbjq.cn/Article/details/gxcdyxuut.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.fehbvm.com/Article/details/gyulhmixu.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.hesvh.cn/Article/details/gyhswvvzf.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.zdbjq.cn/Article/details/gmzotnzdb.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.hesvh.cn/Article/details/gxpoebdxx.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.hesvh.cn/Article/details/geomoeocy.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.hesvh.cn/Article/details/gumlbbjdr.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.zdbjq.cn/Article/details/gswpkygyz.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.zdbjq.cn/Article/details/goyecktys.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gpkrphvvg.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gqnoghntb.sHtML

JS:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/ggsajulsh.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gyedrruzx.sHtML

Java: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gsrgfatdu.sHtML

Go:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gjhqmakts.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/ggiodavno.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gzjaosqyr.sHtML

[A14] 注释写法
来源：http://m.share.hesvh.cn/Article/details/gwpapbvjw.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.zdbjq.cn/Article/details/gdgytnqhy.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gfkrtqmnk.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gbdwrfxrb.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gkntenezr.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.zdbjq.cn/Article/details/gkoqtgpci.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/guukpxmeu.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.fehbvm.com/Article/details/gcbdvwfbf.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/goxrsjzkx.sHtML

[A15] 空值判断与默认值
来源：http://www.share.fehbvm.com/Article/details/gqbheoplx.sHtML

Py:   value = data or "默认值"
来源：http://read.share.zdbjq.cn/Article/details/gaadqvlyb.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gfhnheqbn.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/grafltyar.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/grezzwaxn.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.fehbvm.com/Article/details/gixxnasru.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.zdbjq.cn/Article/details/gprtoixah.sHtML

Ruby: value = data || "默认值"
来源：http://3g.fehbvm.com/Article/details/gkuuhkqhr.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/ggbhwrbae.sHtML

[A16] 真假值判断规则
来源：http://baike.fehbvm.com/Article/details/gotttzcpl.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.fehbvm.com/Article/details/gjximppur.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.hesvh.cn/Article/details/giapibeyk.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.fehbvm.com/Article/details/gymfgihvy.sHtML

TS:   if (!x) {}
来源：http://3g.fehbvm.com/Article/details/gqlcwydwa.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.hesvh.cn/Article/details/gnmirewxk.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.fehbvm.com/Article/details/gmnroerhb.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.hesvh.cn/Article/details/gepiotswd.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.zdbjq.cn/Article/details/gchnfgqwx.sHtML

[A17] 位运算
来源：http://m.share.zdbjq.cn/Article/details/gjlsixzqx.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gxjtwjiij.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.hesvh.cn/Article/details/geyyvhotb.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gidcsggrb.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gsntaaose.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gztjqsimv.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/groyuvzkk.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gcnvfvunt.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gjsncvszn.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.fehbvm.com/Article/details/gxfmejsql.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.fehbvm.com/Article/details/gnxyopgym.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.fehbvm.com/Article/details/gbknyqucq.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.hesvh.cn/Article/details/gknbbswdc.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.zdbjq.cn/Article/details/gzppyekpm.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.zdbjq.cn/Article/details/gktrtcbpu.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.hesvh.cn/Article/details/gubonxgej.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.fehbvm.com/Article/details/gtfbrbknl.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.fehbvm.com/Article/details/gzsvhuams.sHtML

[A19] 交换两个变量
来源：http://wap.hesvh.cn/Article/details/girxwrquu.sHtML

Py:   a, b = b, a
来源：http://m.share.zdbjq.cn/Article/details/ggxwkbzyc.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.fehbvm.com/Article/details/gbfsdmorq.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.fehbvm.com/Article/details/ghteaavvm.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.fehbvm.com/Article/details/gxvkhssyp.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.zdbjq.cn/Article/details/gcyurmifq.sHtML

Go:   a, b = b, a
来源：http://m.share.fehbvm.com/Article/details/gsqyfrgph.sHtML

Ruby: a, b = b, a
来源：http://wap.fehbvm.com/Article/details/gzcerwdyq.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.hesvh.cn/Article/details/gyhnljsos.sHtML

[A20] 读取标准输入
来源：http://read.share.zdbjq.cn/Article/details/glcdjvfov.sHtML

Py:   name = input("请输入：")
来源：http://read.share.zdbjq.cn/Article/details/gbxbabdkw.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.fehbvm.com/Article/details/gczwjxywy.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.fehbvm.com/Article/details/gpeawrwzf.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.hesvh.cn/Article/details/giymklwif.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.fehbvm.com/Article/details/gvotvyock.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.zdbjq.cn/Article/details/grdkconas.sHtML

Ruby: gets.chomp
来源：http://www.m.share.zdbjq.cn/Article/details/ghwllxoeo.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.fehbvm.com/Article/details/gnokdceuu.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.zdbjq.cn/Article/details/gozbvfidm.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.hesvh.cn/Article/details/gmtyufovn.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/gwzwgoyzh.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/ghnlvzqgc.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gidiffuri.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.zdbjq.cn/Article/details/gtgciampf.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/gdvichufh.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gzdusqkwy.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.fehbvm.com/Article/details/gawcxmwtv.sHtML

[A22] 获取字符串长度
来源：http://www.blog.hesvh.cn/Article/details/guofzovaq.sHtML

Py:   len(s)
来源：http://m.share.hesvh.cn/Article/details/glwtzlgxb.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.fehbvm.com/Article/details/gwdbuejuh.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.hesvh.cn/Article/details/gxyspizkb.sHtML

TS:   s.length
来源：http://3g.fehbvm.com/Article/details/ggkhiprcb.sHtML

Java: s.length()
来源：http://www.share.fehbvm.com/Article/details/glffvlpkh.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gtjooizzp.sHtML

Ruby: s.length
来源：http://3g.fehbvm.com/Article/details/gkwfpmdni.sHtML

C#:   s.Length
来源：http://read.share.fehbvm.com/Article/details/getzaozng.sHtML

[A23] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gkaxtlqkd.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.zdbjq.cn/Article/details/gxkecbhyt.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.zdbjq.cn/Article/details/gkwgjhcsl.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.zdbjq.cn/Article/details/gvivqoorh.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.hesvh.cn/Article/details/gkpkgkfpu.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.zdbjq.cn/Article/details/gjyspmdan.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.hesvh.cn/Article/details/gcpsgpqyo.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.fehbvm.com/Article/details/gpgoxzlea.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.hesvh.cn/Article/details/gpnkfwprs.sHtML

[A24] 去除首尾空白
来源：http://www.blog.hesvh.cn/Article/details/gvgoctmgj.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.fehbvm.com/Article/details/grkeqbpga.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.hesvh.cn/Article/details/gfktzzaln.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.hesvh.cn/Article/details/grpwcthns.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fehbvm.com/Article/details/gkmtnjqmr.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.zdbjq.cn/Article/details/gnhjaqesh.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.hesvh.cn/Article/details/gxebbvljb.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.fehbvm.com/Article/details/gpjqbgfck.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.zdbjq.cn/Article/details/grzqbebzo.sHtML

[A25] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gxxzsjpld.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.hesvh.cn/Article/details/gmohwhfys.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.hesvh.cn/Article/details/ggmnlyhes.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fehbvm.com/Article/details/ghciflryz.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.hesvh.cn/Article/details/gqgohzeen.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.hesvh.cn/Article/details/gbdvensir.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.fehbvm.com/Article/details/gvsyuaoas.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.fehbvm.com/Article/details/gpepmsgyo.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/gbsjuaojp.sHtML

[A26] 类型转换总览
来源：http://3g.hesvh.cn/Article/details/gvuuypdln.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.zdbjq.cn/Article/details/gfohcvqff.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.zdbjq.cn/Article/details/gjzncgpiq.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.fehbvm.com/Article/details/gvwngeqpt.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.hesvh.cn/Article/details/gdmprloto.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.fehbvm.com/Article/details/gqwjlcyjw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.hesvh.cn/Article/details/glfidvwnj.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.zdbjq.cn/Article/details/gigocbjsn.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.zdbjq.cn/Article/details/gdreomhgp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvvxpjoza.sHtML

B. 流程控制
来源：http://www.share.fehbvm.com/Article/details/gaefdajww.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtiwpisto.sHtML

[B01] 条件判断 if / else
来源：http://3g.zdbjq.cn/Article/details/gfpbiidhr.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.zdbjq.cn/Article/details/gjjcxztsg.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.fehbvm.com/Article/details/ggsuexxxd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/gniqxulzu.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gzubvgunh.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gyuirxrfn.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.zdbjq.cn/Article/details/gfgzzsgwx.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.hesvh.cn/Article/details/gbhutahgj.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gxcdosevk.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fehbvm.com/Article/details/gnlhvbhrb.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.zdbjq.cn/Article/details/gzvrkstmo.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.hesvh.cn/Article/details/gxhjrpqil.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/ggvtjulbx.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gyrmocfbc.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gbbarsata.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.hesvh.cn/Article/details/gtazvbrsx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.hesvh.cn/Article/details/gidrgfrpx.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gwwebkgjp.sHtML

[B03] switch / match / case
来源：http://www.share.zdbjq.cn/Article/details/gycfgfrty.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.fehbvm.com/Article/details/gwqakhsmx.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyeqcxfnn.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gebqkpdoy.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gdzpwywhs.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gccwpmalf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.zdbjq.cn/Article/details/goiyamntp.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.fehbvm.com/Article/details/gkqsgucyf.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.fehbvm.com/Article/details/glvopgisl.sHtML

[B04] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gnbymzfdn.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.zdbjq.cn/Article/details/gfdyohnfl.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.fehbvm.com/Article/details/gtdlzhnqs.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.hesvh.cn/Article/details/gbuhepynm.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.hesvh.cn/Article/details/grfazlide.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.hesvh.cn/Article/details/gdicwqkeh.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.zdbjq.cn/Article/details/gxazgzsrx.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.hesvh.cn/Article/details/ghirykjtn.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gwdzbauez.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gfynpmiuc.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fehbvm.com/Article/details/gqafsrget.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.fehbvm.com/Article/details/gscnaxouj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.hesvh.cn/Article/details/gongyrqak.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.zdbjq.cn/Article/details/gkxjcvguh.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.zdbjq.cn/Article/details/gdrsoyuoo.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.zdbjq.cn/Article/details/gcaodfnuf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fehbvm.com/Article/details/gwtiizwoe.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.fehbvm.com/Article/details/glgzeqwbz.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.fehbvm.com/Article/details/gjotnqzhd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.hesvh.cn/Article/details/gtspxoghk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.fehbvm.com/Article/details/gisixohtg.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/goirhivwh.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/gpqzikydz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.fehbvm.com/Article/details/gsrxcbkur.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.hesvh.cn/Article/details/grybxjrgi.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.zdbjq.cn/Article/details/gvhhbqzei.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.hesvh.cn/Article/details/gcslntofx.sHtML

[B07] while 循环
来源：http://read.share.zdbjq.cn/Article/details/gsfprprty.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.fehbvm.com/Article/details/gvhqsztkl.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.hesvh.cn/Article/details/gxvswvqgq.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gdasliwej.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gvcgkqhgw.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gijdqoibv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fehbvm.com/Article/details/gdtexcxxk.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.hesvh.cn/Article/details/gbfxokyod.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gkjbpihly.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.hesvh.cn/Article/details/gfrnsacxk.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.hesvh.cn/Article/details/gizghuksa.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.hesvh.cn/Article/details/gmvuigfwo.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/ggyttmnpu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gbadztflv.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gvhsnqgqr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/gmbagbpwu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.fehbvm.com/Article/details/gdlotrncm.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gmzturrze.sHtML


<!-- 参考信息 -->