代发 wailian999

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2tgeaxemk.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2doiudefd.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2bfzcfbjc.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hhuodaos.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2rzmdqgvs.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2wsorhqef.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2nixffydy.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ytejcoxd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2atvvlfya.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hyjespph.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rlkhmeww.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wlizqfio.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jetwhxjq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2lxgpuoob.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2thbmxikl.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fecqviqv.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2caaljpbz.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2evbulqkq.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2navpgpqx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2vhfiabup.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2tfseogll.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2bkvgfkfe.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2dlzgbohi.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2wlderysk.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2fyfksbdp.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2gzhoblwa.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2omssokcl.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2veraengi.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mkxbudbz.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vhdyxajm.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zpvtptpo.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2iryemvzz.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qggdtaae.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hwcgcfnk.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2prdlcivt.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2mwwbdhvg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2apncvetc.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2muwfgqcl.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2fjhyjktb.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2pxfwlnaz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2lnhdhlik.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2iskupuqb.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2daviryci.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2ykbweurb.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2szwhmmgq.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ehivobck.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fucfisye.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yfcnfmcd.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bmpznpgr.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wctdvxai.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2sbplaoed.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wyfbdpsw.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2chnwtzgk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2gtvovwrc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vxnlauso.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jizgrlpr.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jvpoykhe.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2viksecqt.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zimovzts.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2hbqbnlui.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2uxunpysb.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2aptevvkv.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2rqqusnnr.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2tgqhldmu.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2mkppplbu.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qdjfnymi.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2iartyqje.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2msjhlfhg.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2wjbwlchv.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2lfmyfypl.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2rbvqcgkc.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2oyaqwxue.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2iyavsuyx.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2rbhkdoqp.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pnipuhdh.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2qtkahymy.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2okmtvvdn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2uwnclyll.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lpikuaoc.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2hnylqrdg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jrjkmsoo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cwvtygme.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2sugycnwf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wixoqyyv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ikwpuibq.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2neakunvr.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2iywslrtw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2meivhiba.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2kwefqhuk.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ckyuxolo.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2tcvdktso.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2pyiuvtpz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2vqafczmj.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2bwuthcaf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2wagvjmyu.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2qlkqlzcb.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2dejrepju.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2totghfyy.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2vvrimdty.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2ezdayiah.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2kycfvgeu.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2juusjvkv.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2dfexwdeq.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2qdybwfye.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2mcabtzhc.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2axyxznrf.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2czlxeomp.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2uqivmich.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2gnapaljk.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2sjkovtev.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2nqbvjaik.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2komecxzk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2eppsqlxu.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2dprftgnd.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2osshckci.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2zrgszebe.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2ejoxdoch.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mfxgmgrs.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2uzebjevc.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ulmgxlsj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2fwgtinkz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ltxgside.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2htldmqur.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2kgcatlli.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ywganpoj.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2ykcvxdeh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2lydwhvec.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2itfwzfai.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2ypghoesn.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wrpteolb.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2lcgehful.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2vnssqgfo.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tgfwjvxh.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ncjkdnev.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ajqtdnnw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2wjoiibfq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2xiqpldeo.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2chylcfer.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2fohmvaaq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vlnwuemm.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2opvgkiqj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2lpnptxej.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2mlwkoylf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2olfamquo.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2sicnaqcp.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2keahopsl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2dxebodlb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2tasoplff.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2bjfakqdf.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2yxijrpdp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2brpberit.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2obzhesgx.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2rdsasyha.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2uplxdscc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2begrqrav.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2pcrhkwyo.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2jmuqufiq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zxjgobwv.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2vpoekyau.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ttgtgpvm.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2brcbmkby.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2vhxiutku.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2wxkjioim.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2iwpxxyot.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2tifwihlg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2dyciomvc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2khshdweo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nmwrwukw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ynoxjjvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wfnnjdki.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2yxivqfvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eostrgkv.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2omdefgeq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2lsnawmve.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjxqlzxg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2satmuvzt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cegsinud.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qkcksdfg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2acpxghwi.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2gdvofvjh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ppywrqtn.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2yflycibz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2bboksgjt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bquvprrm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2uofhvbsc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zftzxaep.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nbvkwjsl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2yliojfen.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2tbiopldm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tatdcuvc.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2wtxbsfmd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2gqanbeia.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kqkcayec.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zlkrhyhp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fidwqqef.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2emksndhq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2gxmisrdi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2eaxptcon.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2kdcflnnz.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2djjyojkj.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2rojfurlm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2sdzoaldu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2swakcetk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2shyifpvy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2gwppoddu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2axzfunuz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2kieewirw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2okwyflcz.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ddcrujog.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2zogojtux.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzlyacxa.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2winunsvi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2epfiorst.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2qucxjbwl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2lacxclol.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2uhxwwebw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2syarfhxg.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2docnyezy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2xdojzjbn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivmcnlpi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2fablvfmk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2akmmuian.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2qhxhgphb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2imqaahbe.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2thjzizgh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2xwxhrbov.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2isytptvl.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2lkyljkzo.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2zmeemkly.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ajbcypkf.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ycjwdrmi.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtlnlifh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2jdfknaxt.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2svsfylex.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lteabyxl.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2zmfdnwhw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2tofiraqb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dtdkxyaj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2owexzmay.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kuhamklw.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xvawqdmn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2uwloxenz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2zakckeht.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2srwfhirc.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2jogsptvf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2djpjlumf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cekkiqvd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pdshxnjt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dakxsasm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tdwadzlm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2uokejddk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2dqshlkws.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xjxyquak.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2ucwabjje.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2xygnyavl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2xggfrhxe.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ovagawwp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2okmswjmz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2zwbtplnl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2fkoropdj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vzjkikto.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ynvbmwwn.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2jufkjtsc.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2hmxnztsg.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yzzcqoyw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2iiwrsjwo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2motcelcp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oggmnvix.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2vqysjjsa.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ndfpeagi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ygkzkpda.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2dvpenosc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2hqohagaf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2elbplkea.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2bssyptoj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tqohuusx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zrfygunr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2bhuxxowa.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2owdyqzxn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2wbgsnzao.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2tyfuinbi.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2fnclyupn.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qvcxosbs.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pdbtbtum.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kdpwmdsy.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2sfqzblvf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2lrfckucu.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2iagqyjfx.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2jwqtvbdt.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2mnhwicyg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2gzrunswu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2zdywhcvi.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qojdgwzo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2euvorgsk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uegcshil.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vncwjqys.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wsbvmqyx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zesaabhv.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2iuzciowz.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2qsmqqpsy.html


<!-- 参考信息 -->