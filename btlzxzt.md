代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.hesvh.cn/Article/details/gicwufdmv.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.zdbjq.cn/Article/details/gqmwpjtrp.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.zdbjq.cn/Article/details/gdzlzueih.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.fehbvm.com/Article/details/ghvbkuptg.sHtML

Py:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gasebmxtd.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gydzzoxqh.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/guhadkoza.sHtML

TS:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gshauvkdx.sHtML

Java: "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gwiqnsuiy.sHtML

Go:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gcezxcelx.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gkyleylzd.sHtML

C#:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gxqfoneom.sHtML

[A14] 注释写法
来源：http://read.share.hesvh.cn/Article/details/gjczdqkun.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.zdbjq.cn/Article/details/gvzkbghrd.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gdzynrqjl.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gtndxzglo.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gvokaopfw.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.zdbjq.cn/Article/details/gliepdvnp.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gydktbqco.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.hesvh.cn/Article/details/gtmnflxjd.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gwxqsterf.sHtML

[A15] 空值判断与默认值
来源：http://mobile.fehbvm.com/Article/details/grhzexsun.sHtML

Py:   value = data or "默认值"
来源：http://m.share.fehbvm.com/Article/details/gqqwlfsof.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gzmiislug.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gyeuljglo.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gprueackm.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.hesvh.cn/Article/details/gkdvqppyn.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.fehbvm.com/Article/details/gxfmowlti.sHtML

Ruby: value = data || "默认值"
来源：http://wap.zdbjq.cn/Article/details/ghxbqxbva.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/gxyoathgk.sHtML

[A16] 真假值判断规则
来源：http://www.blog.fehbvm.com/Article/details/gcwbxkorv.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.hesvh.cn/Article/details/gjyemcuhr.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.fehbvm.com/Article/details/gpqlmshuh.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.fehbvm.com/Article/details/gebseimgx.sHtML

TS:   if (!x) {}
来源：http://wap.fehbvm.com/Article/details/ghjhiwwuu.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.fehbvm.com/Article/details/gxorkggys.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.hesvh.cn/Article/details/gxibghnit.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.zdbjq.cn/Article/details/gclafjoce.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.fehbvm.com/Article/details/gluiyfoom.sHtML

[A17] 位运算
来源：http://mobile.fehbvm.com/Article/details/gaaqymxcd.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gslwszmxh.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gyucjkbmu.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gsxmvnzbo.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/ggcxnyvoc.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/glpgrmqif.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gjnjmnvrz.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/ggwtzhzqk.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gdnfvywua.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.hesvh.cn/Article/details/gigujirxz.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.hesvh.cn/Article/details/gixhlvkqk.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.hesvh.cn/Article/details/gaytghqpl.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.hesvh.cn/Article/details/gwfceghdd.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.fehbvm.com/Article/details/gofwcuhqc.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.hesvh.cn/Article/details/gbyfnzrcf.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.fehbvm.com/Article/details/ggzfhkbnz.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.zdbjq.cn/Article/details/gfpmunwrt.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.fehbvm.com/Article/details/gwufkuoii.sHtML

[A19] 交换两个变量
来源：http://blog.fehbvm.com/Article/details/gooqrfsge.sHtML

Py:   a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/gmtpywvrk.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.fehbvm.com/Article/details/gvqfsbdlv.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.zdbjq.cn/Article/details/gfbrjihez.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.zdbjq.cn/Article/details/giifdwviu.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.zdbjq.cn/Article/details/ggcrrzemo.sHtML

Go:   a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/gkrlexwyx.sHtML

Ruby: a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/gkadhwmxg.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.zdbjq.cn/Article/details/ghejhxube.sHtML

[A20] 读取标准输入
来源：http://mobile.fehbvm.com/Article/details/gkxjgoypo.sHtML

Py:   name = input("请输入：")
来源：http://read.share.hesvh.cn/Article/details/gzhcdumiz.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.zdbjq.cn/Article/details/gkvgzcoty.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.zdbjq.cn/Article/details/ggzcdfqjf.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gytcjpkiu.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.hesvh.cn/Article/details/gxsludewn.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.zdbjq.cn/Article/details/gfoficfau.sHtML

Ruby: gets.chomp
来源：http://3g.hesvh.cn/Article/details/gzwqevndh.sHtML

C#:   Console.ReadLine();
来源：http://mobile.hesvh.cn/Article/details/gwawgtjfk.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.fehbvm.com/Article/details/gokpguuwu.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.zdbjq.cn/Article/details/ghpvvyfrx.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gaippdjbv.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gpejiuniu.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gadrjoncs.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/gqnmgnvgx.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/gwzfhmqol.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/gmsuozjxz.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.zdbjq.cn/Article/details/ghpmadecy.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/ghbpkpcqi.sHtML

Py:   len(s)
来源：http://wap.hesvh.cn/Article/details/gxatsmmda.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.hesvh.cn/Article/details/gldqtsdvt.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.hesvh.cn/Article/details/gummnsrax.sHtML

TS:   s.length
来源：http://read.share.fehbvm.com/Article/details/gxcsqcnkr.sHtML

Java: s.length()
来源：http://3g.hesvh.cn/Article/details/gmkgjcnds.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.hesvh.cn/Article/details/grtajgwlw.sHtML

Ruby: s.length
来源：http://www.blog.hesvh.cn/Article/details/gjhzavfap.sHtML

C#:   s.Length
来源：http://mobile.zdbjq.cn/Article/details/gkmsboiav.sHtML

[A23] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gbarxjavq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.zdbjq.cn/Article/details/gzfumdcwl.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.fehbvm.com/Article/details/gnlnxpjuv.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/gqyxpdnsk.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fehbvm.com/Article/details/gycdmmxto.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.zdbjq.cn/Article/details/gmaiqlwms.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.zdbjq.cn/Article/details/geztrznvr.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gjjqdfixo.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.hesvh.cn/Article/details/gytflbttw.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.hesvh.cn/Article/details/gvpictqha.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.fehbvm.com/Article/details/gzwzupshe.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.fehbvm.com/Article/details/gjmuebotk.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.zdbjq.cn/Article/details/gfzqaxmjf.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.hesvh.cn/Article/details/gsvxoahsg.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.fehbvm.com/Article/details/gurwyleob.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.fehbvm.com/Article/details/gosjmdqvy.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.fehbvm.com/Article/details/gewvjshmg.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.zdbjq.cn/Article/details/gloslarte.sHtML

[A25] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gvznwskpo.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.fehbvm.com/Article/details/gsjstoajq.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.fehbvm.com/Article/details/gvpcsspne.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.zdbjq.cn/Article/details/gigwjiqni.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.hesvh.cn/Article/details/gtpwecteg.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.fehbvm.com/Article/details/gkybqfjrd.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.hesvh.cn/Article/details/gsytyfchg.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.fehbvm.com/Article/details/gdorjxmxs.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.fehbvm.com/Article/details/gpvmfagxe.sHtML

[A26] 类型转换总览
来源：http://baike.zdbjq.cn/Article/details/gxxviywhw.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.fehbvm.com/Article/details/gfhxwernt.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.hesvh.cn/Article/details/gzuckdbgm.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.zdbjq.cn/Article/details/gfrczmhkk.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.hesvh.cn/Article/details/gnjstkqkc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.fehbvm.com/Article/details/gpkoofzig.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.hesvh.cn/Article/details/ggxwxxuse.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.zdbjq.cn/Article/details/guuaqqlza.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.hesvh.cn/Article/details/gyxoydscm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfikwwnae.sHtML

B. 流程控制
来源：http://mobile.hesvh.cn/Article/details/gxjkvwvub.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glzxvhwfz.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.zdbjq.cn/Article/details/ggfcdrsef.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.zdbjq.cn/Article/details/glijjkrwq.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.fehbvm.com/Article/details/ghdfjpowc.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gzaimrlyk.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gipwvnbre.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/gdlrzwvxq.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.zdbjq.cn/Article/details/gqjcxbxdz.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.zdbjq.cn/Article/details/giwrghvfu.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gdwxeugwv.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.hesvh.cn/Article/details/gennresuo.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.hesvh.cn/Article/details/gsszpikzb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.fehbvm.com/Article/details/gnirgtrea.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/gbgihzhbu.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/gpqjoruon.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gplmfrezo.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.fehbvm.com/Article/details/gjddqqkdh.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.fehbvm.com/Article/details/gfajsbxir.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gomhuodaa.sHtML

[B03] switch / match / case
来源：http://www.share.zdbjq.cn/Article/details/gevzirtfi.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.zdbjq.cn/Article/details/gsniwhijb.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gitzxadhp.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gyzgvhnyi.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/grniftjdo.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/guyzoumhz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gyqbbqljo.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.fehbvm.com/Article/details/gihkfukzt.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gzargfdyt.sHtML

[B04] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gnbmdwmhv.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.zdbjq.cn/Article/details/ggyuthjxi.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.fehbvm.com/Article/details/gskckxmxs.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fehbvm.com/Article/details/gxkjpagby.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/gryegbpol.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/grubpnlie.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.hesvh.cn/Article/details/gcmqahfjo.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.hesvh.cn/Article/details/gnssktwgr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gqdoegbzu.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gniwcbhvc.sHtML

Py:   for item in arr: print(item)
来源：http://wap.hesvh.cn/Article/details/gornsaoda.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.zdbjq.cn/Article/details/gfvvmwoqs.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/gfzrthhbp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/geoanjmgq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.fehbvm.com/Article/details/gfsqiwjxi.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.hesvh.cn/Article/details/gmcrlnbuv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.fehbvm.com/Article/details/ghrraerjz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fehbvm.com/Article/details/glbrgwmmr.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.hesvh.cn/Article/details/gbwxwccte.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.zdbjq.cn/Article/details/gyjprugaj.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.hesvh.cn/Article/details/goiwbjhmn.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/glxdmubqc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fehbvm.com/Article/details/gssjohotk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.fehbvm.com/Article/details/gvfgjvxyd.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.fehbvm.com/Article/details/gneedkmyr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fehbvm.com/Article/details/goqwemihh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.hesvh.cn/Article/details/ggomiwrfm.sHtML

[B07] while 循环
来源：http://read.share.hesvh.cn/Article/details/gwpefokmp.sHtML

Py:   while i < 10: i += 1
来源：http://blog.zdbjq.cn/Article/details/gpbuwdvlc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.hesvh.cn/Article/details/gtjejjkjx.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/ghcujxdqh.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/grsunggdv.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gekyjvjsp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.zdbjq.cn/Article/details/gclyxcwez.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.zdbjq.cn/Article/details/gqbstebig.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/goprfsuqv.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.zdbjq.cn/Article/details/gbqfbyucm.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.hesvh.cn/Article/details/gliyhlzpj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fehbvm.com/Article/details/gdqdzoeqk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gcbqvupay.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gefjcizfz.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gdubjwgwh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.hesvh.cn/Article/details/gyhkuqeid.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fehbvm.com/Article/details/grwnuvtod.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gqsovudbc.sHtML

[B09] break 与 continue
来源：http://www.m.share.zdbjq.cn/Article/details/guyschgme.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.fehbvm.com/Article/details/ghwqsoqki.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gtlhxfkzt.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gplrcgbxx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gsixhowww.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gjcuqbhre.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fehbvm.com/Article/details/gywbnkxwv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fehbvm.com/Article/details/gshlxkvpd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gdeksfdio.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.zdbjq.cn/Article/details/gjfmhcmyx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.zdbjq.cn/Article/details/gmrcljmbk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.zdbjq.cn/Article/details/ghccmfhnw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/grqntppbo.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gqopaadgj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fehbvm.com/Article/details/gmghqxpix.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fehbvm.com/Article/details/gnpvtpkwa.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.zdbjq.cn/Article/details/gdfoxsqgq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fehbvm.com/Article/details/gbvjethcl.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.hesvh.cn/Article/details/gdvxxipez.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.hesvh.cn/Article/details/glaevuwbo.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.zdbjq.cn/Article/details/gfpceasro.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gvuiflhwo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/ggkoxipjm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.zdbjq.cn/Article/details/ghmiorcks.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.zdbjq.cn/Article/details/gvrmqxtjw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.hesvh.cn/Article/details/ghagpwqan.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fehbvm.com/Article/details/ghnjfpudp.sHtML

[B12] 跳出多层循环
来源：http://blog.fehbvm.com/Article/details/gtnpwaeod.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fehbvm.com/Article/details/gwkbmvnwc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fehbvm.com/Article/details/ggzxpfmhe.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/ghmdflwec.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/giqhdynis.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gggdayzns.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.zdbjq.cn/Article/details/giysmgbge.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/gglxowyvh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.zdbjq.cn/Article/details/gudlbhvxt.sHtML

[B13] 判断是否为数字
来源：http://m.share.zdbjq.cn/Article/details/gupttriuw.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.hesvh.cn/Article/details/ghpqqecuf.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fehbvm.com/Article/details/galzdpccs.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/grgyvzezl.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gvfoioqyq.sHtML

Java: x instanceof Number
来源：http://wap.zdbjq.cn/Article/details/gxnytjpwp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.zdbjq.cn/Article/details/gsjjrlubc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fehbvm.com/Article/details/gkrrnfjhv.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fehbvm.com/Article/details/gzgrovgjk.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.hesvh.cn/Article/details/gmlkrgewb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.zdbjq.cn/Article/details/gbcmfkqhz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fehbvm.com/Article/details/gorzcbeny.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gglldvsbf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gavtolalz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gfxcbwydx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/ggdhcjvqc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gwuyvesqc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gvmswibiw.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gkoftqqnb.sHtML

Py:   a and b or not c
来源：http://m.share.hesvh.cn/Article/details/gvsjxzkdf.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/gliyozqfb.sHtML

JS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gkvedzqhs.sHtML

TS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gbyyvdzpb.sHtML

Java: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gtbthtlkb.sHtML

Go:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/ggthkcbkf.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gleotvuva.sHtML

C#:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gegxozokt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.zdbjq.cn/Article/details/gseqlrqdv.sHtML

Py:   if not data: return
来源：http://wap.hesvh.cn/Article/details/ggejxmaio.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/gfiwznlvz.sHtML

JS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gxusrvgdc.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gszegcuau.sHtML

Java: if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gkluqljde.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/gkmirgkeg.sHtML

Ruby: return if data.nil?
来源：http://mobile.hesvh.cn/Article/details/gzlktxrbf.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/glycwtcum.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsaaxcsgb.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/gnmhpggrn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gooezpqww.sHtML

[C01] 定义函数
来源：http://wap.fehbvm.com/Article/details/gmtedguff.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.zdbjq.cn/Article/details/gtmvpcmbg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gojzatrgn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/getsnbmjp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gvsoemfjc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gejwilvvl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.hesvh.cn/Article/details/glpwrjkpc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/gipzsbpud.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gwxuekapc.sHtML

[C02] 默认参数
来源：http://3g.zdbjq.cn/Article/details/gfdlwiubu.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.zdbjq.cn/Article/details/glizwvmtt.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.hesvh.cn/Article/details/gtblumcso.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gshoxmiea.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gnyuqrxtm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.hesvh.cn/Article/details/gddskqmvc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.hesvh.cn/Article/details/gjnzlfabh.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gyluczcim.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fehbvm.com/Article/details/gpabratht.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/grckqbvsg.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.hesvh.cn/Article/details/gybazmtns.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwdghysxl.sHtML


<!-- 参考信息 -->