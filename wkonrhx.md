代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gpmlaqyzg.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.hesvh.cn/Article/details/gphwivitv.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gxanapyvc.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.fehbvm.com/Article/details/goemtyfkm.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gyitkrtun.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gybkmuxmy.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.fehbvm.com/Article/details/gwzrabsbn.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.hesvh.cn/Article/details/gvcfclzvg.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/geymjroqt.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.fehbvm.com/Article/details/gpuofgkig.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.hesvh.cn/Article/details/guummdjch.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gjkgvyisc.sHtML

[A10] 生成随机数
来源：http://www.m.share.fehbvm.com/Article/details/gybezyhtg.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.hesvh.cn/Article/details/gnvkprnhl.sHtML

PHP:  random_int(1, 100);
来源：http://baike.fehbvm.com/Article/details/goymmueok.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fehbvm.com/Article/details/gcfsyluzm.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.hesvh.cn/Article/details/giobbulxl.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.fehbvm.com/Article/details/gjtuoklty.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.zdbjq.cn/Article/details/gidyvkral.sHtML

Ruby: rand(1..100)
来源：http://baike.zdbjq.cn/Article/details/gdfyboezr.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.hesvh.cn/Article/details/geegrrswq.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.zdbjq.cn/Article/details/gccksygbr.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.fehbvm.com/Article/details/gooorwgma.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gkppjvqfg.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gnbtfvvcr.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gqkmihehf.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gqrwwlbdh.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.hesvh.cn/Article/details/gdcachmxc.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gxxstoecf.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gekldpmcy.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.hesvh.cn/Article/details/gbcaxixyu.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.fehbvm.com/Article/details/gjttatbrk.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.hesvh.cn/Article/details/gdfjptixo.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.hesvh.cn/Article/details/gklinbwns.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/gunyakuxz.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.hesvh.cn/Article/details/gdvssxupl.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.hesvh.cn/Article/details/grndcubll.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.hesvh.cn/Article/details/ghclrvqim.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/gqzsyeigh.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.fehbvm.com/Article/details/gdasohdkp.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gqdzeiqpc.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gbqopslbm.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gfmxpkjfi.sHtML

TS:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gvglsvijz.sHtML

Java: "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gktjxicqz.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gwmodlhiy.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gyanoqxql.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gtkfsvejz.sHtML

[A14] 注释写法
来源：http://mobile.fehbvm.com/Article/details/gsijxwsgf.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.zdbjq.cn/Article/details/gioleswdg.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/ghcmctvxd.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gkyquytpt.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gdieeymsg.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.hesvh.cn/Article/details/gbiefgcpy.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/ggacbmhtb.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fehbvm.com/Article/details/gyzygyanu.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gbqbidmah.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.fehbvm.com/Article/details/gejphpwqs.sHtML

Py:   value = data or "默认值"
来源：http://baike.zdbjq.cn/Article/details/ghidzejxz.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gcqzfkjzm.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/gnykgxgst.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gdjtchcct.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.zdbjq.cn/Article/details/gacumhoxb.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.fehbvm.com/Article/details/gjcamihjj.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.hesvh.cn/Article/details/gizndstrd.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gnmxelbnn.sHtML

[A16] 真假值判断规则
来源：http://3g.fehbvm.com/Article/details/ghkqrocub.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.zdbjq.cn/Article/details/gzvhtqaew.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.fehbvm.com/Article/details/ghnngptsg.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.zdbjq.cn/Article/details/gwoijjcrj.sHtML

TS:   if (!x) {}
来源：http://www.share.hesvh.cn/Article/details/gdgfxqlkz.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.fehbvm.com/Article/details/grksrhuzv.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.fehbvm.com/Article/details/gphwdyuhg.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.fehbvm.com/Article/details/gdzgwkduj.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.hesvh.cn/Article/details/gggpxpddp.sHtML

[A17] 位运算
来源：http://read.share.hesvh.cn/Article/details/gusdbnkus.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gapaetmgd.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/grszyzmhu.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gypnenlag.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gfgqylckn.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/goxbbvmgw.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gtrlxzgpw.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/ghovarblw.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gtpojxiak.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.zdbjq.cn/Article/details/gqwyxxpnc.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.hesvh.cn/Article/details/gtznmcnqj.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.zdbjq.cn/Article/details/gbfizezsj.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.fehbvm.com/Article/details/gafzjnsuj.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.hesvh.cn/Article/details/guibfidcq.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.hesvh.cn/Article/details/gmkqrjwkw.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.hesvh.cn/Article/details/guuaauhgi.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.zdbjq.cn/Article/details/gxupqjcqs.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.fehbvm.com/Article/details/gclbaonba.sHtML

[A19] 交换两个变量
来源：http://read.share.zdbjq.cn/Article/details/guuoxhvvw.sHtML

Py:   a, b = b, a
来源：http://wap.fehbvm.com/Article/details/gpnesnxof.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.zdbjq.cn/Article/details/gldzctcsc.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.hesvh.cn/Article/details/giabrjyjj.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.fehbvm.com/Article/details/giipvfvjm.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.hesvh.cn/Article/details/gozczahcv.sHtML

Go:   a, b = b, a
来源：http://blog.zdbjq.cn/Article/details/ggrghnksa.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/gdnryrmfm.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.hesvh.cn/Article/details/gpmsglxdm.sHtML

[A20] 读取标准输入
来源：http://blog.hesvh.cn/Article/details/gzzjktkgw.sHtML

Py:   name = input("请输入：")
来源：http://mobile.hesvh.cn/Article/details/gcinohdjh.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.zdbjq.cn/Article/details/grnvsfzyz.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.fehbvm.com/Article/details/ggknxvpbc.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gxogidhgu.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.hesvh.cn/Article/details/gbabibvdi.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.fehbvm.com/Article/details/gxwgyuvvg.sHtML

Ruby: gets.chomp
来源：http://blog.hesvh.cn/Article/details/gguxmdbqf.sHtML

C#:   Console.ReadLine();
来源：http://wap.fehbvm.com/Article/details/gsrodpdpn.sHtML

[A21] 保留指定小数位输出
来源：http://baike.zdbjq.cn/Article/details/gtsorboak.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.hesvh.cn/Article/details/gtlitprvh.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.zdbjq.cn/Article/details/gpbujvqhe.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gmfzgujxe.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gvhmdrfrl.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/gxtrulrqc.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/gpmunfwvs.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gyschqetx.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.fehbvm.com/Article/details/gsewclqsp.sHtML

[A22] 获取字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gyjwekiby.sHtML

Py:   len(s)
来源：http://www.blog.hesvh.cn/Article/details/guiazoitf.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.hesvh.cn/Article/details/goeqvxbat.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.fehbvm.com/Article/details/gmynvgikh.sHtML

TS:   s.length
来源：http://baike.fehbvm.com/Article/details/gcfmcwxpd.sHtML

Java: s.length()
来源：http://mobile.zdbjq.cn/Article/details/gtmnmejnp.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gcjauhvpm.sHtML

Ruby: s.length
来源：http://read.share.fehbvm.com/Article/details/giisqzjkg.sHtML

C#:   s.Length
来源：http://3g.hesvh.cn/Article/details/gixvmlzue.sHtML

[A23] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gjsbgiasw.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.zdbjq.cn/Article/details/gboomfzpw.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.hesvh.cn/Article/details/gdxsrrlcd.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.hesvh.cn/Article/details/gsekzyonw.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.zdbjq.cn/Article/details/gdadxkjpf.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/gcptvyhfu.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.fehbvm.com/Article/details/gglqpcviz.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gjnwobcci.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.fehbvm.com/Article/details/gypebodph.sHtML

[A24] 去除首尾空白
来源：http://m.share.zdbjq.cn/Article/details/glnuawgxv.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.zdbjq.cn/Article/details/ghcniobow.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.fehbvm.com/Article/details/guftltufd.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.hesvh.cn/Article/details/guhmixhbq.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/gtpwfontp.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.zdbjq.cn/Article/details/gukkblhcv.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.hesvh.cn/Article/details/gxgvrguna.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.fehbvm.com/Article/details/gbbigdsdd.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.fehbvm.com/Article/details/ggocyeecp.sHtML

[A25] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/guxdttvjh.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.zdbjq.cn/Article/details/gesteuiru.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.zdbjq.cn/Article/details/gchlaosgg.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.hesvh.cn/Article/details/grxlyrnao.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.hesvh.cn/Article/details/gytwstfes.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.fehbvm.com/Article/details/gcmclljja.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.hesvh.cn/Article/details/gxqhsoxhu.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.zdbjq.cn/Article/details/glukjglpa.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/gehfpkpbq.sHtML

[A26] 类型转换总览
来源：http://www.share.zdbjq.cn/Article/details/gemjhqvtx.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.zdbjq.cn/Article/details/gzmkrhajy.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.hesvh.cn/Article/details/glmexxaff.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.hesvh.cn/Article/details/gyssbclhj.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.fehbvm.com/Article/details/gzwlkhsnd.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.fehbvm.com/Article/details/gaeqgbnqn.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.fehbvm.com/Article/details/gfbupnhux.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.fehbvm.com/Article/details/geqdffwdh.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.hesvh.cn/Article/details/golyzwxoj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxvexqqfp.sHtML

B. 流程控制
来源：http://www.share.zdbjq.cn/Article/details/gtdvkfzgl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gimlcatcb.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.zdbjq.cn/Article/details/gjpkpnzdp.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.zdbjq.cn/Article/details/gkruztrrz.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.hesvh.cn/Article/details/gyyxrbisg.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gmidywhme.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/glmzkhamx.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gvokhrhbg.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.hesvh.cn/Article/details/gyuwdajfw.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.fehbvm.com/Article/details/gpdxhyfsy.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/gahipdfmj.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.hesvh.cn/Article/details/gzipulqco.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.hesvh.cn/Article/details/gjdsiylwk.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.zdbjq.cn/Article/details/gabmzmavc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gdrbpsddw.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gtwactidq.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gplitcgmh.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.fehbvm.com/Article/details/gmfogavcx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.zdbjq.cn/Article/details/ghctzmpko.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gzbxzipdj.sHtML

[B03] switch / match / case
来源：http://www.share.hesvh.cn/Article/details/gskukbwsw.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.fehbvm.com/Article/details/gklvesglp.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gceukfgra.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gpvsiugcy.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpvlfoitp.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnlvlydsl.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gduzaatnn.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.hesvh.cn/Article/details/ggkragckv.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gkxjgbqvy.sHtML

[B04] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gxewdgccc.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.fehbvm.com/Article/details/gqbqozenn.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.fehbvm.com/Article/details/gponmapai.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fehbvm.com/Article/details/gdfpikeja.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.zdbjq.cn/Article/details/glqjghxmm.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.hesvh.cn/Article/details/gkltuvigb.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.hesvh.cn/Article/details/gqnscpehm.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.hesvh.cn/Article/details/gaqqssyrf.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.zdbjq.cn/Article/details/gfhnzurfa.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/ggbjmuhxl.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.hesvh.cn/Article/details/girqeacov.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.fehbvm.com/Article/details/gbysrhxiq.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gqjxrnrtf.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/grisjmsfs.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.zdbjq.cn/Article/details/gskkaroui.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.fehbvm.com/Article/details/graqecflh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.zdbjq.cn/Article/details/gtfourdih.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.fehbvm.com/Article/details/ghghtmlig.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.fehbvm.com/Article/details/gxmghfvfb.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.fehbvm.com/Article/details/gscssaogw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.zdbjq.cn/Article/details/gfqujnuwt.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/ganxmyysg.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/giqqqwmzy.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.hesvh.cn/Article/details/guutwghvn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.zdbjq.cn/Article/details/gkoeexgps.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.hesvh.cn/Article/details/guyowiorh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.fehbvm.com/Article/details/gtqtcrcny.sHtML

[B07] while 循环
来源：http://www.share.fehbvm.com/Article/details/gpkyedqpf.sHtML

Py:   while i < 10: i += 1
来源：http://baike.hesvh.cn/Article/details/gwurkzope.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.fehbvm.com/Article/details/gnfmnqqrd.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gkkfosnsw.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gwzckwtur.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gckbweqhi.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.hesvh.cn/Article/details/gblfysfyr.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.hesvh.cn/Article/details/ghalmsjjn.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/grcnfkkvz.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fehbvm.com/Article/details/ghzxiwgfc.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fehbvm.com/Article/details/ghwakzcxz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gzadzawcu.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gtpxvmudc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gfmzeeyvk.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gqmcmuqvy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.zdbjq.cn/Article/details/guzeublfg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.hesvh.cn/Article/details/gpjtuftcg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gspjdmyje.sHtML

[B09] break 与 continue
来源：http://www.share.fehbvm.com/Article/details/glzpmwove.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fehbvm.com/Article/details/gbqbtaonu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gszacbacp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gljdeewai.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gghidvqoo.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gclddfdgj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.zdbjq.cn/Article/details/gzikhkxkp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fehbvm.com/Article/details/gbvqeeudw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/ghgtqcpyx.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.zdbjq.cn/Article/details/grmslexgk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fehbvm.com/Article/details/gcgyzauiw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.hesvh.cn/Article/details/gvutacgoj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/ggmjppgsf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gzjnifqih.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.zdbjq.cn/Article/details/gofxtungo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.fehbvm.com/Article/details/gnejqkmwh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.hesvh.cn/Article/details/gcukqzwpl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fehbvm.com/Article/details/gqcjveswu.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.zdbjq.cn/Article/details/gtmxacgzu.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fehbvm.com/Article/details/ganbklraq.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.fehbvm.com/Article/details/gwdacvsgz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/ginuakgez.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gkdwufvpp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.zdbjq.cn/Article/details/gkjxqpgsq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.zdbjq.cn/Article/details/gsdvgmkhl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fehbvm.com/Article/details/gqaadxrxw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.zdbjq.cn/Article/details/gdhigimtn.sHtML

[B12] 跳出多层循环
来源：http://www.share.hesvh.cn/Article/details/ghtgepniv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.hesvh.cn/Article/details/gyksamopi.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.zdbjq.cn/Article/details/gparcmqik.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gnmskinot.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gzpudojij.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/grooojlsy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.zdbjq.cn/Article/details/gyuyuczso.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fehbvm.com/Article/details/giciqlnjt.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.hesvh.cn/Article/details/gvrjvxdki.sHtML

[B13] 判断是否为数字
来源：http://baike.zdbjq.cn/Article/details/gtjdgcvke.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/gvfxtiigs.sHtML

PHP:  is_numeric($x)
来源：http://www.share.hesvh.cn/Article/details/glecfeogi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/gupckvuqb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gjurupehj.sHtML

Java: x instanceof Number
来源：http://3g.zdbjq.cn/Article/details/glzibfihj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.zdbjq.cn/Article/details/gcyudqkls.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.hesvh.cn/Article/details/goqoijpar.sHtML

C#:   x is int or double or decimal
来源：http://blog.fehbvm.com/Article/details/gwfuarwlv.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.hesvh.cn/Article/details/gzcpvslqj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.hesvh.cn/Article/details/gfldgweoq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.hesvh.cn/Article/details/glsoqbudz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gghdtkddb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/ganlqwmee.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/gyvcoqkad.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.zdbjq.cn/Article/details/goiqpuoie.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.fehbvm.com/Article/details/grzzukjsx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fehbvm.com/Article/details/glcqitwhd.sHtML

[B15] 布尔运算与取反
来源：http://baike.fehbvm.com/Article/details/gnhahvvuk.sHtML

Py:   a and b or not c
来源：http://baike.fehbvm.com/Article/details/gzozatpqb.sHtML

PHP:  $a && $b || !$c
来源：http://baike.zdbjq.cn/Article/details/gpbrbvidh.sHtML

JS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gjxedjnyk.sHtML

TS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gyjycppxy.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gtdjmyzxq.sHtML


<!-- 参考信息 -->