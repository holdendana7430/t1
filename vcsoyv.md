代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://hz.feifeiyinyue.top/gtffnqminr.html

[A11] 条件表达式（三元）
来源：http://hz.zhiwuduotai.top/gtjavctcqh.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.xziqi.cn/gtvpogqaau.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.xuetiantiany.cn/gtqizemams.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.jqgufenzy.top/gtbmxdtfsc.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.shuidangran.top/gtxhcfmgnn.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.nwbrower.top/gtnyzcrnsk.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.meibo888.top/gtosvkfaxs.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.yj20258.top/gtoqtcupau.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.xuanzx.com/gtkbduozbc.html

[A12] 字符串插值 / 格式化
来源：http://hz.xingfuxueyuan.xyz/gtzxncbjgy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.nwbrower.top/gtwwphylcz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.pycfn.com/gtgsaknhwo.html

JS:   `Hello, ${name}!`
来源：http://hz.guannengcc.top/gtxdplnbqw.html

TS:   `Hello, ${name}!`
来源：http://hz.ivvv.top/gtsyiowpkk.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.yanxiufei.cn/gtvorywsky.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.xuanzx.com/gtyyqpryqd.html

Ruby: "Hello, #{name}!"
来源：http://hz.hfpthk.cn/gtfpbirquy.html

C#:   $"Hello, {name}!"
来源：http://hz.smart0.xyz/gtwiwulbsx.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.vqdsnc.cn/gtjirkrmuy.html

Py:   "第一行\n第二行"
来源：http://hz.hnxiangtu.top/gtnqonnpiq.html

PHP:  "第一行\n第二行"
来源：http://hz.xziqi.cn/gtanlhwmkt.html

JS:   "第一行\n第二行"
来源：http://hz.ywan-chungtsiang.top/gtqvuseuik.html

TS:   "第一行\n第二行"
来源：http://hz.redwolf501.top/gtgogkleqe.html

Java: "第一行\n第二行"
来源：http://hz.aizwys.cn/gthxcvfgre.html

Go:   "第一行\n第二行"
来源：http://hz.tianlin.xyz/gtijqbaosl.html

Ruby: "第一行\n第二行"
来源：http://hz.xinyue.icu/gtljvtqdxc.html

C#:   "第一行\n第二行"
来源：http://hz.hnqzz.top/gtrksvuikw.html

[A14] 注释写法
来源：http://hz.316326.xyz/gtsmwehutb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.fengsongda.top/gtaydiqkmc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.zhoulong.xyz/gtiiiknpvp.html

JS:   // 单行；/* 多行 */
来源：http://hz.c1oappe.top/gtplwxxwvz.html

TS:   // 单行；/* 多行 */
来源：http://hz.hammf.cn/gtqukntgrs.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.yangfankeji.com/gtejuymrem.html

Go:   // 单行；/* 多行 */
来源：http://hz.yj20258.top/gtldhsbauk.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.yangfankeji.com/gtxlnyfkul.html

C#:   // 单行；/* 多行 */
来源：http://hz.xylfe.cn/gtfzbjarcu.html

[A15] 空值判断与默认值
来源：http://hz.cqqwz.cn/gtnnrpieod.html

Py:   value = data or "默认值"
来源：http://hz.zhoulong.xyz/gtiapntddm.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.guannengcc.top/gtsccimhpk.html

JS:   const value = data ?? "默认值";
来源：http://hz.zhongyouzk.top/gtztvgnceu.html

TS:   const value = data ?? "默认值";
来源：http://hz.gogol.net.cn/gtzukumssj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.sufxvd.cn/gtlxpbigtw.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.meibo888.top/gtchcaqjzy.html

Ruby: value = data || "默认值"
来源：http://hz.zhixingplan.top/gtmbkfpegh.html

C#:   var value = data ?? "默认值";
来源：http://hz.zhixingplan.top/gtiymoqhlb.html

[A16] 真假值判断规则
来源：http://hz.jqgfzy.top/gtrtxeslpi.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.haohaochexian.top/gtimoaapzx.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.xuanzx.com/gtlaefgqdz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.c1oappe.top/gtqtjraqrr.html

TS:   if (!x) {}
来源：http://hz.nwbrower.top/gthqsvyrgl.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.zhijiandao.cn/gtxtmizkbk.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.ybcxt.top/gtgzgsnbtj.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.hongshengwenyu.top/gtyepkcsdi.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.hnxiangtu.top/gtqhnarrbe.html

[A17] 位运算
来源：http://hz.ehwqpu.com/gtrtiqotas.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yueranfly.top/gtfmdxsacf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.havefunace.top/gtgtstqkol.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.guowangkeji.top/gtqpaqvhux.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.bjfxy.top/gtwdnamzmj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jinghuilouyu.cn/gtreybayla.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.jlsjyb.cn/gtodqgwwkk.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.andypj.xyz/gtbibcgqdq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jinqigufen.top/gtxkozgpnr.html

[A18] 字符与 ASCII 码互转
来源：http://hz.zhixingplan.top/gtqbnuwjde.html

Py:   ord("A"); chr(65)
来源：http://hz.dianchejie.cn/gtontkqpsd.html

PHP:  ord("A"); chr(65)
来源：http://hz.chenzaomai.com/gtoifpzvqw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.chenzaomai.com/gtskpqmwsc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.yj202588.top/gtfydjquov.html

Java: (int) 'A'; (char) 65
来源：http://hz.yj20258.top/gtdvivjdst.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.sufxvd.cn/gtambvlhip.html

Ruby: "A".ord; 65.chr
来源：http://hz.andypj.xyz/gtwpjllhdb.html

C#:   (int)'A'; (char)65
来源：http://hz.yuanzhike.top/gticfjyiyj.html

[A19] 交换两个变量
来源：http://hz.iojbl.cn/gtggxvhtmy.html

Py:   a, b = b, a
来源：http://hz.zdqjudy.top/gtjrcpcfbc.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.ehwqpu.com/gtdkpnmbmd.html

JS:   [a, b] = [b, a];
来源：http://hz.jyoumei.cn/gtybwhlinr.html

TS:   [a, b] = [b, a];
来源：http://hz.hfpthk.cn/gtiygckccs.html

Java: int t = a; a = b; b = t;
来源：http://hz.ybcxt.top/gtpbvogggs.html

Go:   a, b = b, a
来源：http://hz.yj202588.top/gtzbrzzsyd.html

Ruby: a, b = b, a
来源：http://hz.quarkkingdee.top/gtxzbfitbk.html

C#:   (a, b) = (b, a);
来源：http://hz.feifeiyinyue.top/gthbvotuly.html

[A20] 读取标准输入
来源：http://hz.gaohongyu789.top/gtvusybzqk.html

Py:   name = input("请输入：")
来源：http://hz.zhixingplan.top/gtjyzwrvuf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.yj20258888.top/gtjhaaeeht.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.jiagoushi.top/gtrmdfkwap.html

TS:   // Node.js：readline 模块
来源：http://hz.shanyushiyangkeji.top/gtimaohzoi.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.tanke756.top/gtgwtwakle.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.yueranfly.top/gtxgaoulfb.html

Ruby: gets.chomp
来源：http://hz.svipenyu.cn/gtfropyypg.html

C#:   Console.ReadLine();
来源：http://hz.c1oappe.top/gtedsyfaas.html

[A21] 保留指定小数位输出
来源：http://hz.jqgfzy.top/gtwqujuzws.html

Py:   f"{3.14159:.2f}"
来源：http://hz.quarkkingdee.top/gtqskbrzzd.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.jinyuanbaomall.cn/gtoishrnko.html

JS:   (3.14159).toFixed(2)
来源：http://hz.shanyushiyangtech.top/gtsnswgsbw.html

TS:   (3.14159).toFixed(2)
来源：http://hz.jinqigfzy.top/gtccuxwsug.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.tianlin.xyz/gtxmfwakqv.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.cashguo.top/gtacafrpqp.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.aibaodan.cn/gtjpqmmhex.html

C#:   3.14159.ToString("F2")
来源：http://hz.gotoacloud.top/gtggevkqmv.html

[A22] 获取字符串长度
来源：http://hz.haohaochexian.top/gtuiesemqi.html

Py:   len(s)
来源：http://hz.yuxming.cn/gtxxorynif.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.xingfuxueyuan.xyz/gtcngvstuq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.quarkkingdee.top/gtxpzlnzqs.html

TS:   s.length
来源：http://hz.gotoacloud.top/gtbvetibpi.html

Java: s.length()
来源：http://hz.wangdashe.top/gttldfmuvi.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.hywenlv.cn/gtusgwowmm.html

Ruby: s.length
来源：http://hz.gotoacloud.top/gtnrdzojso.html

C#:   s.Length
来源：http://hz.yangfankeji.com/gteiledlbh.html

[A23] 大小写转换
来源：http://hz.fengsongda.top/gtcfcovqpy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.daria6918.cn/gtobpcyzbm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.bjfxy.top/gtlgmjxoso.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.xylfe.cn/gtupctpbvm.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.yanxiufei.cn/gtynzxdlhc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.cdnleiting.top/gtfzkuyisp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.yj20258.top/gtekxrgnow.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.zhijiandao.cn/gttkhmlarh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.sweek.top/gtmxlbegtb.html

[A24] 去除首尾空白
来源：http://hz.hysaishi.cn/gtouxbeuhs.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.wangshuangyany.cn/gtfabwtccb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.gogol.net.cn/gtpmtwuvfz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.52xcode.cn/gtzmfquvcn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.sweek.top/gtirxfemel.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.yuxming.cn/gtsyfmrcat.html

Go:   strings.TrimSpace(s)
来源：http://hz.xylfe.cn/gtbetywtxo.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.tanke756.top/gtsfmderul.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.smart0.xyz/gtggvqmcbx.html

[A25] 字符串比较
来源：http://hz.9152youxi.cn/gtruxyrngu.html

Py:   s1 == s2; s1 != s2
来源：http://hz.kuanghao11.cn/gtyedibxwt.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.yuanzhike.top/gteqjdyich.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yonumen.top/gtdiyomlbv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.aizwys.cn/gthyhtvymn.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.0kj1m.cn/gtiqxfvdoj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.jianghu66.top/gtucmqodzf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.nanxinkj.top/gtetzzusym.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.cheryme.top/gtxyxkeelf.html

[A26] 类型转换总览
来源：http://hz.jiagoushi.top/gtsuwmbyaj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.jlsjyb.cn/gtjfyqqbuj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.ehwqpu.com/gteatsqmia.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.andypj.xyz/gtifmqrygx.html

TS:   Number() String() Boolean() x as number
来源：http://hz.ivvv.top/gtvngbjjlv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.zhongyouzk.top/gtjzbihjop.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.xuetiantiany.cn/gtfqlafvjr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.yueranfly.top/gtsgqrepcv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.shanyushiyangtech.top/gtaiwkmhwp.html

================================================================================
来源：http://hz.xuanzx.com/gtzillamdq.html

B. 流程控制
来源：http://hz.meibo888.top/gtzixtbolp.html

================================================================================
来源：http://hz.jinqigfzy.top/gtugixcnrh.html

[B01] 条件判断 if / else
来源：http://hz.gogol.net.cn/gtnenalbin.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.pycfn.com/gtfpaedcwk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.yueranfly.top/gtqjweyxzc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.jinqigufen.top/gtlsuopcsp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.daria6918.cn/gtvjbeadvz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.pengpengdd.cyou/gtyjowurqa.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.jinyuanbaomall.cn/gtmqkvkzvb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.iojbl.cn/gtlooabodx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.ehwqpu.com/gtbcfhrxgj.html

[B02] 多分支 else if / elif
来源：http://hz.xylfe.cn/gtzakqcuxz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.zhengqikj.top/gtwmbmnlpe.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.tianlin.xyz/gtvaboxryw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jqgfzy.top/gtzwquyoxd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.quarkkingdee.top/gtemixcyma.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ydjk.org.cn/gtwdnaexfg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.nanxinkj.top/gtpncprzmb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.hnxiangtu.top/gtkxbxoghd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhaomingkeji.xyz/gtprptwiiv.html

[B03] switch / match / case
来源：http://hz.redwolf501.top/gtbsdefaeo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.316326.xyz/gthznadovk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.hnqzz.top/gtojxbbqca.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.daxiang520.top/gtjqbtrjav.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.cheryme.top/gtrmocldcr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.mhx1999.top/gtzsezsrqs.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.zhengqikj.top/gtwlpixafq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.chenjidiqi.icu/gtftgwjgcw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.nanxuanxn.top/gtoyhlaxcs.html

[B04] for 计数循环
来源：http://hz.ydzc1.top/gtxycwxkpb.html

Py:   for i in range(10): print(i)
来源：http://hz.mhx1999.top/gtptjuepvd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.nwbrower.top/gtlgpqjzjy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.zhixingplan.top/gthcwxjwgt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yuanzhike.top/gtkvcrxzmq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.yangfankeji.com/gtzgijxijj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.mhx1999.top/gtnbzuydbz.html

Ruby: 10.times { |i| puts i }
来源：http://hz.sysykeji.top/gtjukbocjd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.feifeiyinyue.top/gtjovxbdex.html

[B05] 遍历数组 / 列表
来源：http://hz.jqgfzy.top/gtffwprgux.html

Py:   for item in arr: print(item)
来源：http://hz.hysaishi.cn/gtyfqtvquk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.9152youxi.cn/gtlwzhfobk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.yangfankeji.com/gtknvickih.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.yuanzhike.top/gtmmjbrriy.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.jinqigufen.top/gtteaysxqj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.xingfuxueyuan.xyz/gtfpnmdjog.html

Ruby: arr.each { |item| puts item }
来源：http://hz.chenlongwang.top/gtpstbdmnh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.andypj.xyz/gtnwbhshct.html

[B06] 遍历字典 / 对象
来源：http://hz.jyoumei.cn/gtspzaozvf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.redwolf501.top/gtfwxzhtph.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.zhixingplan.top/gtlvnsomtw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhixingplan.top/gtzwvdxnmr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zycfv.cn/gtcopiwuru.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.yanxiufei.cn/gtdatyesus.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.zhiwuduotai.top/gttcechrqx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.zhiwuduotai.top/gtkvuxxrqz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.xylfe.cn/gtfyucxeaz.html

[B07] while 循环
来源：http://hz.sufxvd.cn/gtlfsysuri.html

Py:   while i < 10: i += 1
来源：http://hz.zhiwuduotai.top/gtokdnxfnt.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.havefunace.top/gtnpjcpqjt.html

JS:   while (i < 10) { i++; }
来源：http://hz.cheryme.top/gtreyumazq.html

TS:   while (i < 10) { i++; }
来源：http://hz.cashguo.top/gtnwbwjjeo.html

Java: while (i < 10) { i++; }
来源：http://hz.kuanghao11.cn/gtfgewblun.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.hongshengwenyu.top/gtyljapcwn.html

Ruby: while i < 10; i += 1; end
来源：http://hz.hammf.cn/gtnhukvhia.html

C#:   while (i < 10) { i++; }
来源：http://hz.ydjk.org.cn/gtwxcidnka.html

[B08] do-while（至少执行一次）
来源：http://hz.yongpay.top/gtplqleutj.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.jinghuilouyu.cn/gtfmzrkylf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zhiwuduotai.top/gtyazetwjc.html

JS:   do { i++; } while (i < 10);
来源：http://hz.hfpthk.cn/gtkxxnkelg.html

TS:   do { i++; } while (i < 10);
来源：http://hz.gogol.net.cn/gtsravhkba.html

Java: do { i++; } while (i < 10);
来源：http://hz.yuanzhike.top/gtwxezuijx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.yonumen.top/gtramfqlji.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.9152youxi.cn/gtfgofqohs.html

C#:   do { i++; } while (i < 10);
来源：http://hz.tanke756.top/gtgyqgyxyg.html

[B09] break 与 continue
来源：http://hz.iojbl.cn/gtlvjxpgka.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.ydzc1.top/gtgxyoqolk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.xingfuxueyuan.xyz/gtsnuiinrt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ppjwa.cn/gtkoxgtwfx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shangyingyoupin.top/gtqhfdryet.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shanyushiyangtech.top/gtslezzidx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jinghuilouyu.cn/gttjdolnnc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jqgfzy.top/gtjamujvrn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.bjfxy.top/gtvmisjnde.html

[B10] 遍历同时拿索引
来源：http://hz.sysykeji.top/gtyexktuqt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.sweek.top/gttaekycfz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.smart0.xyz/gtoqtjpdxe.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.guannengcc.top/gtwitbmuce.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.vqdsnc.cn/gtnwinykuu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.zhiwuduotai.top/gtshovuyql.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.sweek.top/gtxxijbksu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.tian-w.cn/gtecuexmjg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.sysykeji.top/gtmyujfxmh.html

[B11] 生成数字序列 / 区间
来源：http://hz.mhx1999.top/gtpdrhllpj.html

Py:   list(range(0, 10, 2))
来源：http://hz.xinyue.icu/gtyaqbdmfr.html

PHP:  range(0, 10, 2);
来源：http://hz.jqgfzy.top/gtqrkscupb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jinqigfzy.top/gtwpkxxhxp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.chenzaomai.com/gtgmtjvskg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.yj202588.top/gtnefdcech.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.smart0.xyz/gtpmaijery.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yonumen.top/gtsnihxfxm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.tianlin.xyz/gtcopfkuni.html

[B12] 跳出多层循环
来源：http://hz.jinqigufen.top/gtzzlhvbll.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.ehwqpu.com/gtwxqddcxg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.hysaishi.cn/gtqkcjznqf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cheryme.top/gtjztmdura.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinqigufen.top/gtyombdcpk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.shuidangran.top/gtmdgbxvyh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jlsjyb.cn/gtxpjiaivv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.zhaomingkeji.xyz/gtkzusillm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yueranfly.top/gtajmentza.html

[B13] 判断是否为数字
来源：http://hz.snrcjt.cn/gtnpqwawde.html

Py:   isinstance(x, (int, float))
来源：http://hz.jinqigufen.top/gtjlyqkipi.html

PHP:  is_numeric($x)
来源：http://hz.sweek.top/gtbuhaihke.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sufxvd.cn/gtvuododtx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.quarkkingdee.top/gtxmatoaxq.html

Java: x instanceof Number
来源：http://hz.hysaishi.cn/gtxapimubu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zhongyouzk.top/gtcteslvuo.html

Ruby: x.is_a?(Numeric)
来源：http://hz.nwbrower.top/gtpklwqawb.html

C#:   x is int or double or decimal
来源：http://hz.ivvv.top/gtizkrntsg.html

[B14] 判断值是否在集合内
来源：http://hz.jinqigufen.top/gtmvitwlst.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.9152youxi.cn/gttdsabulq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jinghuilouyu.cn/gtejleaemg.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.hongshengwenyu.top/gtplfvkaak.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.sweek.top/gtfpjveqtw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.xziqi.cn/gtlberedwh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.pengpengdd.cyou/gtzmiyzuja.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yueranfly.top/gtqecwiges.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.c1oappe.top/gtbpuultvb.html

[B15] 布尔运算与取反
来源：http://hz.wangdashe.top/gttaoohwsm.html

Py:   a and b or not c
来源：http://hz.zdqjudy.top/gtlfpwnaxk.html

PHP:  $a && $b || !$c
来源：http://hz.hywenlv.cn/gtmloyuitk.html

JS:   a && b || !c
来源：http://hz.andypj.xyz/gtavaocjbg.html

TS:   a && b || !c
来源：http://hz.yj202588.top/gtqmudpcwx.html

Java: a && b || !c
来源：http://hz.xylfe.cn/gtuwyuosrr.html

Go:   a && b || !c
来源：http://hz.ydjk.org.cn/gtfihcazfc.html

Ruby: a && b || !c
来源：http://hz.bjfxy.top/gtipowrxnv.html

C#:   a && b || !c
来源：http://hz.ywan-chungtsiang.top/gtzgikiqgb.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.fzhhl.top/gthfnnteef.html

Py:   if not data: return
来源：http://hz.sufxvd.cn/gtpeqeomtk.html

PHP:  if (!$data) { return; }
来源：http://hz.chenzaomai.com/gtbpzenmhr.html

JS:   if (!data) return;
来源：http://hz.yangfankeji.com/gtakqkrdbb.html

TS:   if (!data) return;
来源：http://hz.zhiwuduotai.top/gtywdjxzaz.html

Java: if (data == null) return;
来源：http://hz.hongshengwenyu.top/gtfvlzfgbm.html

Go:   if data == nil { return }
来源：http://hz.gogol.net.cn/gthfrkwurg.html

Ruby: return if data.nil?
来源：http://hz.aizwys.cn/gtmippmvbj.html

C#:   if (data == null) return;
来源：http://hz.ydzc1.top/gtdgsninhm.html

================================================================================
来源：http://hz.birdmap.top/gtjkgijbej.html

C. 函数与作用域
来源：http://hz.yongpay.top/gtdplwnsxz.html

================================================================================
来源：http://hz.hywenlv.cn/gtnjqwuprn.html

[C01] 定义函数
来源：http://hz.yvedp.cn/gttrxtsdmh.html

Py:   def add(a, b): return a + b
来源：http://hz.tian-w.cn/gtnhegmpqr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tianlin.xyz/gtaxawktag.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.daria6918.cn/gtiarhpifr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xingfuxueyuan.xyz/gtaxwavous.html


<!-- 参考信息 -->