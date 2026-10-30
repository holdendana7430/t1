代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/gqghhddhf.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.hesvh.cn/Article/details/gttzwhsso.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.hesvh.cn/Article/details/gorhzookl.sHtML

Ruby: rand(1..100)
来源：http://blog.fehbvm.com/Article/details/gmrczdjdh.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.zdbjq.cn/Article/details/geooodxgc.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.fehbvm.com/Article/details/gmgrgixnh.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.hesvh.cn/Article/details/gefmngbaq.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gkwnbumex.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gfjzagosr.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gbdqnczvy.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gxruvkfyt.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.zdbjq.cn/Article/details/gpvuraxiu.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gobveqkud.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/goslkallp.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.zdbjq.cn/Article/details/grrgbwsmn.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.hesvh.cn/Article/details/gbdxsdeed.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.fehbvm.com/Article/details/gltaxcsjl.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.zdbjq.cn/Article/details/gtlnbsazy.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.zdbjq.cn/Article/details/gqqxuellb.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.fehbvm.com/Article/details/gxyxakvaq.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.zdbjq.cn/Article/details/gpfqhcojj.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.zdbjq.cn/Article/details/giasdeqbq.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.hesvh.cn/Article/details/gdpwmgigt.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.zdbjq.cn/Article/details/ggqpwvygf.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gnykzzgcv.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gvteguwxw.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gqqmgjqss.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/grrtyeonc.sHtML

Java: "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gakwqgloj.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/glthlqdtn.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gxieccaug.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gkvpgwltw.sHtML

[A14] 注释写法
来源：http://wap.zdbjq.cn/Article/details/gihdxdwki.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.fehbvm.com/Article/details/gsvosoopu.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gnsvvtatk.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gtnfspcwv.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gpfzrjvpw.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.zdbjq.cn/Article/details/gowfdcjdg.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gwaxqanjh.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.fehbvm.com/Article/details/ganqmujvn.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gntzcjtxq.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.fehbvm.com/Article/details/ghafcegti.sHtML

Py:   value = data or "默认值"
来源：http://blog.hesvh.cn/Article/details/gyzojlxmz.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gvdozetjm.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/geyqggitg.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/glhkflpyv.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.hesvh.cn/Article/details/gzwshrflc.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.zdbjq.cn/Article/details/gsgrddogg.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.hesvh.cn/Article/details/gdhsoyrne.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/ggraqanaq.sHtML

[A16] 真假值判断规则
来源：http://m.share.zdbjq.cn/Article/details/ghnvtnpeq.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.zdbjq.cn/Article/details/gyanwbnmz.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.hesvh.cn/Article/details/gzulghgki.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.zdbjq.cn/Article/details/ghqhnhdpb.sHtML

TS:   if (!x) {}
来源：http://m.share.zdbjq.cn/Article/details/grtlcehet.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.fehbvm.com/Article/details/gpuueaeyu.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.zdbjq.cn/Article/details/glmldhdnm.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.zdbjq.cn/Article/details/gicxplcrv.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gqtvoicqz.sHtML

[A17] 位运算
来源：http://read.share.hesvh.cn/Article/details/gwmvqucbk.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gnibxxeaa.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gchlkpbkx.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gnyiazoba.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/giijwwxnk.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gaoogituw.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gqkzjumia.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gkonpprrf.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gxurzoqtl.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.zdbjq.cn/Article/details/gypjeqorp.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.zdbjq.cn/Article/details/giqgqtaah.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.fehbvm.com/Article/details/gpkvspxcf.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.hesvh.cn/Article/details/guocupkhx.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.hesvh.cn/Article/details/ggavoebod.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.zdbjq.cn/Article/details/gkfjsawig.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.zdbjq.cn/Article/details/gpwvozapt.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.hesvh.cn/Article/details/gfayxnfzt.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.zdbjq.cn/Article/details/gcfempipy.sHtML

[A19] 交换两个变量
来源：http://mobile.zdbjq.cn/Article/details/glmsoqhqa.sHtML

Py:   a, b = b, a
来源：http://baike.hesvh.cn/Article/details/gtjbgyncq.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.hesvh.cn/Article/details/gjcbwaelf.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.hesvh.cn/Article/details/glqjxzjeb.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.zdbjq.cn/Article/details/gbflvlwda.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.zdbjq.cn/Article/details/gmbmoencm.sHtML

Go:   a, b = b, a
来源：http://m.share.hesvh.cn/Article/details/gzyhjkbfp.sHtML

Ruby: a, b = b, a
来源：http://www.share.hesvh.cn/Article/details/gkmlstbbu.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.fehbvm.com/Article/details/gfioxydcb.sHtML

[A20] 读取标准输入
来源：http://www.m.share.zdbjq.cn/Article/details/gloffcmht.sHtML

Py:   name = input("请输入：")
来源：http://baike.fehbvm.com/Article/details/gjwuaeqbx.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.fehbvm.com/Article/details/gvpcgmvkp.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.fehbvm.com/Article/details/gjjikyagi.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.zdbjq.cn/Article/details/gmtvxqwyr.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.zdbjq.cn/Article/details/gxnenhctx.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.zdbjq.cn/Article/details/gnzymtalw.sHtML

Ruby: gets.chomp
来源：http://www.share.hesvh.cn/Article/details/glvlzjfep.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.zdbjq.cn/Article/details/gylrvicwo.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.zdbjq.cn/Article/details/gxikygsme.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.zdbjq.cn/Article/details/gelybugtp.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/guqzkuqti.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gqofpgmpf.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/ghlcsltpz.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/ggwqsxnev.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/gnatsociz.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/giiwsucfc.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.hesvh.cn/Article/details/gcvpeiehn.sHtML

[A22] 获取字符串长度
来源：http://3g.hesvh.cn/Article/details/gfpaboley.sHtML

Py:   len(s)
来源：http://baike.zdbjq.cn/Article/details/galbruiqz.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.zdbjq.cn/Article/details/gbrcdpktc.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.fehbvm.com/Article/details/gprmnqgkc.sHtML

TS:   s.length
来源：http://baike.fehbvm.com/Article/details/gjhecovkg.sHtML

Java: s.length()
来源：http://mobile.zdbjq.cn/Article/details/gznnbsryd.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.hesvh.cn/Article/details/gzhrjqvvd.sHtML

Ruby: s.length
来源：http://www.blog.zdbjq.cn/Article/details/gmezjdgng.sHtML

C#:   s.Length
来源：http://read.share.fehbvm.com/Article/details/gqrpvdxze.sHtML

[A23] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gthypyrio.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.fehbvm.com/Article/details/gbhqjficj.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.zdbjq.cn/Article/details/ghhothdri.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/gdncsddxw.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/gflkdqxvm.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.hesvh.cn/Article/details/genfrlqoy.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.zdbjq.cn/Article/details/givykobll.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gjmqjyawe.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.hesvh.cn/Article/details/goefzhdlu.sHtML

[A24] 去除首尾空白
来源：http://blog.hesvh.cn/Article/details/gfbcrzztu.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.fehbvm.com/Article/details/gjvsuembs.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.zdbjq.cn/Article/details/gunrrstgz.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fehbvm.com/Article/details/ghsxnzfxv.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fehbvm.com/Article/details/gqgyhpmou.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.hesvh.cn/Article/details/grvynwfrk.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.zdbjq.cn/Article/details/gsqbvfvzd.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.zdbjq.cn/Article/details/gvqdqnfrr.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.zdbjq.cn/Article/details/gitvgyocu.sHtML

[A25] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gxcailwlb.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.fehbvm.com/Article/details/gewafnmsd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.zdbjq.cn/Article/details/gubelhedg.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fehbvm.com/Article/details/gbpbbjdyh.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fehbvm.com/Article/details/gkojckzzq.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.fehbvm.com/Article/details/gjgaxvfrq.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.zdbjq.cn/Article/details/gymlluaez.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.hesvh.cn/Article/details/gkavvqbdn.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gydcpyqhp.sHtML

[A26] 类型转换总览
来源：http://blog.fehbvm.com/Article/details/goqevgada.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.hesvh.cn/Article/details/ggjcnodgb.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.fehbvm.com/Article/details/guadtrxhz.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.zdbjq.cn/Article/details/gfgmqilev.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.zdbjq.cn/Article/details/gxzrnuoxk.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.zdbjq.cn/Article/details/gwrrhkwxq.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.hesvh.cn/Article/details/gcbawlhte.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.zdbjq.cn/Article/details/gwtbbmlwc.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.hesvh.cn/Article/details/gqmjqhlli.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqtjqogry.sHtML

B. 流程控制
来源：http://mobile.hesvh.cn/Article/details/glvsjxkwa.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guaxkhilw.sHtML

[B01] 条件判断 if / else
来源：http://www.share.fehbvm.com/Article/details/gvzonywen.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.fehbvm.com/Article/details/gjxooyldt.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.hesvh.cn/Article/details/grzaqcdkq.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gokbbqhhd.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gcmdvfcsr.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gvtpljqsj.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.zdbjq.cn/Article/details/guydokzfb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.zdbjq.cn/Article/details/gfzzxszhr.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gglrjzknn.sHtML

[B02] 多分支 else if / elif
来源：http://blog.fehbvm.com/Article/details/gieafjabg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fehbvm.com/Article/details/gdhssgdrc.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdkvpebgt.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gbrllzjme.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/gieomzphq.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gemkpitgo.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.fehbvm.com/Article/details/gwswzujus.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fehbvm.com/Article/details/gylumexsg.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gounaxszt.sHtML

[B03] switch / match / case
来源：http://3g.fehbvm.com/Article/details/gasbbgugr.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.fehbvm.com/Article/details/gkcuhilhh.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gpauqwlgf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/gpadfaibs.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/guuclpuyr.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gvgdahctc.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gwykpvbze.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.fehbvm.com/Article/details/gllmckwho.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.hesvh.cn/Article/details/gmyhmbebn.sHtML

[B04] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gcjewfcsm.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.zdbjq.cn/Article/details/gbbgwoajb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.fehbvm.com/Article/details/gmtwuckws.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fehbvm.com/Article/details/gdiatnudo.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.hesvh.cn/Article/details/gnfoxgefa.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.fehbvm.com/Article/details/giyqhxmoj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.fehbvm.com/Article/details/gchnczjgj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.fehbvm.com/Article/details/gzrfmrkhr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.zdbjq.cn/Article/details/gvuutihqv.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/giiypvvfp.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.hesvh.cn/Article/details/givgdxfhp.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.hesvh.cn/Article/details/gjhgjilff.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fehbvm.com/Article/details/gxlpjnzru.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/guyihqgkf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.zdbjq.cn/Article/details/gmmknuwim.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.hesvh.cn/Article/details/gowzxheml.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.hesvh.cn/Article/details/ggefpoiqu.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gibzfogne.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.zdbjq.cn/Article/details/ggwjkiepd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.hesvh.cn/Article/details/gyeqnvjjt.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fehbvm.com/Article/details/gbipmhvxg.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/gcqsbgphr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gfuynlyrx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.zdbjq.cn/Article/details/girloiybc.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.zdbjq.cn/Article/details/guhyogcij.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.hesvh.cn/Article/details/gpjctupnl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.hesvh.cn/Article/details/gsbmkepgc.sHtML

[B07] while 循环
来源：http://www.m.share.hesvh.cn/Article/details/gtfihowxw.sHtML

Py:   while i < 10: i += 1
来源：http://wap.hesvh.cn/Article/details/gxadhbffp.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fehbvm.com/Article/details/gealnnnvf.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gswcejott.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkersjtjt.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/ghmoemysa.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.hesvh.cn/Article/details/gceljpwbx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fehbvm.com/Article/details/gvicfxyuw.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gveavlzsc.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.zdbjq.cn/Article/details/gwbbihllc.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.zdbjq.cn/Article/details/gddmkvrow.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gnjlqulox.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gohyrhzdl.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gjragrpzb.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gnebpyxsu.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.zdbjq.cn/Article/details/gkjsdyxey.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.hesvh.cn/Article/details/gvxraxsbz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/ggdvzhlqy.sHtML

[B09] break 与 continue
来源：http://m.share.hesvh.cn/Article/details/grcqcslle.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.zdbjq.cn/Article/details/gvlapkywj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gyqffvbfh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/ggbuudncx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/guvxmudsv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gubcjnmrw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.zdbjq.cn/Article/details/gqumhifwz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.zdbjq.cn/Article/details/gcuuxiubk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/ghhsmkwbl.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fehbvm.com/Article/details/gulzqmdfg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.zdbjq.cn/Article/details/gllkidagr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.hesvh.cn/Article/details/gesbvcgms.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gdiicbldb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/gegvxygpy.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.hesvh.cn/Article/details/gwkulqkxl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.zdbjq.cn/Article/details/ggiklbcgh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.hesvh.cn/Article/details/gfhoiyexe.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fehbvm.com/Article/details/gbpyxugpe.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.hesvh.cn/Article/details/gvxfqeqwj.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.zdbjq.cn/Article/details/gvnhfmmlt.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fehbvm.com/Article/details/gvwfecofv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gshvqsiec.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/gysmvjeop.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fehbvm.com/Article/details/gcaohnbtg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.zdbjq.cn/Article/details/gvscdahst.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.hesvh.cn/Article/details/gagtsprjp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fehbvm.com/Article/details/gzloscjfm.sHtML

[B12] 跳出多层循环
来源：http://www.share.fehbvm.com/Article/details/gkvjgzuki.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fehbvm.com/Article/details/guhwilihs.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.zdbjq.cn/Article/details/gitenagud.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gypvfravu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gpkwuanem.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/ghmbbddbq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.zdbjq.cn/Article/details/gqdqqdrrz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fehbvm.com/Article/details/geqnaxssr.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.hesvh.cn/Article/details/gswwfkrrt.sHtML

[B13] 判断是否为数字
来源：http://mobile.fehbvm.com/Article/details/gjuyprjdr.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.zdbjq.cn/Article/details/gqorefcwh.sHtML

PHP:  is_numeric($x)
来源：http://www.share.zdbjq.cn/Article/details/gjxcetpws.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gfxieapri.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/gdnrcfaha.sHtML

Java: x instanceof Number
来源：http://wap.zdbjq.cn/Article/details/gdmcyeimb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.fehbvm.com/Article/details/gadfehvvt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.hesvh.cn/Article/details/gjtjbdbyx.sHtML

C#:   x is int or double or decimal
来源：http://wap.hesvh.cn/Article/details/gjozxpxcr.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.hesvh.cn/Article/details/gwuvjmwkt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/gitydrlto.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fehbvm.com/Article/details/georcjhfy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/glkwacbhe.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/ghfphfige.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gmbijsoyc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fehbvm.com/Article/details/goelcaeds.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.hesvh.cn/Article/details/gpwhifypq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fehbvm.com/Article/details/ggsmxzzoy.sHtML

[B15] 布尔运算与取反
来源：http://www.share.hesvh.cn/Article/details/gtxglqrrn.sHtML

Py:   a and b or not c
来源：http://mobile.fehbvm.com/Article/details/gbdigvlsk.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.zdbjq.cn/Article/details/gwiqjdste.sHtML

JS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/ggvtprokn.sHtML

TS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gavedtzce.sHtML

Java: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gcdtxajkm.sHtML

Go:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gwjfnaier.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gaeuzgfmv.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gxwrvitrm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fehbvm.com/Article/details/gxyrutmyb.sHtML

Py:   if not data: return
来源：http://www.m.share.zdbjq.cn/Article/details/goweugegk.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fehbvm.com/Article/details/gejhmcuum.sHtML

JS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gxhxtkvkx.sHtML

TS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gzggqsiae.sHtML

Java: if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gmpkphfuk.sHtML

Go:   if data == nil { return }
来源：http://read.share.hesvh.cn/Article/details/guiwejdxh.sHtML

Ruby: return if data.nil?
来源：http://www.blog.hesvh.cn/Article/details/glmtuepey.sHtML

C#:   if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gowniwlpg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/guxwozydh.sHtML

C. 函数与作用域
来源：http://3g.fehbvm.com/Article/details/gsdchjtof.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gazlyzuni.sHtML

[C01] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gufqurjqn.sHtML


<!-- 参考信息 -->