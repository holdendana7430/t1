代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.hesvh.cn/Article/details/garkpentx.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/gcyipqoqh.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.hesvh.cn/Article/details/gbhvtxeku.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.zdbjq.cn/Article/details/gnwhqjqxj.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gnfuqesbu.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/giajqibuh.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gutqdledt.sHtML

TS:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/glovjuwob.sHtML

Java: "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gnzquqqbj.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gjeajagcr.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/ghnktrvlq.sHtML

C#:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gfmcohouq.sHtML

[A14] 注释写法
来源：http://wap.fehbvm.com/Article/details/gftztwqil.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.hesvh.cn/Article/details/gwguidllb.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/glndyfqrw.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gqbferenw.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gnyhuayaw.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.zdbjq.cn/Article/details/gyxwfttlb.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gaosofqyk.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.zdbjq.cn/Article/details/ggsqvnmfz.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gnkvqsdlh.sHtML

[A15] 空值判断与默认值
来源：http://m.share.zdbjq.cn/Article/details/gzthsqyhw.sHtML

Py:   value = data or "默认值"
来源：http://3g.fehbvm.com/Article/details/guiaovrqw.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gvvfhoqnc.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gwexljten.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gencrhbno.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.fehbvm.com/Article/details/gkswydtfw.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.fehbvm.com/Article/details/ghfoohoys.sHtML

Ruby: value = data || "默认值"
来源：http://blog.hesvh.cn/Article/details/gsefjigni.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gkvirimqr.sHtML

[A16] 真假值判断规则
来源：http://www.share.zdbjq.cn/Article/details/glvtjwhuf.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.zdbjq.cn/Article/details/gqfishvhd.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.fehbvm.com/Article/details/gooigtksb.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.hesvh.cn/Article/details/genzbpofe.sHtML

TS:   if (!x) {}
来源：http://wap.fehbvm.com/Article/details/gbjyrlbry.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.fehbvm.com/Article/details/gqklegquy.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.zdbjq.cn/Article/details/gzvsxykvb.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.hesvh.cn/Article/details/gmjawaber.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.hesvh.cn/Article/details/gnnsshrbg.sHtML

[A17] 位运算
来源：http://m.share.fehbvm.com/Article/details/glewfpzwx.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/ghickwfxd.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.fehbvm.com/Article/details/gnttxpufa.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gdkorhkkb.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gvsfyrcpi.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gwdutramk.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gkdvkjgok.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gvqzjncda.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gryydaqxq.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.hesvh.cn/Article/details/goyppvhyh.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.hesvh.cn/Article/details/gkcmtiqqr.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.hesvh.cn/Article/details/gcxprecrl.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.zdbjq.cn/Article/details/gsizfxzjd.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.zdbjq.cn/Article/details/grqrngxhn.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.fehbvm.com/Article/details/gbnrbwazw.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.hesvh.cn/Article/details/girhdibjx.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.fehbvm.com/Article/details/gbioerecp.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.fehbvm.com/Article/details/gqxahhcav.sHtML

[A19] 交换两个变量
来源：http://www.m.share.hesvh.cn/Article/details/gpgkgnlhx.sHtML

Py:   a, b = b, a
来源：http://www.m.share.hesvh.cn/Article/details/gkvnttcaf.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.fehbvm.com/Article/details/gkuoebiuw.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.fehbvm.com/Article/details/ggxqoepgd.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.fehbvm.com/Article/details/gikwaabvi.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.hesvh.cn/Article/details/grgknkwar.sHtML

Go:   a, b = b, a
来源：http://blog.fehbvm.com/Article/details/gkyjhsude.sHtML

Ruby: a, b = b, a
来源：http://3g.zdbjq.cn/Article/details/gphwarbng.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.hesvh.cn/Article/details/gtjpppnbl.sHtML

[A20] 读取标准输入
来源：http://www.blog.fehbvm.com/Article/details/gaaokssdc.sHtML

Py:   name = input("请输入：")
来源：http://mobile.hesvh.cn/Article/details/gpexrzgiw.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.zdbjq.cn/Article/details/gfmoxpvrc.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.zdbjq.cn/Article/details/gjfozhsvt.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.fehbvm.com/Article/details/glmunorju.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.fehbvm.com/Article/details/gdqhneqph.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.fehbvm.com/Article/details/gmufyajis.sHtML

Ruby: gets.chomp
来源：http://blog.fehbvm.com/Article/details/gktcxwcta.sHtML

C#:   Console.ReadLine();
来源：http://3g.fehbvm.com/Article/details/gyiztnwfv.sHtML

[A21] 保留指定小数位输出
来源：http://blog.fehbvm.com/Article/details/gfgvmedqm.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.zdbjq.cn/Article/details/gdmrgaywv.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/gfgtefdeg.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gaszcrifq.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gwtlvyamq.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/gwvvvrcen.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gghrobwtz.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gnneridrj.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.zdbjq.cn/Article/details/gdaptfihj.sHtML

[A22] 获取字符串长度
来源：http://blog.hesvh.cn/Article/details/gnqgpdkfu.sHtML

Py:   len(s)
来源：http://www.share.zdbjq.cn/Article/details/gvbasavso.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.hesvh.cn/Article/details/gjxkeybjf.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.zdbjq.cn/Article/details/ggsivjhgb.sHtML

TS:   s.length
来源：http://www.m.share.fehbvm.com/Article/details/gxttrxdqs.sHtML

Java: s.length()
来源：http://m.share.fehbvm.com/Article/details/grcwdkhrq.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gotnmbjkm.sHtML

Ruby: s.length
来源：http://mobile.zdbjq.cn/Article/details/gleigfwux.sHtML

C#:   s.Length
来源：http://mobile.fehbvm.com/Article/details/gzfkgflch.sHtML

[A23] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gfeguntnp.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.hesvh.cn/Article/details/gpopitfha.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.fehbvm.com/Article/details/gejzgezxy.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.zdbjq.cn/Article/details/ghltgduri.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.zdbjq.cn/Article/details/ghsdvczqk.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.hesvh.cn/Article/details/gcxwjnrkx.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.fehbvm.com/Article/details/gkgajhtzg.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.fehbvm.com/Article/details/glxyjanux.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.fehbvm.com/Article/details/glzlglxbp.sHtML

[A24] 去除首尾空白
来源：http://m.share.fehbvm.com/Article/details/ghlioltwn.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.fehbvm.com/Article/details/gjixcruya.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.zdbjq.cn/Article/details/gwnjyetxd.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.hesvh.cn/Article/details/gldjglguc.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fehbvm.com/Article/details/gmktrubhi.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.zdbjq.cn/Article/details/ggqquksdr.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.fehbvm.com/Article/details/gbrbqknzi.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.zdbjq.cn/Article/details/gsesyhefx.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.zdbjq.cn/Article/details/gdeinfgna.sHtML

[A25] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gpcmqyrdh.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.zdbjq.cn/Article/details/gpvfgqqgo.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.zdbjq.cn/Article/details/gdxltexdc.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gisqbkzhc.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.hesvh.cn/Article/details/gdcinukeu.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.zdbjq.cn/Article/details/gphacfkue.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.hesvh.cn/Article/details/gtfchcykx.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.fehbvm.com/Article/details/gsselsimm.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.zdbjq.cn/Article/details/gqextcwdu.sHtML

[A26] 类型转换总览
来源：http://www.share.zdbjq.cn/Article/details/gbcnfryvd.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.hesvh.cn/Article/details/gepjfnvru.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.fehbvm.com/Article/details/gminpnvbo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.fehbvm.com/Article/details/gyfmcuzyp.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.hesvh.cn/Article/details/gygofefyr.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.fehbvm.com/Article/details/gifwdphox.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.zdbjq.cn/Article/details/gytswsjme.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.zdbjq.cn/Article/details/ghlbmnuby.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.fehbvm.com/Article/details/gjndjzlcu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnmofvgul.sHtML

B. 流程控制
来源：http://m.share.hesvh.cn/Article/details/gmaaapuoq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmpwbdbtd.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.fehbvm.com/Article/details/giammeocw.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.hesvh.cn/Article/details/gvzfmeifh.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.zdbjq.cn/Article/details/ggfqnojwf.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gyxowwrke.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gypgrbzzb.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gjsgtxaxo.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.hesvh.cn/Article/details/gsndqwuho.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.fehbvm.com/Article/details/gosorcufk.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gigbuofqd.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.hesvh.cn/Article/details/gybtvhbtn.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.hesvh.cn/Article/details/gqrcclndv.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.hesvh.cn/Article/details/gbncsbqjc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gihirhbum.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gyuruzshy.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gtgjohoot.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.hesvh.cn/Article/details/gchjvzugf.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.zdbjq.cn/Article/details/gpuaatwbn.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gyqrtoywq.sHtML

[B03] switch / match / case
来源：http://mobile.fehbvm.com/Article/details/gvplzuutp.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.zdbjq.cn/Article/details/grkqpztkd.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gnvyoxoxi.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gbsboeabf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gmpexfnxz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gsrngpozx.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.hesvh.cn/Article/details/gwqqiasir.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.fehbvm.com/Article/details/gyblpsclm.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/gehforzfm.sHtML

[B04] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gcdhtbyqc.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.hesvh.cn/Article/details/gcsenhlwc.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.hesvh.cn/Article/details/gvveoznyp.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fehbvm.com/Article/details/gouzznkqx.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gflgsboka.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.hesvh.cn/Article/details/guqpobqxr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.zdbjq.cn/Article/details/gqihcyfgk.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.fehbvm.com/Article/details/gfmywbttj.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.fehbvm.com/Article/details/gqvacfkhm.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/glycujdsx.sHtML

Py:   for item in arr: print(item)
来源：http://baike.fehbvm.com/Article/details/gofyzbkxf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.hesvh.cn/Article/details/geoajlpvu.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/ghvithqnv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.zdbjq.cn/Article/details/glacyfelp.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.fehbvm.com/Article/details/guhbdzydx.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.hesvh.cn/Article/details/gjdxmugqb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.hesvh.cn/Article/details/gdvzvtcoi.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.zdbjq.cn/Article/details/gkebsxupo.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.zdbjq.cn/Article/details/ggsvnnjhl.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.hesvh.cn/Article/details/grgqxjlwt.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.fehbvm.com/Article/details/goenniutw.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/gckuynbiw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/gctdsiqkf.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fehbvm.com/Article/details/goozulvng.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fehbvm.com/Article/details/gcfbarygj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.hesvh.cn/Article/details/gscrsjlfq.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.fehbvm.com/Article/details/gwtpjstyw.sHtML

[B07] while 循环
来源：http://www.share.fehbvm.com/Article/details/gcryrrtgn.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fehbvm.com/Article/details/gvwvfwywi.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.hesvh.cn/Article/details/gxiwudlyd.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gcmwhhrzo.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gzyvsjxst.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwgsxchiu.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.hesvh.cn/Article/details/gapaemtyx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.zdbjq.cn/Article/details/giffpelox.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/grvwhbcvz.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fehbvm.com/Article/details/gcwubimxg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.zdbjq.cn/Article/details/gfthydsnw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gcbfbtxaa.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gmayngxvv.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gbrdpgnmz.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gugpbrutd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.hesvh.cn/Article/details/guuccvpti.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fehbvm.com/Article/details/gldeloygz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gkxzocswn.sHtML

[B09] break 与 continue
来源：http://www.share.fehbvm.com/Article/details/gxlwtfboe.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.zdbjq.cn/Article/details/gmvmbwrin.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/glbyfvznj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gttorlgeg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/giylrenem.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gfijaoujx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.hesvh.cn/Article/details/gilwhhiuj.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.hesvh.cn/Article/details/gvexanyxb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/guvvbbbfd.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.hesvh.cn/Article/details/gapmxnqzs.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.hesvh.cn/Article/details/ghevwnmbg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.hesvh.cn/Article/details/gvppipegf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/gvsgculcw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/gskbnzmpr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fehbvm.com/Article/details/gbdscfgcl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fehbvm.com/Article/details/gzewxdpyq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fehbvm.com/Article/details/gtrexigcw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.zdbjq.cn/Article/details/gairprcrr.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.hesvh.cn/Article/details/guuvzmglg.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.hesvh.cn/Article/details/gcelvzxma.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fehbvm.com/Article/details/gngtodiui.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/gloxaupbu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/geayvydqc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.hesvh.cn/Article/details/gltsozont.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.zdbjq.cn/Article/details/gxrgledkr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fehbvm.com/Article/details/gozblkquw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.zdbjq.cn/Article/details/gpvevkplg.sHtML

[B12] 跳出多层循环
来源：http://www.share.hesvh.cn/Article/details/gnipmjfqn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.hesvh.cn/Article/details/geedxdruh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/gffsulnow.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gvidmcnrb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gfypvdzcm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gzjljliwy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fehbvm.com/Article/details/gmmzmwzrr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/gmfzvruej.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.hesvh.cn/Article/details/gijnsjcfy.sHtML

[B13] 判断是否为数字
来源：http://www.blog.zdbjq.cn/Article/details/ghsuxaswi.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fehbvm.com/Article/details/ggavxwstg.sHtML

PHP:  is_numeric($x)
来源：http://blog.hesvh.cn/Article/details/gzjmakwgy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkwwmmsef.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gmjsddkkq.sHtML

Java: x instanceof Number
来源：http://wap.hesvh.cn/Article/details/gqzxghfzp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.hesvh.cn/Article/details/gxqvbjcbh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fehbvm.com/Article/details/ggsvxmrek.sHtML

C#:   x is int or double or decimal
来源：http://blog.hesvh.cn/Article/details/gurdfnhfb.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.zdbjq.cn/Article/details/gbybuevnn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fehbvm.com/Article/details/gnkhqeyql.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.hesvh.cn/Article/details/gebyrdlhz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/grxinoccb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/guqjekmbb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.hesvh.cn/Article/details/gbeodkrlj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.hesvh.cn/Article/details/gykisnumz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fehbvm.com/Article/details/gxwjmxzpt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gwdicbfvi.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/govgyhixy.sHtML

Py:   a and b or not c
来源：http://www.m.share.hesvh.cn/Article/details/gmtssafqr.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.zdbjq.cn/Article/details/gldarwpfp.sHtML

JS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gzzerkzcn.sHtML

TS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gpmeczswl.sHtML

Java: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gzlrfyzli.sHtML

Go:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gllbatsye.sHtML

Ruby: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gxhhbhtgz.sHtML

C#:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gxapdkubx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.zdbjq.cn/Article/details/gmpcsdesq.sHtML

Py:   if not data: return
来源：http://wap.zdbjq.cn/Article/details/glguqowpn.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fehbvm.com/Article/details/gndkvccif.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gflpgkzck.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gpbntgpyf.sHtML

Java: if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gwvphlcvi.sHtML

Go:   if data == nil { return }
来源：http://3g.hesvh.cn/Article/details/gvpdpljle.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gbbwilqub.sHtML

C#:   if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gvtzfveip.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gyzwowdes.sHtML

C. 函数与作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gvolwyvxj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggxmbgkmx.sHtML

[C01] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gpldxhmad.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.zdbjq.cn/Article/details/gzrpbnkue.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gmaqzaivd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gnhuafrgs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gxmytimgg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gnfkpxrbo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gloqzefau.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.zdbjq.cn/Article/details/gwvygpqdv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gxcxevzul.sHtML

[C02] 默认参数
来源：http://wap.zdbjq.cn/Article/details/gutkrepla.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/giozmmswk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fehbvm.com/Article/details/ganazetwu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbwqfsyis.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/ggycsdbrq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fehbvm.com/Article/details/gdsvtehtr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/geapaartj.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fehbvm.com/Article/details/ggizzhuqm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.zdbjq.cn/Article/details/gybaaszub.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/gfylgmooa.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.hesvh.cn/Article/details/gtbrfnwwc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/giyqzwnio.sHtML


<!-- 参考信息 -->