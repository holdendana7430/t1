代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://hz.hammf.cn/gthqyfsbyh.html

[A11] 条件表达式（三元）
来源：http://hz.xziqi.cn/gtbkwpkhju.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.shanyushiyangkeji.top/gtcqgzfpyh.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.tianlin.xyz/gtmlhvldka.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.yj202588.top/gtnrqfbtoz.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.zhijiandao.cn/gtfrmubmis.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.hongshengwenyu.top/gtayubqdny.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.bjfxy.top/gtbsxtefhl.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.zhijiandao.cn/gtcbzrelec.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.svipenyu.cn/gttrnwvaui.html

[A12] 字符串插值 / 格式化
来源：http://hz.yj20258.top/gthjuniqzp.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.sweek.top/gtyqdkzhfe.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.tanke756.top/gtdfwqhstj.html

JS:   `Hello, ${name}!`
来源：http://hz.tanke756.top/gtzyvltpck.html

TS:   `Hello, ${name}!`
来源：http://hz.smart0.xyz/gtczrbmpmq.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.daria6918.cn/gtomvdzvvr.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.ydzc1.top/gtwlmnyofd.html

Ruby: "Hello, #{name}!"
来源：http://hz.52xcode.cn/gtrrxbbqcm.html

C#:   $"Hello, {name}!"
来源：http://hz.jlsjyb.cn/gtcwiwekoh.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.cucudq.cn/gtmvzvbecx.html

Py:   "第一行\n第二行"
来源：http://hz.xziqi.cn/gtinapowxr.html

PHP:  "第一行\n第二行"
来源：http://hz.316326.xyz/gtutypbtet.html

JS:   "第一行\n第二行"
来源：http://hz.dianchejie.cn/gtdwqrwonk.html

TS:   "第一行\n第二行"
来源：http://hz.zhongyouzk.top/gtqbaiwnid.html

Java: "第一行\n第二行"
来源：http://hz.9152youxi.cn/gtsivpqppv.html

Go:   "第一行\n第二行"
来源：http://hz.yongpay.top/gthdtkeugn.html

Ruby: "第一行\n第二行"
来源：http://hz.guannengcc.top/gtkwuadedc.html

C#:   "第一行\n第二行"
来源：http://hz.nwbrower.top/gtqwefomvn.html

[A14] 注释写法
来源：http://hz.ydzc1.top/gtssucylrl.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.ehwqpu.com/gtjkqpslaz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.wangshuangyany.cn/gtiebhpwlt.html

JS:   // 单行；/* 多行 */
来源：http://hz.fengsongda.top/gtzbtxgirv.html

TS:   // 单行；/* 多行 */
来源：http://hz.zhaomingkeji.xyz/gtomumkmcs.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.zhaomingkeji.xyz/gttastsynk.html

Go:   // 单行；/* 多行 */
来源：http://hz.yvedp.cn/gtpagfnayp.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.ybcxt.top/gtnnopyhen.html

C#:   // 单行；/* 多行 */
来源：http://hz.nanxuanxn.top/gtmlguprow.html

[A15] 空值判断与默认值
来源：http://hz.cqqwz.cn/gtrjqfwfnz.html

Py:   value = data or "默认值"
来源：http://hz.daria6918.cn/gtetheqlgn.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.nanxuanxn.top/gtfvkglczq.html

JS:   const value = data ?? "默认值";
来源：http://hz.c1oappe.top/gtmgfeqkfb.html

TS:   const value = data ?? "默认值";
来源：http://hz.jqgfzy.top/gtwbjmfyxy.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.jianghu66.top/gtgzjwxknk.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.yj20258.top/gtvvsykdzg.html

Ruby: value = data || "默认值"
来源：http://hz.shanyushiyangkeji.top/gtljdqchpf.html

C#:   var value = data ?? "默认值";
来源：http://hz.quarkkingdee.top/gtvddbwvsq.html

[A16] 真假值判断规则
来源：http://hz.iojbl.cn/gtczqkpaqi.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.aibaodan.cn/gtxgkumaol.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.jqgufenzy.top/gtfobpdwjl.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.ehwqpu.com/gtktgrfyei.html

TS:   if (!x) {}
来源：http://hz.birdmap.top/gtxnbqtntt.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.hammf.cn/gtpmubnilf.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.jinqigufen.top/gtzczdauws.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.ppjwa.cn/gtaoamfcos.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.xuanzx.com/gtmpltjsms.html

[A17] 位运算
来源：http://hz.jqgufenzy.top/gtylyqbgmr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yueranfly.top/gtirrfxdqp.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.zhijiandao.cn/gtkbgfelmr.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yangfankeji.com/gteltlpyox.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.zhiwuduotai.top/gtwogingiu.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.tianlin.xyz/gtfbalvfhm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.cheryme.top/gtwdcndhvy.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.cashguo.top/gtrzdcfvfb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.cucudq.cn/gtjhyscnom.html

[A18] 字符与 ASCII 码互转
来源：http://hz.tanke756.top/gtftohpwjg.html

Py:   ord("A"); chr(65)
来源：http://hz.fengsongda.top/gtocdugxel.html

PHP:  ord("A"); chr(65)
来源：http://hz.guowangkeji.top/gtjqogvjgi.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.iojbl.cn/gtmcdtoqwy.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.zhaomingkeji.xyz/gtspesvjtc.html

Java: (int) 'A'; (char) 65
来源：http://hz.xylfe.cn/gtpifoqjkg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.yuxming.cn/gtkxccqijk.html

Ruby: "A".ord; 65.chr
来源：http://hz.feifeiyinyue.top/gtdeowcprk.html

C#:   (int)'A'; (char)65
来源：http://hz.316326.xyz/gtgqhwgnas.html

[A19] 交换两个变量
来源：http://hz.sxryk.cn/gtdhnhytng.html

Py:   a, b = b, a
来源：http://hz.hongshengwenyu.top/gtunpugcfb.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.kuanghao11.cn/gtdzdhnfal.html

JS:   [a, b] = [b, a];
来源：http://hz.vqdsnc.cn/gtcgeoaipx.html

TS:   [a, b] = [b, a];
来源：http://hz.daria6918.cn/gtxcgzelze.html

Java: int t = a; a = b; b = t;
来源：http://hz.hammf.cn/gtlfbhmbds.html

Go:   a, b = b, a
来源：http://hz.yuanzhike.top/gtkrhmvend.html

Ruby: a, b = b, a
来源：http://hz.tanke756.top/gtrxbwmuln.html

C#:   (a, b) = (b, a);
来源：http://hz.zdqjudy.top/gtsqkuypbc.html

[A20] 读取标准输入
来源：http://hz.c1oappe.top/gtbnhctbkn.html

Py:   name = input("请输入：")
来源：http://hz.zhongyouzk.top/gtairkbhus.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.shzxlz.cn/gtyaznstwo.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.guowangkeji.top/gtwxujqone.html

TS:   // Node.js：readline 模块
来源：http://hz.xuanzx.com/gtdlmxioep.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.xinyue.icu/gtiayjuaxi.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.xingfuxueyuan.xyz/gtlrcyjpem.html

Ruby: gets.chomp
来源：http://hz.shangyingyoupin.top/gtsegzbhwa.html

C#:   Console.ReadLine();
来源：http://hz.shanyushiyangtech.top/gtpmwomenx.html

[A21] 保留指定小数位输出
来源：http://hz.zhixingplan.top/gtucblhglw.html

Py:   f"{3.14159:.2f}"
来源：http://hz.yuxming.cn/gtcwuxrzoz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.daxiang520.top/gtvulctulr.html

JS:   (3.14159).toFixed(2)
来源：http://hz.wangshuangyany.cn/gtgfahwonk.html

TS:   (3.14159).toFixed(2)
来源：http://hz.yuanzhike.top/gtxfcuqfed.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.aibaodan.cn/gtzizbpciz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.yanxiufei.cn/gtouquysgh.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.yanxiufei.cn/gtgvjlcewu.html

C#:   3.14159.ToString("F2")
来源：http://hz.52xcode.cn/gtwtzrdzdq.html

[A22] 获取字符串长度
来源：http://hz.svipenyu.cn/gtddkmaxwk.html

Py:   len(s)
来源：http://hz.yueranfly.top/gtuckyncue.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.feifeiyinyue.top/gtnflfgyux.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.chenjidiqi.icu/gtqqkoclgz.html

TS:   s.length
来源：http://hz.guowangkeji.top/gtelrqhgmc.html

Java: s.length()
来源：http://hz.mhx1999.top/gtulytnctc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.fzhhl.top/gthzvksxif.html

Ruby: s.length
来源：http://hz.jqgufenzy.top/gtafjrktgz.html

C#:   s.Length
来源：http://hz.zhengqikj.top/gtzbulyyyp.html

[A23] 大小写转换
来源：http://hz.316326.xyz/gtqrdrhmku.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.cdnleiting.top/gtyrzxvbqr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.xingfuxueyuan.xyz/gtudjosllv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.52xcode.cn/gtbayfyzsl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.tianlin.xyz/gtcvhsiwvf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.shanyushiyangkeji.top/gtkcxlbjxg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.c1oappe.top/gtmzhokuls.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.jinqigfzy.top/gtqkqikvbp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.yj20258888.top/gtcywjjaee.html

[A24] 去除首尾空白
来源：http://hz.yj20258888.top/gtfnuplqyb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.shanyushiyangkeji.top/gtmjcymjao.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.xuanzx.com/gtkbogryfl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.hongshengwenyu.top/gtuavjlsoj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zhoulong.xyz/gtjerspdyf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.gogol.net.cn/gtlhdexjcg.html

Go:   strings.TrimSpace(s)
来源：http://hz.jlsjyb.cn/gtcgxitcow.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.cashguo.top/gtxujfvyfa.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.zhoulong.xyz/gtoexatahw.html

[A25] 字符串比较
来源：http://hz.cheryme.top/gtpcigopgm.html

Py:   s1 == s2; s1 != s2
来源：http://hz.jinghuilouyu.cn/gtuduggqis.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.tanke756.top/gtzfensrbo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.snrcjt.cn/gtebrprqnd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.gaohongyu789.top/gthnswfaqx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.xylfe.cn/gtunlfmfhj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.jinghuilouyu.cn/gtqzgghfdc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.316326.xyz/gtinnotkle.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.jinyuanbaomall.cn/gtrgzapzzp.html

[A26] 类型转换总览
来源：http://hz.sxryk.cn/gtebupofmv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.wangshuangyany.cn/gtmeptedjv.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.jiagoushi.top/gtswisucsd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.yangfankeji.com/gtgeroxqvx.html

TS:   Number() String() Boolean() x as number
来源：http://hz.andypj.xyz/gtgwtxzspq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.shuidangran.top/gtstipmsbv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.meibo888.top/gtnlxcnnsj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.guowangkeji.top/gtmqmtpufr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.sxryk.cn/gtteireivt.html

================================================================================
来源：http://hz.tianlin.xyz/gtcdhnllxh.html

B. 流程控制
来源：http://hz.aizwys.cn/gtvtxnyiqr.html

================================================================================
来源：http://hz.dianchejie.cn/gtvyjvxpkc.html

[B01] 条件判断 if / else
来源：http://hz.yj20258888.top/gtgdvazhem.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.52xcode.cn/gtxfxghmol.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.xingfuxueyuan.xyz/gtqadbwwau.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.316326.xyz/gtctqktjon.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.wangshuangyany.cn/gtbjlrrgrl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.yj20258888.top/gtxltflhry.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.yongpay.top/gtseedwmyy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.fzhhl.top/gtegjrkrxv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.pycfn.com/gtmqnedqgk.html

[B02] 多分支 else if / elif
来源：http://hz.xylfe.cn/gtlkfrdyfp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.yanxiufei.cn/gteblahsyw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.gzhubu.top/gtokswztwi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shangyingyoupin.top/gtzwogecrh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.vqdsnc.cn/gtwwfnvrqk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhoulong.xyz/gtvsaakrxi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.yuxming.cn/gtkdaijnqy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.zycfv.cn/gtpfqmxvgv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.fengsongda.top/gtkwqpaocr.html

[B03] switch / match / case
来源：http://hz.yueranfly.top/gtdoaryuqz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.yongpay.top/gtweknsgmi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.xinyue.icu/gtsgoibnkm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.svipenyu.cn/gtizmwctjc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.ywan-chungtsiang.top/gtvjevyzlv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.mhx1999.top/gtqsfcnlml.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.guannengcc.top/gtmpfyjrbo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.ivvv.top/gtkwzhcrvl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.chenlongwang.top/gtnqedgvdg.html

[B04] for 计数循环
来源：http://hz.yvedp.cn/gtjqlzopeq.html

Py:   for i in range(10): print(i)
来源：http://hz.andypj.xyz/gtlqhprfuu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.cashguo.top/gtrfyzjrjd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.gotoacloud.top/gtsbdqdvfm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.shuidangran.top/gtptvrgugl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.chenjidiqi.icu/gthuofdfwk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.tanke756.top/gtoxcswqzv.html

Ruby: 10.times { |i| puts i }
来源：http://hz.quarkkingdee.top/gttpbqyrjd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.zhongyouzk.top/gtyddtrieh.html

[B05] 遍历数组 / 列表
来源：http://hz.yuxming.cn/gtdxxlekrq.html

Py:   for item in arr: print(item)
来源：http://hz.c1oappe.top/gtgqlsbuop.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.gogol.net.cn/gtofjlncew.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.shanyushiyangkeji.top/gtstuccxnw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.gogol.net.cn/gtclsbhsjd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.feifeiyinyue.top/gttltotubd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.zhiwuduotai.top/gtmephrfnu.html

Ruby: arr.each { |item| puts item }
来源：http://hz.jlsjyb.cn/gtutujundp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.zhaomingkeji.xyz/gtwypvgicq.html

[B06] 遍历字典 / 对象
来源：http://hz.hnqzz.top/gtjkxcryuj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.sweek.top/gtxrwgbypq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.pengpengdd.cyou/gtopfjkmkg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.nwbrower.top/gthlalyhkb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.gotoacloud.top/gttpbbtshr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.guowangkeji.top/gtkfqadgnf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.zhaomingkeji.xyz/gtwxritogt.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.jlsjyb.cn/gtgrkcpdkj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.havefunace.top/gtcdjedblh.html

[B07] while 循环
来源：http://hz.redwolf501.top/gtbanqqnpe.html

Py:   while i < 10: i += 1
来源：http://hz.nanxinkj.top/gtyrvygmnm.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.dashuyun.cn/gtsvulszpf.html

JS:   while (i < 10) { i++; }
来源：http://hz.hnxiangtu.top/gthgwjydpc.html

TS:   while (i < 10) { i++; }
来源：http://hz.yuxming.cn/gtzzmxfcak.html

Java: while (i < 10) { i++; }
来源：http://hz.sysykeji.top/gtjgeujlpv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.ydzc1.top/gtiraiauxx.html

Ruby: while i < 10; i += 1; end
来源：http://hz.hnqzz.top/gtxydbsgmk.html

C#:   while (i < 10) { i++; }
来源：http://hz.nanxinkj.top/gtfrkcwuxk.html

[B08] do-while（至少执行一次）
来源：http://hz.sxryk.cn/gtxhpcyrkr.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.snrcjt.cn/gtyytbudbk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.andypj.xyz/gtrsbgcsmt.html

JS:   do { i++; } while (i < 10);
来源：http://hz.cheryme.top/gtzkmjthjw.html

TS:   do { i++; } while (i < 10);
来源：http://hz.zhaomingkeji.xyz/gtbacdwtjo.html

Java: do { i++; } while (i < 10);
来源：http://hz.ybcxt.top/gtkyburlgh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.sysykeji.top/gtliscgprs.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.ppjwa.cn/gtpwxqiqgl.html

C#:   do { i++; } while (i < 10);
来源：http://hz.bjfxy.top/gtckszhtqi.html

[B09] break 与 continue
来源：http://hz.birdmap.top/gtsegtysok.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.shanyushiyangkeji.top/gtfayysfxj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.gaohongyu789.top/gtgsyahagk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.c1oappe.top/gtiqyuwhsi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.chenlongwang.top/gttlucyouw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.52xcode.cn/gtcmmrsxhe.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.zhoulong.xyz/gtrylxmhti.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.xingfuxueyuan.xyz/gtjgvmyvhm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gaohongyu789.top/gtjvmetxqr.html

[B10] 遍历同时拿索引
来源：http://hz.jinqigufen.top/gtmgbwufjx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.zhongyouzk.top/gtzwsrupmh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.hnqzz.top/gtocayzizj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.zhengqikj.top/gtvsanwaxw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.pengpengdd.cyou/gtrgtopzpc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.ywan-chungtsiang.top/gtydlurshr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yj20258.top/gtxddjgnvn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jqgufenzy.top/gtjjacitvp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.sysykeji.top/gtbdtmbcxt.html

[B11] 生成数字序列 / 区间
来源：http://hz.fzhhl.top/gtetvznulg.html

Py:   list(range(0, 10, 2))
来源：http://hz.tianlin.xyz/gtqooczsbk.html

PHP:  range(0, 10, 2);
来源：http://hz.tanke756.top/gtzjrwhwqs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.haohaochexian.top/gtzlsjzswo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ydzc1.top/gtbgreltnx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.316326.xyz/gtoohyetmi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.gzhubu.top/gtwzuxmecs.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yuxming.cn/gtxlozoiqv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.gaohongyu789.top/gttzgwganu.html

[B12] 跳出多层循环
来源：http://hz.yj20258.top/gtqghvojdt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.9152youxi.cn/gtbvkgljmn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jqgfzy.top/gtpxqdwcos.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yueranfly.top/gtvavvoigw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yongpay.top/gtdumbhxxb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.tanke756.top/gtegijnzqh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jlsjyb.cn/gtzaxywrmn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yuanzhike.top/gtsurtctgu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.gzhubu.top/gtgppvoldf.html

[B13] 判断是否为数字
来源：http://hz.hfpthk.cn/gtuvjcykyi.html

Py:   isinstance(x, (int, float))
来源：http://hz.ydzc1.top/gtlectyiav.html

PHP:  is_numeric($x)
来源：http://hz.sweek.top/gtvnmqaqqk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.gzhubu.top/gtbqnnypub.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jinqigufen.top/gtabsfxhkt.html

Java: x instanceof Number
来源：http://hz.yuanzhike.top/gtamaigodm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jinqigufen.top/gtaxwbkaip.html

Ruby: x.is_a?(Numeric)
来源：http://hz.feifeiyinyue.top/gtunxiiejh.html

C#:   x is int or double or decimal
来源：http://hz.hnqzz.top/gtauxyncus.html

[B14] 判断值是否在集合内
来源：http://hz.zhongyouzk.top/gtogybfwwi.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yangfankeji.com/gtbltsprxn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.sxryk.cn/gtenflpkjy.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yueranfly.top/gtvbqamewb.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jyoumei.cn/gttrhztuhj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zhixingplan.top/gtktxwndxs.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.andypj.xyz/gtzcveynnb.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.shanyushiyangtech.top/gtwadqpmwo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jinqigufen.top/gtzrctdkig.html

[B15] 布尔运算与取反
来源：http://hz.jqgfzy.top/gtpfoapefn.html

Py:   a and b or not c
来源：http://hz.nanxuanxn.top/gtpmwqnkwn.html

PHP:  $a && $b || !$c
来源：http://hz.hnqzz.top/gtsugzbmuc.html

JS:   a && b || !c
来源：http://hz.shangyingyoupin.top/gtddxwzivj.html

TS:   a && b || !c
来源：http://hz.aibaodan.cn/gtrubjneqz.html

Java: a && b || !c
来源：http://hz.xingfuxueyuan.xyz/gtcbqyfrbh.html

Go:   a && b || !c
来源：http://hz.jqgufenzy.top/gthzzlitmw.html

Ruby: a && b || !c
来源：http://hz.ehwqpu.com/gtrrwkhvue.html

C#:   a && b || !c
来源：http://hz.yj20258888.top/gtgjilxsjr.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.smart0.xyz/gtjfwmegoj.html

Py:   if not data: return
来源：http://hz.kuanghao11.cn/gtbslsmhjb.html

PHP:  if (!$data) { return; }
来源：http://hz.sweek.top/gtpwnrlvwl.html

JS:   if (!data) return;
来源：http://hz.jlsjyb.cn/gttqnlifvt.html

TS:   if (!data) return;
来源：http://hz.ehwqpu.com/gtpioristz.html

Java: if (data == null) return;
来源：http://hz.nanxinkj.top/gtalkdmmem.html

Go:   if data == nil { return }
来源：http://hz.zhaomingkeji.xyz/gtlltqrxqp.html

Ruby: return if data.nil?
来源：http://hz.svipenyu.cn/gtrvlwsaur.html

C#:   if (data == null) return;
来源：http://hz.yanxiufei.cn/gtscmswevx.html

================================================================================
来源：http://hz.nwbrower.top/gteggqwksb.html

C. 函数与作用域
来源：http://hz.cashguo.top/gtjadlpirx.html

================================================================================
来源：http://hz.yj20258.top/gtkkkmitic.html

[C01] 定义函数
来源：http://hz.sxryk.cn/gtpdrglvqo.html

Py:   def add(a, b): return a + b
来源：http://hz.jinqigufen.top/gtbbvsdxfa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tanke756.top/gtkmmgutmc.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.pycfn.com/gtqmyxempp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zdqjudy.top/gtoiqyxhzf.html


<!-- 参考信息 -->