代发 wailian999

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ddhygwsh.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3wugjhrxn.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3zqswttzj.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3jzhegozr.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3oncbvqld.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3yunowapy.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3kbiwcxrb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3fzpnqlss.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3rhrmxuxn.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3vrvtyyow.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3gunnexmp.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mdifsjxe.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3cdxovudd.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3yrzyelyo.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3krqmgala.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3kzwsgqgq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3csnlmnir.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vwsjolkd.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tqqdxtxq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dqkzsfte.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xxblllhz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3ovjatisk.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3asmjrwiz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ugkpsosl.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3ojqgdnhd.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3aazkonoe.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3cksbksls.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ekcsmuas.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3kreshyqj.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3qdgpzkdm.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3tzxpffdi.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3zxclwlnp.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3tkhjgvql.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3mprkizmz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3olerqwcp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xcdyydem.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pohtvkqa.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3onndhbaq.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qkadjkyq.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3rwkictfl.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3iagpznne.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nrpytvzz.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3qiggyysj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3pqymozjn.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3hratyhio.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3igcntgql.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3pqbsogdh.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3rclhelcq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3piqzygwq.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3dqaftctm.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3bflejlel.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3hhfmvgfv.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tfgjyyww.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3frqymzyk.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ijdeswen.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pqlykufq.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ewomdjky.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ofxstrhz.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qgtbmnuy.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xtjqlbpm.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3mvdmlmph.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3zijqdaag.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hiwiuuvh.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ypvitdye.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3uuhldnvc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3htacbfws.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3dyfrthod.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3zxzzqbvx.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xomhcaqa.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mfiheeck.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3zftjijsn.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ehzscxzv.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3dvmhgple.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3kdusoscz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3nfyhobwv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3qqhmqerr.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3kmxomoai.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fvczuiil.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3wofijhzl.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3yfhxmjcl.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3oqpcfncq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3cmikddms.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ewyilgiq.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3zxujyzks.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3lrzboqjs.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3xijqlbgc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ikbtuoye.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3iinuvqqo.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cwwmfuer.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3iubsfjxy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ybwktbnx.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yyqrheqv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hgejnubl.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pwajtqlz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xpyxnqil.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hlriaplb.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3ugtxeeje.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3fcmfnkqx.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qgzuikej.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3gfbsylmb.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3pzuhftei.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3mfkkqqfp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3oieyogxo.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3xxpeufkc.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3oeafykmm.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3xzystlba.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3pbtimhyg.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3lokgulzv.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3gsqffowu.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3pnrbatiq.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3ytwmjanj.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ibqitdez.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3nschfzhr.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3trtoqzgw.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3pchcklbv.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3vhormhio.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3tdzmcikv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3bdjojjku.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3ifhggqwf.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3cgzkftnl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3xnlrptea.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3jwxtnato.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3vudwhsaf.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3kjcnajfq.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3plwkmvmq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3bzyypczb.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ouiredic.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vkiqweqw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3mzklnvhc.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3dkwzisph.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ewlqkxzk.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3flprnrxx.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hbkfnitx.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ytkvpjrx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3ihrthkqa.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3zcyuhwvj.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3phajlacy.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qfzpaccj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3hpdwuxyp.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3mxgxizkh.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ladeyivv.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ogfvqwfv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3fbfvhimg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3nkvlugfi.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3iastmotu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ydqagkbj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3lddgocqi.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3tqnzlcgl.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3pzzfxvnk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3irfjxskw.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3oqlhkgfy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3xcizuimq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3nxtsuazs.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3mrnniwat.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3hntklgor.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3cyzljama.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3otaxuakq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3dvsixhil.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3fggkesbs.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ovuukxou.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3twxjeigo.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zizywfdq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3qvymnfqn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jbowaekl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3wcbmiknt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rynsadvh.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3aoibwbfw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ozrsovcl.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3yozbkozk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3zzxlibeh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3jwjlbstc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3fhmbasin.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3ombdukeh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3sfboxpwk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3yankyhsr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3dngzptlm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3hanhmbuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ccymucfn.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3umkdaqqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3anjnypov.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3scnrrzmv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3rasfpabh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3jcwgjdsc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jncrvlgt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3svhgwsll.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3eblmrbrr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3oshotipg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3xpnkrhrm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ubbuzbyv.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3jywqijne.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3fkbtoeif.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3jsyhssvb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3nnbcjdab.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xildsfrj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jnwbolon.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3vvzndmzl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3cbpufecv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ppjznveg.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3agmjtdpw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3tkrkczvk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzukaees.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3elvdzwed.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3czkjjrid.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifpuppmp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3umxetqqb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3ucphfygr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3qmbwdlef.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3wgacefsc.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ppovnodq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3gojcnkpw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3xehmjkkj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3stzxbxpw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ybbukgll.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3flcsfntb.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3ndscjwui.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3uziaaikn.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3hdqexwbw.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3tjhkiamd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3mbkoxhhw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fbmupehj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mmhbxkce.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rahdhggu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ioqbtknr.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3swrpsfbc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qehvmmwi.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3idmwrsru.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3xrodewhx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aihbtxum.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3bxgfrcbb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3gnilgahr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3yaupmpau.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3vgoccxkw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ysyhsgue.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ccnuvesr.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3fmzdiafh.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3byjrngpi.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oontlann.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nvcpdroq.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqspnwth.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jqrrluiw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3xhfohbbx.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3ztynmbib.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nutzazbg.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3crzdhiol.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3eaoellgn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pirhfnxj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bfszgmqx.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cjondpit.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mejyhlbo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3spvzgofe.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3xpcfayuz.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zxzayhtg.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3zleirknw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3bkbhgmir.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmzjygsl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hekzckiy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ljmmrgmd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxumezre.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3xubsbpps.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3dopvrkgk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jfqmxovt.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3iimuigvl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3caruhpvy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ryamhowv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3zahbqlbv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ctvomvpf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3tlkshraa.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3zspphfmg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3azeoekll.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3zcdyfjnh.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3smmmtizj.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3mzcrwmsl.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3vgdvgsks.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jggjzbbn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ubenkgtl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vzmqcszk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3hylsmytf.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qvizdtbm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nereubcw.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3yzgfwdcl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3pqpqkxco.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3vuiopohc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3syimxxir.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bjgyhagq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gsbdfdji.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ezfhisqm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3xpwrvgfw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ptpxqbna.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3vwjglbyj.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3kxbvylmq.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3sxiqqqzi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3qipmubby.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gcexhwzd.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3osnswzkg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3tqdzgelq.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3omawcaxx.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3akbkfljn.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3jaarkwrf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3qzwohjol.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3zxxbrpgm.html


<!-- 参考信息 -->