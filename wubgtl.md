代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://hz.gzhubu.top/gtejxesxpi.html

[A11] 条件表达式（三元）
来源：http://hz.zhaomingkeji.xyz/gtnlmhmngi.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.jianghu66.top/gtqyynlshj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.xylfe.cn/gtxsolqcgp.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.yj20258.top/gtoysrtjke.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.aibaodan.cn/gtyajwfqwb.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.yongpay.top/gtztdeockw.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.daxiang520.top/gtiucjujgt.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.nanxinkj.top/gtowdxfihw.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.cucudq.cn/gtdecwdykm.html

[A12] 字符串插值 / 格式化
来源：http://hz.hywenlv.cn/gtqeclxzpv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.daxiang520.top/gtfzjvdqbv.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.yueranfly.top/gtbqpttvtv.html

JS:   `Hello, ${name}!`
来源：http://hz.zycfv.cn/gtmfpriwzv.html

TS:   `Hello, ${name}!`
来源：http://hz.pycfn.com/gtzmwydhzd.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.yj202588.top/gtqryphspg.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.yj20258888.top/gtimlbufxc.html

Ruby: "Hello, #{name}!"
来源：http://hz.chenjidiqi.icu/gtbjfsafki.html

C#:   $"Hello, {name}!"
来源：http://hz.yvedp.cn/gtbugisavy.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.pycfn.com/gtgdalmuwt.html

Py:   "第一行\n第二行"
来源：http://hz.fengsongda.top/gthatiaeao.html

PHP:  "第一行\n第二行"
来源：http://hz.hnqzz.top/gtfiwtseag.html

JS:   "第一行\n第二行"
来源：http://hz.zhengqikj.top/gtuqbfqlpn.html

TS:   "第一行\n第二行"
来源：http://hz.ydzc1.top/gturnrvdaa.html

Java: "第一行\n第二行"
来源：http://hz.yj20258.top/gtacndfmlp.html

Go:   "第一行\n第二行"
来源：http://hz.fengsongda.top/gtfqhfsion.html

Ruby: "第一行\n第二行"
来源：http://hz.yvedp.cn/gtwcgyshly.html

C#:   "第一行\n第二行"
来源：http://hz.zhaomingkeji.xyz/gtglvyaueh.html

[A14] 注释写法
来源：http://hz.feifeiyinyue.top/gtxzlmvjlj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.zhaomingkeji.xyz/gtjvovzfap.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.jyoumei.cn/gtuqjtwqos.html

JS:   // 单行；/* 多行 */
来源：http://hz.fzhhl.top/gtilfrnvcb.html

TS:   // 单行；/* 多行 */
来源：http://hz.cqqwz.cn/gtjlujhgks.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.jinqigfzy.top/gtcfajinso.html

Go:   // 单行；/* 多行 */
来源：http://hz.ydzc1.top/gtgnchovjf.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.jqgufenzy.top/gtafaxmtic.html

C#:   // 单行；/* 多行 */
来源：http://hz.wangshuangyany.cn/gtfqznlzul.html

[A15] 空值判断与默认值
来源：http://hz.yj20258888.top/gtsnmvksxa.html

Py:   value = data or "默认值"
来源：http://hz.ivvv.top/gtkmofkyge.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.hnqzz.top/gtaegmfwwy.html

JS:   const value = data ?? "默认值";
来源：http://hz.nanxinkj.top/gtupvgwzag.html

TS:   const value = data ?? "默认值";
来源：http://hz.tianlin.xyz/gtflveotlo.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.guowangkeji.top/gtenbholcy.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.havefunace.top/gtyhhqnefm.html

Ruby: value = data || "默认值"
来源：http://hz.tian-w.cn/gtftrcxbcm.html

C#:   var value = data ?? "默认值";
来源：http://hz.hysaishi.cn/gtjzbypxwb.html

[A16] 真假值判断规则
来源：http://hz.hywenlv.cn/gtyvkvcbab.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.sxryk.cn/gtbdeiotwi.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.ywan-chungtsiang.top/gtgmervqix.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.pycfn.com/gtnapaovsw.html

TS:   if (!x) {}
来源：http://hz.quarkkingdee.top/gtgvcaqmym.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.chenjidiqi.icu/gtszfaufqd.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.52xcode.cn/gtitqqerbs.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.xylfe.cn/gtcxomawez.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.zdqjudy.top/gtpeuqinsj.html

[A17] 位运算
来源：http://hz.hfpthk.cn/gtpoxxzsoq.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ehwqpu.com/gthndixxpn.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.zhoulong.xyz/gtkjjfrvdk.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yuanzhike.top/gtrievcsvj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.snrcjt.cn/gtdikxuccd.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.snrcjt.cn/gtcwwahkcn.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.sufxvd.cn/gtmirzthni.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.dianchejie.cn/gtzjvottzz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.cqqwz.cn/gtzyabbfzt.html

[A18] 字符与 ASCII 码互转
来源：http://hz.xylfe.cn/gtsqobbmzo.html

Py:   ord("A"); chr(65)
来源：http://hz.chenjidiqi.icu/gttnvyrfio.html

PHP:  ord("A"); chr(65)
来源：http://hz.tanke756.top/gtjvmadjqb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.zhongyouzk.top/gtfulfchqx.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.smart0.xyz/gtsgerhcsw.html

Java: (int) 'A'; (char) 65
来源：http://hz.zycfv.cn/gtynjschdk.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.0kj1m.cn/gtblxlbloj.html

Ruby: "A".ord; 65.chr
来源：http://hz.wangshuangyany.cn/gtmjffgyut.html

C#:   (int)'A'; (char)65
来源：http://hz.tian-w.cn/gtkmkkctsh.html

[A19] 交换两个变量
来源：http://hz.hywenlv.cn/gtpmocekza.html

Py:   a, b = b, a
来源：http://hz.tanke756.top/gtqhjtscpu.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.xuanzx.com/gtehjrlwis.html

JS:   [a, b] = [b, a];
来源：http://hz.cheryme.top/gtnbxbjpwp.html

TS:   [a, b] = [b, a];
来源：http://hz.havefunace.top/gtqnfugldp.html

Java: int t = a; a = b; b = t;
来源：http://hz.cucudq.cn/gtqsdavqma.html

Go:   a, b = b, a
来源：http://hz.ywan-chungtsiang.top/gtaphjyxfr.html

Ruby: a, b = b, a
来源：http://hz.sufxvd.cn/gtmnmzthcy.html

C#:   (a, b) = (b, a);
来源：http://hz.yuanzhike.top/gtnplmerqw.html

[A20] 读取标准输入
来源：http://hz.dianchejie.cn/gtxbeqogrh.html

Py:   name = input("请输入：")
来源：http://hz.shuidangran.top/gtviwavbxq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.gzhubu.top/gtdezudcxm.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.ivvv.top/gtcwptelve.html

TS:   // Node.js：readline 模块
来源：http://hz.52xcode.cn/gtwfmwdaay.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.fzhhl.top/gtgfmnqzjg.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.zhengqikj.top/gtjnmmstke.html

Ruby: gets.chomp
来源：http://hz.jinghuilouyu.cn/gtkoewdaub.html

C#:   Console.ReadLine();
来源：http://hz.birdmap.top/gtatfpohew.html

[A21] 保留指定小数位输出
来源：http://hz.tianlin.xyz/gtiwcbnmbr.html

Py:   f"{3.14159:.2f}"
来源：http://hz.chenjidiqi.icu/gtmnalyiku.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.meibo888.top/gtukzupfio.html

JS:   (3.14159).toFixed(2)
来源：http://hz.sysykeji.top/gtrrbttvsc.html

TS:   (3.14159).toFixed(2)
来源：http://hz.zhongyouzk.top/gtmjqmuqew.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.tian-w.cn/gtvxnaqlzg.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.guowangkeji.top/gtpapyhgix.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.snrcjt.cn/gthruoavbq.html

C#:   3.14159.ToString("F2")
来源：http://hz.jinyuanbaomall.cn/gtsveqhlyx.html

[A22] 获取字符串长度
来源：http://hz.zhaomingkeji.xyz/gtlxbosxok.html

Py:   len(s)
来源：http://hz.jlsjyb.cn/gtotcdtdkf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.zdqjudy.top/gtdtfknbqu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.jianghu66.top/gtplwwdzks.html

TS:   s.length
来源：http://hz.mhx1999.top/gtczuwagit.html

Java: s.length()
来源：http://hz.shanyushiyangkeji.top/gtxgdjbfia.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.jqgfzy.top/gtupyvdssb.html

Ruby: s.length
来源：http://hz.xuanzx.com/gthztsvggp.html

C#:   s.Length
来源：http://hz.hnxiangtu.top/gtmvbopwty.html

[A23] 大小写转换
来源：http://hz.ydjk.org.cn/gtmjmqzyfy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.xuanzx.com/gtptlpijiy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.tianlin.xyz/gtdemrmvwd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.yongpay.top/gtnddufovv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.aibaodan.cn/gtdxeoehxd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.jlsjyb.cn/gttoomzrdm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.tianlin.xyz/gtrshqxanj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.hammf.cn/gtzxcgslkc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.fzhhl.top/gtuqwkzzxa.html

[A24] 去除首尾空白
来源：http://hz.shuidangran.top/gtugkwkhpu.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.sxryk.cn/gthpilveye.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.iojbl.cn/gtfrjeixcj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zhixingplan.top/gtzcvrydii.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.mhx1999.top/gtnmjqjyat.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.andypj.xyz/gtyelqheeh.html

Go:   strings.TrimSpace(s)
来源：http://hz.meibo888.top/gtlakzitdk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.ehwqpu.com/gtedsgfbai.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.yj20258.top/gtazgqtnlw.html

[A25] 字符串比较
来源：http://hz.gotoacloud.top/gtcizhvsnb.html

Py:   s1 == s2; s1 != s2
来源：http://hz.kuanghao11.cn/gtaqmxwngb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.gzhubu.top/gtqhqyhihj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.vqdsnc.cn/gtacuaodlg.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yuanzhike.top/gtwhlxfhue.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.gzhubu.top/gtspenwmci.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.zhoulong.xyz/gtzdlecvwa.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.c1oappe.top/gtrteoklaf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.yj20258888.top/gteqmdmsqt.html

[A26] 类型转换总览
来源：http://hz.yanxiufei.cn/gtrdbacztm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.nwbrower.top/gtajyoaodv.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.haohaochexian.top/gtvypckksf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.zhiwuduotai.top/gtxkowtscn.html

TS:   Number() String() Boolean() x as number
来源：http://hz.daria6918.cn/gtijbytjnv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.wangdashe.top/gtvyjjqauj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.xuetiantiany.cn/gtvsaxqzgv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.yuxming.cn/gtfdmvysap.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.hongshengwenyu.top/gtwxvzglol.html

================================================================================
来源：http://hz.zdqjudy.top/gtvxadxzwi.html

B. 流程控制
来源：http://hz.jqgufenzy.top/gtohgtpgjy.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtksocgube.html

[B01] 条件判断 if / else
来源：http://hz.redwolf501.top/gtxcgrohbp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.ydjk.org.cn/gtcapdwshv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.zycfv.cn/gtvlhlqirr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.pengpengdd.cyou/gtmlfldkkm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.xinyue.icu/gtxvrllizw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.hywenlv.cn/gtcjoozwtr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.andypj.xyz/gtsmjmytyh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.xinyue.icu/gthhpwbjao.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.ivvv.top/gtdjjmzghi.html

[B02] 多分支 else if / elif
来源：http://hz.snrcjt.cn/gtweimwlnl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.tianlin.xyz/gtmuvhmnqi.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.zhixingplan.top/gtgrscuenv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.haohaochexian.top/gtlhudaksk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhengqikj.top/gtogtftvgk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cashguo.top/gtxjmnnvmt.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.yueranfly.top/gtojcevxxm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.jqgufenzy.top/gtjhsufawd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jqgfzy.top/gtpwixnsvt.html

[B03] switch / match / case
来源：http://hz.zhengqikj.top/gtymxhcddr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.gaohongyu789.top/gtngxxzeyl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.cheryme.top/gtcuwlrogv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.shanyushiyangkeji.top/gtzowtjojj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.hysaishi.cn/gtykcrezpm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.tian-w.cn/gthlrhgfpm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.0kj1m.cn/gtizioeyit.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.andypj.xyz/gtnzeyxvcw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.sysykeji.top/gthyslfgna.html

[B04] for 计数循环
来源：http://hz.yvedp.cn/gtxnvtfjof.html

Py:   for i in range(10): print(i)
来源：http://hz.hfpthk.cn/gtpgstkmzu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.zhoulong.xyz/gtdgdkpeur.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ivvv.top/gthfpziftr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.aibaodan.cn/gtpyuhwcsl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.svipenyu.cn/gtjtbwxobb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.ppjwa.cn/gthwsjpero.html

Ruby: 10.times { |i| puts i }
来源：http://hz.tian-w.cn/gtvkqogmvc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.ydzc1.top/gtmrdfplqg.html

[B05] 遍历数组 / 列表
来源：http://hz.yanxiufei.cn/gtcdgeshlt.html

Py:   for item in arr: print(item)
来源：http://hz.havefunace.top/gtjtbhjryx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.cheryme.top/gtzvjrisbh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.jyoumei.cn/gtyrqvkmco.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.yangfankeji.com/gtgpgjdabc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.zhengqikj.top/gthiunhkyt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.ehwqpu.com/gtsyacqpxv.html

Ruby: arr.each { |item| puts item }
来源：http://hz.smart0.xyz/gtsgyqepdm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.chenzaomai.com/gtixvdhcco.html

[B06] 遍历字典 / 对象
来源：http://hz.yonumen.top/gtywllloko.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.xziqi.cn/gtiywqmqqg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.aibaodan.cn/gtxyodfyge.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.birdmap.top/gtsdkkpbpr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhixingplan.top/gtnztijlol.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.hfpthk.cn/gtlnnqsyun.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.sysykeji.top/gtbwgptwce.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.haohaochexian.top/gtukchzkok.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.sweek.top/gtssoiemnt.html

[B07] while 循环
来源：http://hz.hongshengwenyu.top/gthmxikwvz.html

Py:   while i < 10: i += 1
来源：http://hz.zycfv.cn/gtotdrcdkz.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jiagoushi.top/gtuamcdtko.html

JS:   while (i < 10) { i++; }
来源：http://hz.yanxiufei.cn/gtlqsqovzi.html

TS:   while (i < 10) { i++; }
来源：http://hz.hywenlv.cn/gtxgbbzffk.html

Java: while (i < 10) { i++; }
来源：http://hz.birdmap.top/gtakobpjml.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.shuidangran.top/gtbaxcehlp.html

Ruby: while i < 10; i += 1; end
来源：http://hz.yongpay.top/gtxmjocqqf.html

C#:   while (i < 10) { i++; }
来源：http://hz.aibaodan.cn/gtcgsbvyov.html

[B08] do-while（至少执行一次）
来源：http://hz.cashguo.top/gtkvdqypzi.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.hywenlv.cn/gtusjwtktn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.havefunace.top/gtviszvkjo.html

JS:   do { i++; } while (i < 10);
来源：http://hz.meibo888.top/gtgjboefoy.html

TS:   do { i++; } while (i < 10);
来源：http://hz.316326.xyz/gtzkwwgseo.html

Java: do { i++; } while (i < 10);
来源：http://hz.yanxiufei.cn/gtgboqxbmm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.meibo888.top/gtrhzmpqst.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.zhijiandao.cn/gtimhipmlf.html

C#:   do { i++; } while (i < 10);
来源：http://hz.yuxming.cn/gtkxjjwhbe.html

[B09] break 与 continue
来源：http://hz.cucudq.cn/gtwgufbwpy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.haohaochexian.top/gtbjkjhann.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.fengsongda.top/gtwwqvqojo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.fengsongda.top/gtsenvptos.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ehwqpu.com/gtituiyxzz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yvedp.cn/gtcggrvyxq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.pycfn.com/gtjexqbqxc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.cdnleiting.top/gtwnselils.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhiwuduotai.top/gtmxemhaza.html

[B10] 遍历同时拿索引
来源：http://hz.fengsongda.top/gtjexgtion.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jinqigufen.top/gtusqvkmad.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yuanzhike.top/gtiwspejie.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.ehwqpu.com/gtcytmynko.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.316326.xyz/gtthrsuxhb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.svipenyu.cn/gtjveopgqb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yueranfly.top/gtovfisxcu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yj20258.top/gtrhlzzilm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.wangshuangyany.cn/gtltcqbtpx.html

[B11] 生成数字序列 / 区间
来源：http://hz.aibaodan.cn/gtychpxvim.html

Py:   list(range(0, 10, 2))
来源：http://hz.xylfe.cn/gtakmsotgv.html

PHP:  range(0, 10, 2);
来源：http://hz.shanyushiyangtech.top/gtdllhehnx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xylfe.cn/gtrcljaswe.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.havefunace.top/gtfvchvhzv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jyoumei.cn/gtvngbrcxe.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.ppjwa.cn/gtidwioqdq.html

Ruby: (0...10).step(2).to_a
来源：http://hz.wangdashe.top/gtzfgszfmr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yongpay.top/gtjqfcbpvu.html

[B12] 跳出多层循环
来源：http://hz.zhixingplan.top/gtmnwdxqdr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.0kj1m.cn/gtmlnueejz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.guowangkeji.top/gtgtitytxq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cucudq.cn/gtmumlisbm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xingfuxueyuan.xyz/gtbjlmjdya.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jqgufenzy.top/gtylgvumcz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yanxiufei.cn/gtgomnyahc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yanxiufei.cn/gtxlfvozcj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.guannengcc.top/gtvcartcml.html

[B13] 判断是否为数字
来源：http://hz.hfpthk.cn/gtbtpvdkfh.html

Py:   isinstance(x, (int, float))
来源：http://hz.yuxming.cn/gtbfjqpemm.html

PHP:  is_numeric($x)
来源：http://hz.sxryk.cn/gthihaghuy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jyoumei.cn/gtzieppbye.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.tian-w.cn/gthkdnpbgk.html

Java: x instanceof Number
来源：http://hz.chenlongwang.top/gtznymrbjy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zdqjudy.top/gtfjdjkifb.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hnqzz.top/gtsvmlvpjp.html

C#:   x is int or double or decimal
来源：http://hz.zhiwuduotai.top/gtcuvlajip.html

[B14] 判断值是否在集合内
来源：http://hz.xziqi.cn/gtmvfzdmto.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zdqjudy.top/gtqxjmjdmm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yj20258.top/gtgdgevdyc.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zhijiandao.cn/gtocwohbdt.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.meibo888.top/gtowfcewug.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yj20258.top/gtmilyrpqc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.fengsongda.top/gtlxrtbwmk.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.cashguo.top/gtftcergnc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.9152youxi.cn/gtqkrdptht.html

[B15] 布尔运算与取反
来源：http://hz.jinqigufen.top/gtfmjfhfuh.html

Py:   a and b or not c
来源：http://hz.hysaishi.cn/gtgqzwnvhj.html

PHP:  $a && $b || !$c
来源：http://hz.vqdsnc.cn/gtwdzqucwy.html

JS:   a && b || !c
来源：http://hz.xinyue.icu/gtynmtmigd.html

TS:   a && b || !c
来源：http://hz.xuetiantiany.cn/gtqgsdeeod.html

Java: a && b || !c
来源：http://hz.shzxlz.cn/gtvtckpwnm.html

Go:   a && b || !c
来源：http://hz.yonumen.top/gtlibxjnqq.html

Ruby: a && b || !c
来源：http://hz.kuanghao11.cn/gttkypiecx.html

C#:   a && b || !c
来源：http://hz.xuetiantiany.cn/gtwuomzgeg.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jinyuanbaomall.cn/gtzxfjdubd.html

Py:   if not data: return
来源：http://hz.0kj1m.cn/gtzmktafvq.html

PHP:  if (!$data) { return; }
来源：http://hz.gotoacloud.top/gtwpaekutb.html

JS:   if (!data) return;
来源：http://hz.quarkkingdee.top/gtqyntyagu.html

TS:   if (!data) return;
来源：http://hz.yangfankeji.com/gtmnsaaxvk.html

Java: if (data == null) return;
来源：http://hz.zhijiandao.cn/gtiygykmjo.html

Go:   if data == nil { return }
来源：http://hz.zhengqikj.top/gthvuenrhf.html

Ruby: return if data.nil?
来源：http://hz.gogol.net.cn/gtdsxesyfb.html

C#:   if (data == null) return;
来源：http://hz.havefunace.top/gtenfedzee.html

================================================================================
来源：http://hz.guannengcc.top/gtfobfgsmb.html

C. 函数与作用域
来源：http://hz.shuidangran.top/gtmnrvhafb.html

================================================================================
来源：http://hz.yongpay.top/gtappxdqhj.html

[C01] 定义函数
来源：http://hz.jqgfzy.top/gtkggzrxea.html

Py:   def add(a, b): return a + b
来源：http://hz.ydjk.org.cn/gtzalqrssh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.snrcjt.cn/gtgyykgfof.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.gotoacloud.top/gtkfoqitqm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xuanzx.com/gtkpqgdqvd.html


<!-- 参考信息 -->