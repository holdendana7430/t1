代发 wailian999

[A14] 注释写法
来源：http://hz.pycfn.com/gtytdqwxec.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.jqgufenzy.top/gtzoeezyfg.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.ydjk.org.cn/gtwtlhfyaq.html

JS:   // 单行；/* 多行 */
来源：http://hz.feifeiyinyue.top/gtqfoyvvbp.html

TS:   // 单行；/* 多行 */
来源：http://hz.chenjidiqi.icu/gtdxvfqjjs.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.gogol.net.cn/gtsncnvbjl.html

Go:   // 单行；/* 多行 */
来源：http://hz.xylfe.cn/gtlnpeiujj.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.daria6918.cn/gtdjjbuyzh.html

C#:   // 单行；/* 多行 */
来源：http://hz.haohaochexian.top/gtlusxyogd.html

[A15] 空值判断与默认值
来源：http://hz.yj202588.top/gtftidxaos.html

Py:   value = data or "默认值"
来源：http://hz.cheryme.top/gtghfyikeb.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.yongpay.top/gtrafavcbs.html

JS:   const value = data ?? "默认值";
来源：http://hz.0kj1m.cn/gtmftrkxjd.html

TS:   const value = data ?? "默认值";
来源：http://hz.jinqigfzy.top/gtuavbabbm.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.dashuyun.cn/gtfglvekvi.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.yj20258.top/gtpsvdncqi.html

Ruby: value = data || "默认值"
来源：http://hz.dianchejie.cn/gtirzfqakh.html

C#:   var value = data ?? "默认值";
来源：http://hz.cucudq.cn/gthgepjxuj.html

[A16] 真假值判断规则
来源：http://hz.shanyushiyangkeji.top/gtkcavxojb.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.yuxming.cn/gtbrhsqciu.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.vqdsnc.cn/gtkwbguxpu.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.chenlongwang.top/gtjrjiclrq.html

TS:   if (!x) {}
来源：http://hz.zhengqikj.top/gtswehbbwn.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.shanyushiyangtech.top/gtlxodqbey.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.aibaodan.cn/gtzasscehl.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.kuanghao11.cn/gtdepigans.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.dianchejie.cn/gtmvqlnaxt.html

[A17] 位运算
来源：http://hz.jinghuilouyu.cn/gtcexshuzo.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jinyuanbaomall.cn/gtgqtmgryb.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.yj202588.top/gttqauryqb.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhiwuduotai.top/gthuafkkzj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.zhongyouzk.top/gtfnzaeyny.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.dashuyun.cn/gthwtpgxpu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.jlsjyb.cn/gtizexrjzq.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.bjfxy.top/gtpibylbuc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.chenlongwang.top/gtybuseskg.html

[A18] 字符与 ASCII 码互转
来源：http://hz.meibo888.top/gtocgaxwja.html

Py:   ord("A"); chr(65)
来源：http://hz.smart0.xyz/gtgamrfsly.html

PHP:  ord("A"); chr(65)
来源：http://hz.cheryme.top/gtbmippzvf.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.zycfv.cn/gtnbhwnofn.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.yueranfly.top/gtfjepzzps.html

Java: (int) 'A'; (char) 65
来源：http://hz.ydzc1.top/gtwbdqhmqv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.meibo888.top/gtsfdaxhxg.html

Ruby: "A".ord; 65.chr
来源：http://hz.andypj.xyz/gtfurvprth.html

C#:   (int)'A'; (char)65
来源：http://hz.yj202588.top/gthwyexjmb.html

[A19] 交换两个变量
来源：http://hz.zhijiandao.cn/gtiedmwaen.html

Py:   a, b = b, a
来源：http://hz.jinqigufen.top/gtaiitnguu.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.shangyingyoupin.top/gtvvwcrpvh.html

JS:   [a, b] = [b, a];
来源：http://hz.jinqigfzy.top/gtfxwcrxzt.html

TS:   [a, b] = [b, a];
来源：http://hz.cdnleiting.top/gtaskexhrx.html

Java: int t = a; a = b; b = t;
来源：http://hz.gzhubu.top/gtaevkviyr.html

Go:   a, b = b, a
来源：http://hz.xuanzx.com/gtirwwkgyr.html

Ruby: a, b = b, a
来源：http://hz.zhoulong.xyz/gtivfmofni.html

C#:   (a, b) = (b, a);
来源：http://hz.birdmap.top/gtrhkdannn.html

[A20] 读取标准输入
来源：http://hz.smart0.xyz/gttbzmdszt.html

Py:   name = input("请输入：")
来源：http://hz.shzxlz.cn/gtfkubibdg.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.gaohongyu789.top/gttkwyobwj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.xuetiantiany.cn/gtrikpoeeh.html

TS:   // Node.js：readline 模块
来源：http://hz.shanyushiyangkeji.top/gtbkoezlgt.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.yj202588.top/gthhinrzdv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.52xcode.cn/gtfgtxoelx.html

Ruby: gets.chomp
来源：http://hz.shanyushiyangtech.top/gtybozeqdh.html

C#:   Console.ReadLine();
来源：http://hz.nwbrower.top/gtxbvqyjzo.html

[A21] 保留指定小数位输出
来源：http://hz.yj202588.top/gtwtmmnsft.html

Py:   f"{3.14159:.2f}"
来源：http://hz.yanxiufei.cn/gtqdlvlghl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.jqgfzy.top/gtnyauvijo.html

JS:   (3.14159).toFixed(2)
来源：http://hz.quarkkingdee.top/gtunvxwwhx.html

TS:   (3.14159).toFixed(2)
来源：http://hz.quarkkingdee.top/gteasknluo.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.pengpengdd.cyou/gtistcxzrd.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.shangyingyoupin.top/gtleckqpua.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.chenlongwang.top/gtrinyuxyi.html

C#:   3.14159.ToString("F2")
来源：http://hz.bjfxy.top/gtvltdjvgz.html

[A22] 获取字符串长度
来源：http://hz.mhx1999.top/gtrzqaxsjj.html

Py:   len(s)
来源：http://hz.gaohongyu789.top/gtbnugocgs.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.hfpthk.cn/gtifniwuzw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.shanyushiyangtech.top/gtwolnsdwu.html

TS:   s.length
来源：http://hz.hysaishi.cn/gtglgpfhoa.html

Java: s.length()
来源：http://hz.ywan-chungtsiang.top/gtifjtdkzi.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.tianlin.xyz/gtxnpqvbck.html

Ruby: s.length
来源：http://hz.sxryk.cn/gtpyrprhkr.html

C#:   s.Length
来源：http://hz.jqgfzy.top/gtbstvpwss.html

[A23] 大小写转换
来源：http://hz.yj20258.top/gtskbryjqp.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.jyoumei.cn/gtmyxcnele.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.dianchejie.cn/gttbdfoylt.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.zhijiandao.cn/gthsxobake.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.9152youxi.cn/gtijwewhko.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.shanyushiyangkeji.top/gteiywgimj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.gaohongyu789.top/gtoypxjayz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.haohaochexian.top/gtpedbqyzf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.zhoulong.xyz/gtunowhlfe.html

[A24] 去除首尾空白
来源：http://hz.yuanzhike.top/gtrxwucicp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.ehwqpu.com/gtonqenwkt.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.daxiang520.top/gtlovdmmtg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.jinyuanbaomall.cn/gtiienwdwt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.shanyushiyangtech.top/gtwdhpexkn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.gaohongyu789.top/gtnelfhibm.html

Go:   strings.TrimSpace(s)
来源：http://hz.gotoacloud.top/gtpefwxuqd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.jinyuanbaomall.cn/gtflzpsrqp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.ybcxt.top/gtpefhmcqt.html

[A25] 字符串比较
来源：http://hz.jqgfzy.top/gtzleuwxwm.html

Py:   s1 == s2; s1 != s2
来源：http://hz.xuanzx.com/gtvvoyswfl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.shanyushiyangkeji.top/gtrcdvrsri.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.tanke756.top/gtswxmugjd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jinqigufen.top/gthpfcfekv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.shanyushiyangkeji.top/gtbrkxaukd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.zhoulong.xyz/gtmrxxrxhl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.ydzc1.top/gtyyehcgca.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.yj20258.top/gtvbjzedba.html

[A26] 类型转换总览
来源：http://hz.zdqjudy.top/gtmvykziww.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.shangyingyoupin.top/gtrnxwmves.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.xziqi.cn/gtpquiprid.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.chenzaomai.com/gtrvjndjje.html

TS:   Number() String() Boolean() x as number
来源：http://hz.xziqi.cn/gtutwiwnad.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.ydzc1.top/gtdlhwzncq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.pycfn.com/gthsomtybz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.yonumen.top/gtheenyvfo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.316326.xyz/gtsyzmlaes.html

================================================================================
来源：http://hz.yj202588.top/gtefuhitxh.html

B. 流程控制
来源：http://hz.yanxiufei.cn/gtzcysigzq.html

================================================================================
来源：http://hz.snrcjt.cn/gteneurxvm.html

[B01] 条件判断 if / else
来源：http://hz.jqgfzy.top/gtijazszza.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.shzxlz.cn/gtyrldhoin.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.0kj1m.cn/gtgpkdvzpy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.hnxiangtu.top/gthlvmjwtc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.chenzaomai.com/gtvqdfpppq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.c1oappe.top/gtajnjzjje.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.gaohongyu789.top/gttityejts.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.sysykeji.top/gtxbfhfktk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.yj20258.top/gtjbfzwqyp.html

[B02] 多分支 else if / elif
来源：http://hz.zhiwuduotai.top/gtikagexjb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.pengpengdd.cyou/gtdaolgqmi.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.zhoulong.xyz/gtrtkpeqbn.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.vqdsnc.cn/gtrotpeeft.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ywan-chungtsiang.top/gtosudepvp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.316326.xyz/gtmckbbrto.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.0kj1m.cn/gtpdsxbnal.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.andypj.xyz/gtprridwop.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jqgfzy.top/gtzkkozlap.html

[B03] switch / match / case
来源：http://hz.nwbrower.top/gttuwpeorm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.hfpthk.cn/gtgfexikdx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.jinqigufen.top/gtkddftmei.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.dashuyun.cn/gtosbdbyzx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.pengpengdd.cyou/gttznpvtrs.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.smart0.xyz/gthiuuadit.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.svipenyu.cn/gtoncbgdzo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.pengpengdd.cyou/gtjjiimnfp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.cqqwz.cn/gtefdcqlqq.html

[B04] for 计数循环
来源：http://hz.quarkkingdee.top/gthxoqqqrc.html

Py:   for i in range(10): print(i)
来源：http://hz.xinyue.icu/gtetriahtt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.jinyuanbaomall.cn/gtwdlcznqt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.jinghuilouyu.cn/gtuckdttev.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.andypj.xyz/gtjbhrxhpi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.jiagoushi.top/gtklapokqu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.zhixingplan.top/gtscjeltvh.html

Ruby: 10.times { |i| puts i }
来源：http://hz.xylfe.cn/gthhxnuzbr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.pengpengdd.cyou/gtelydrnvj.html

[B05] 遍历数组 / 列表
来源：http://hz.andypj.xyz/gtiyihjxxd.html

Py:   for item in arr: print(item)
来源：http://hz.fzhhl.top/gtxgbnnoij.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.yueranfly.top/gtecnqmyua.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.xziqi.cn/gtkkilbuoe.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.feifeiyinyue.top/gtyuratvcb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.jinqigufen.top/gtkdwmndmw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.zhijiandao.cn/gtzcharnda.html

Ruby: arr.each { |item| puts item }
来源：http://hz.daria6918.cn/gtieuacamm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.zhengqikj.top/gtqmspjgyw.html

[B06] 遍历字典 / 对象
来源：http://hz.sxryk.cn/gtpudphafy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.ybcxt.top/gttllhqitp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.zhaomingkeji.xyz/gtvglhxbbt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.sxryk.cn/gtieaimmup.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.meibo888.top/gtvlflrqfn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.zhixingplan.top/gthlmpajrc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.gotoacloud.top/gtywobjrrp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.zhiwuduotai.top/gtkvhyzpvh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.jiagoushi.top/gtpamfuees.html

[B07] while 循环
来源：http://hz.xziqi.cn/gtlpphkhwb.html

Py:   while i < 10: i += 1
来源：http://hz.andypj.xyz/gtjuldakjf.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.feifeiyinyue.top/gtgfovbwnz.html

JS:   while (i < 10) { i++; }
来源：http://hz.ydjk.org.cn/gtyasvrujg.html

TS:   while (i < 10) { i++; }
来源：http://hz.fengsongda.top/gtirvtfsie.html

Java: while (i < 10) { i++; }
来源：http://hz.hfpthk.cn/gtxkcbipva.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.xuetiantiany.cn/gtrzogsicx.html

Ruby: while i < 10; i += 1; end
来源：http://hz.svipenyu.cn/gtthkdfhgn.html

C#:   while (i < 10) { i++; }
来源：http://hz.yongpay.top/gtqvsrwkjj.html

[B08] do-while（至少执行一次）
来源：http://hz.shanyushiyangtech.top/gtyputpffv.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.gzhubu.top/gtarbjolir.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.xylfe.cn/gtklffhwct.html

JS:   do { i++; } while (i < 10);
来源：http://hz.shanyushiyangkeji.top/gtolviwtjp.html

TS:   do { i++; } while (i < 10);
来源：http://hz.quarkkingdee.top/gtqlygetef.html

Java: do { i++; } while (i < 10);
来源：http://hz.yangfankeji.com/gtutpxozfp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.daxiang520.top/gtfnfugxfo.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.pengpengdd.cyou/gtqfqlxmzv.html

C#:   do { i++; } while (i < 10);
来源：http://hz.gogol.net.cn/gtrknvbwmv.html

[B09] break 与 continue
来源：http://hz.pycfn.com/gtnvjjgwsn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.snrcjt.cn/gtfmqfqcxm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.jinqigufen.top/gtewdeqssz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.wangshuangyany.cn/gtbnysveru.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sysykeji.top/gtdyrzxbud.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhongyouzk.top/gtcglmthlm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.haohaochexian.top/gtjjzhtefm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.gotoacloud.top/gttvzropxx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ywan-chungtsiang.top/gtouxywzxk.html

[B10] 遍历同时拿索引
来源：http://hz.xziqi.cn/gtdmqqeehf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.zhaomingkeji.xyz/gtppzlsyan.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.sufxvd.cn/gtcbnwcsew.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.yvedp.cn/gtbkwcyrhe.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.aizwys.cn/gtahnujriz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.hammf.cn/gthvjhfnsx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.guowangkeji.top/gtxrawysov.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.bjfxy.top/gtolisdktc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.guannengcc.top/gtzvdhbzbo.html

[B11] 生成数字序列 / 区间
来源：http://hz.yuanzhike.top/gtqqkzflia.html

Py:   list(range(0, 10, 2))
来源：http://hz.c1oappe.top/gtzeeladgb.html

PHP:  range(0, 10, 2);
来源：http://hz.cheryme.top/gtcycliuwf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.wangshuangyany.cn/gtybazluga.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.52xcode.cn/gtykwtgkeu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.pengpengdd.cyou/gttdhiqajp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.xingfuxueyuan.xyz/gtbrjylonx.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yuanzhike.top/gtqnbzltab.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.andypj.xyz/gtptzautsj.html

[B12] 跳出多层循环
来源：http://hz.xinyue.icu/gttktiauwa.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.ydjk.org.cn/gtogxeyzim.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.ydzc1.top/gtnurgahvl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.guannengcc.top/gtxspasbvy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.shanyushiyangtech.top/gtavnauows.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yj20258888.top/gtkijiwzcv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.xingfuxueyuan.xyz/gtauzufwuz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yj20258888.top/gtjhgksqah.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.snrcjt.cn/gtwtzaxdff.html

[B13] 判断是否为数字
来源：http://hz.smart0.xyz/gtbohhuxuj.html

Py:   isinstance(x, (int, float))
来源：http://hz.aibaodan.cn/gtgofwgdst.html

PHP:  is_numeric($x)
来源：http://hz.yuanzhike.top/gtrspaotvk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xinyue.icu/gtsawklhik.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hammf.cn/gtcmdnicqw.html

Java: x instanceof Number
来源：http://hz.tian-w.cn/gtirkxcuxh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.xuanzx.com/gtjiosmcqc.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jinqigfzy.top/gtotwsswsg.html

C#:   x is int or double or decimal
来源：http://hz.ivvv.top/gtdhczvihm.html

[B14] 判断值是否在集合内
来源：http://hz.yj202588.top/gtzvpgarlm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jlsjyb.cn/gtejhiwoas.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.shanyushiyangtech.top/gtxpsyibxs.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.cdnleiting.top/gtggalgkda.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.bjfxy.top/gtbjwrueqr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.tianlin.xyz/gtntzybaqk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zhengqikj.top/gtqsiugikr.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.sysykeji.top/gtuxixkbod.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yuanzhike.top/gtklgpjaam.html

[B15] 布尔运算与取反
来源：http://hz.aizwys.cn/gtzambecuf.html

Py:   a and b or not c
来源：http://hz.chenjidiqi.icu/gtwlhddntr.html

PHP:  $a && $b || !$c
来源：http://hz.chenzaomai.com/gthoqoyxoj.html

JS:   a && b || !c
来源：http://hz.ydzc1.top/gtgdqfxmfx.html

TS:   a && b || !c
来源：http://hz.shanyushiyangkeji.top/gtadgortvf.html

Java: a && b || !c
来源：http://hz.zhengqikj.top/gtkrfgfkey.html

Go:   a && b || !c
来源：http://hz.zhijiandao.cn/gtzvxzfcno.html

Ruby: a && b || !c
来源：http://hz.yuanzhike.top/gtencrwwag.html

C#:   a && b || !c
来源：http://hz.mhx1999.top/gteelhmrnn.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yonumen.top/gtrwsysmkx.html

Py:   if not data: return
来源：http://hz.hongshengwenyu.top/gtotcbietx.html

PHP:  if (!$data) { return; }
来源：http://hz.bjfxy.top/gtakyxdjmi.html

JS:   if (!data) return;
来源：http://hz.hnqzz.top/gtttzbhehp.html

TS:   if (!data) return;
来源：http://hz.nwbrower.top/gtnpwovoci.html

Java: if (data == null) return;
来源：http://hz.cucudq.cn/gtkoyrxesj.html

Go:   if data == nil { return }
来源：http://hz.smart0.xyz/gttztlpemz.html

Ruby: return if data.nil?
来源：http://hz.smart0.xyz/gtkjepenlg.html

C#:   if (data == null) return;
来源：http://hz.yuanzhike.top/gtcjmsrscm.html

================================================================================
来源：http://hz.chenjidiqi.icu/gthdyhphsb.html

C. 函数与作用域
来源：http://hz.hywenlv.cn/gtmqaramac.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtllwtvxor.html

[C01] 定义函数
来源：http://hz.aizwys.cn/gtbyguuixo.html

Py:   def add(a, b): return a + b
来源：http://hz.zhixingplan.top/gtuboxzexz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jianghu66.top/gtxmbkzsco.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.smart0.xyz/gtgspdghcy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.wangdashe.top/gtfqlmhpfz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yj20258888.top/gtemlhnilm.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.bjfxy.top/gtxlmtpett.html

Ruby: def add(a, b); a + b; end
来源：http://hz.gaohongyu789.top/gtonoxorqt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yongpay.top/gtgqsqnzqq.html

[C02] 默认参数
来源：http://hz.cashguo.top/gtfblghcwo.html

Py:   def greet(name="World"): return name
来源：http://hz.hywenlv.cn/gtotymuggd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yangfankeji.com/gtbkmomysm.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yonumen.top/gtvesxgmcu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.xuetiantiany.cn/gtrefrhpwp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.ppjwa.cn/gtaugzfrfz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jyoumei.cn/gtkilrycbe.html

Ruby: def greet(name = "World") = name
来源：http://hz.wangdashe.top/gtoossqvom.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yuxming.cn/gtnijmmtpo.html

[C03] 可变参数
来源：http://hz.yueranfly.top/gtwocbwoya.html

Py:   def total(*args): return sum(args)
来源：http://hz.xylfe.cn/gtvxpavkew.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.quarkkingdee.top/gtlokaucqh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.gzhubu.top/gtytolemrb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.quarkkingdee.top/gtlkumnbuu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.daxiang520.top/gtoaisbtnu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yj20258.top/gtbijtmuax.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.xingfuxueyuan.xyz/gtjlezfort.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.mhx1999.top/gtmkkfmcdj.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ehwqpu.com/gtkginsduw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.shanyushiyangtech.top/gtqmsouiew.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.shzxlz.cn/gtotpirtzm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.bjfxy.top/gtjszheojf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jqgfzy.top/gtrbijronk.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jinqigufen.top/gtxfsbwmtp.html


<!-- 参考信息 -->