代发 wailian999

Java: "第一行\n第二行"
来源：http://hz.shzxlz.cn/gtiaipftcg.html

Go:   "第一行\n第二行"
来源：http://hz.yj202588.top/gtcnuybwaf.html

Ruby: "第一行\n第二行"
来源：http://hz.dianchejie.cn/gtcblxgpko.html

C#:   "第一行\n第二行"
来源：http://hz.hysaishi.cn/gteimjmufm.html

[A14] 注释写法
来源：http://hz.snrcjt.cn/gtmdqdrgfv.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.hnxiangtu.top/gtrxucmzdj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.dianchejie.cn/gtdfunwgeh.html

JS:   // 单行；/* 多行 */
来源：http://hz.yanxiufei.cn/gtnoqyckgk.html

TS:   // 单行；/* 多行 */
来源：http://hz.mhx1999.top/gtpliegetc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.zhixingplan.top/gtlyzpnzpk.html

Go:   // 单行；/* 多行 */
来源：http://hz.gaohongyu789.top/gttdfxjska.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.hnxiangtu.top/gtkbmknnzs.html

C#:   // 单行；/* 多行 */
来源：http://hz.dianchejie.cn/gtwfbnmghq.html

[A15] 空值判断与默认值
来源：http://hz.shangyingyoupin.top/gtptrkdash.html

Py:   value = data or "默认值"
来源：http://hz.shzxlz.cn/gtlugijkto.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.shzxlz.cn/gtgtefriae.html

JS:   const value = data ?? "默认值";
来源：http://hz.kuanghao11.cn/gtrbuxqxxh.html

TS:   const value = data ?? "默认值";
来源：http://hz.jlsjyb.cn/gtvssltaxp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.guowangkeji.top/gtcwgqpqvx.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.gotoacloud.top/gtfzmuujti.html

Ruby: value = data || "默认值"
来源：http://hz.xylfe.cn/gtksnxmpbb.html

C#:   var value = data ?? "默认值";
来源：http://hz.wangdashe.top/gtumjxapfb.html

[A16] 真假值判断规则
来源：http://hz.yj202588.top/gtawfywuyf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.aibaodan.cn/gtvvhxiwbp.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.sysykeji.top/gtfwytemcc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.jqgufenzy.top/gtuhswigok.html

TS:   if (!x) {}
来源：http://hz.xinyue.icu/gtjjoxfmgw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.9152youxi.cn/gtmcgtqrqc.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.guowangkeji.top/gtnpgyxuaa.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.kuanghao11.cn/gtibmcogxi.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.gaohongyu789.top/gtqrmyqkhw.html

[A17] 位运算
来源：http://hz.yuanzhike.top/gtlztzrklf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.chenzaomai.com/gtlyizdwvl.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.zdqjudy.top/gtiexujdts.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.sweek.top/gtbtyjviok.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.jyoumei.cn/gtnpfttaxz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.tianlin.xyz/gtvwlifzcu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.daxiang520.top/gtexfoasbj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jlsjyb.cn/gtgjvaymuv.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.quarkkingdee.top/gtjnkembbt.html

[A18] 字符与 ASCII 码互转
来源：http://hz.xylfe.cn/gtbmhqdpfr.html

Py:   ord("A"); chr(65)
来源：http://hz.shangyingyoupin.top/gtkkdomckd.html

PHP:  ord("A"); chr(65)
来源：http://hz.haohaochexian.top/gtufeysiie.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.pengpengdd.cyou/gtroegtxdz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.kuanghao11.cn/gtnriklwqs.html

Java: (int) 'A'; (char) 65
来源：http://hz.nwbrower.top/gtpnwdblup.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.feifeiyinyue.top/gtfwocvtvb.html

Ruby: "A".ord; 65.chr
来源：http://hz.cqqwz.cn/gtvcutnbsg.html

C#:   (int)'A'; (char)65
来源：http://hz.gogol.net.cn/gtgtxbodro.html

[A19] 交换两个变量
来源：http://hz.zhongyouzk.top/gtdhnghugr.html

Py:   a, b = b, a
来源：http://hz.gotoacloud.top/gtmoaasfzj.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.dianchejie.cn/gttrmvgxig.html

JS:   [a, b] = [b, a];
来源：http://hz.yueranfly.top/gtqzigjqpa.html

TS:   [a, b] = [b, a];
来源：http://hz.ydzc1.top/gtadcishqd.html

Java: int t = a; a = b; b = t;
来源：http://hz.fengsongda.top/gtfuneaigz.html

Go:   a, b = b, a
来源：http://hz.zhijiandao.cn/gtnefeocco.html

Ruby: a, b = b, a
来源：http://hz.yvedp.cn/gtdfkkbhha.html

C#:   (a, b) = (b, a);
来源：http://hz.0kj1m.cn/gtjlypsvqy.html

[A20] 读取标准输入
来源：http://hz.nwbrower.top/gtguzvullz.html

Py:   name = input("请输入：")
来源：http://hz.wangshuangyany.cn/gtndfcuxfe.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.jyoumei.cn/gtxlswxund.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.yuanzhike.top/gticagxtim.html

TS:   // Node.js：readline 模块
来源：http://hz.jqgufenzy.top/gtsfkylozx.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.sweek.top/gtktmobvye.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.yj20258888.top/gtfaciocid.html

Ruby: gets.chomp
来源：http://hz.yuxming.cn/gtazobcfps.html

C#:   Console.ReadLine();
来源：http://hz.aizwys.cn/gtcflftchz.html

[A21] 保留指定小数位输出
来源：http://hz.wangshuangyany.cn/gtwtdquaut.html

Py:   f"{3.14159:.2f}"
来源：http://hz.quarkkingdee.top/gtomjqbnpq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.cheryme.top/gtnjmfxycm.html

JS:   (3.14159).toFixed(2)
来源：http://hz.daria6918.cn/gtnluamfkz.html

TS:   (3.14159).toFixed(2)
来源：http://hz.xuetiantiany.cn/gteluyfgrz.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.jinyuanbaomall.cn/gtnsovxudi.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.wangdashe.top/gtccnjsofb.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.jinqigufen.top/gtptwtnawk.html

C#:   3.14159.ToString("F2")
来源：http://hz.jianghu66.top/gtdritzatt.html

[A22] 获取字符串长度
来源：http://hz.jyoumei.cn/gtxrrczbhk.html

Py:   len(s)
来源：http://hz.chenzaomai.com/gtxfshefrt.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.c1oappe.top/gtxdattyuv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.yueranfly.top/gtpdlnoxqk.html

TS:   s.length
来源：http://hz.svipenyu.cn/gtftsmhwof.html

Java: s.length()
来源：http://hz.yongpay.top/gtbnfxxeri.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.redwolf501.top/gtwskxlola.html

Ruby: s.length
来源：http://hz.guannengcc.top/gttnmonwur.html

C#:   s.Length
来源：http://hz.cheryme.top/gthpzsvufa.html

[A23] 大小写转换
来源：http://hz.jlsjyb.cn/gtdkhcbqba.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.zycfv.cn/gtopotogdm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.ydzc1.top/gtwkaxtxvk.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.tian-w.cn/gttxpnaybr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.52xcode.cn/gtsvaskvms.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.gogol.net.cn/gtgnklchoz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.jlsjyb.cn/gtwrclvqno.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.chenjidiqi.icu/gtysapwhsc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.xingfuxueyuan.xyz/gtxuujblzs.html

[A24] 去除首尾空白
来源：http://hz.yonumen.top/gtyqqbulrd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.kuanghao11.cn/gthsmazekc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.quarkkingdee.top/gttvhrdvie.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.tanke756.top/gtktzthlpg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.birdmap.top/gtlybxkimf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.zhixingplan.top/gtpgfqudya.html

Go:   strings.TrimSpace(s)
来源：http://hz.ppjwa.cn/gtowishikc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.jinqigufen.top/gtopcgbjcv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.yuanzhike.top/gtwemyaiot.html

[A25] 字符串比较
来源：http://hz.yangfankeji.com/gttizxpbgg.html

Py:   s1 == s2; s1 != s2
来源：http://hz.jinqigufen.top/gtugmazsrs.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.c1oappe.top/gtdostgvnh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.0kj1m.cn/gtqwdlwmhl.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.shanyushiyangkeji.top/gtvcgbxzkm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.yuanzhike.top/gttmmyhmfo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.ydjk.org.cn/gtjwzsqebb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.shanyushiyangkeji.top/gtdurqdkjf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.hnxiangtu.top/gtefddbjcc.html

[A26] 类型转换总览
来源：http://hz.tian-w.cn/gtbygaxdgj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.wangdashe.top/gtiapiumwr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.shangyingyoupin.top/gtnvidrdxu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.yj202588.top/gtmsurwdwt.html

TS:   Number() String() Boolean() x as number
来源：http://hz.yvedp.cn/gtimldpjgi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.316326.xyz/gtqkysvvfe.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.iojbl.cn/gtsfohmjmz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.mhx1999.top/gtkknujzaq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.zhixingplan.top/gtbgxnevoo.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtuyzbtnmh.html

B. 流程控制
来源：http://hz.xuetiantiany.cn/gtdyjxrdsw.html

================================================================================
来源：http://hz.daria6918.cn/gtjynekpdo.html

[B01] 条件判断 if / else
来源：http://hz.gaohongyu789.top/gtdzvzwmvx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.jinghuilouyu.cn/gtughoxvtd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.zhiwuduotai.top/gttjrhzjdc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.xuetiantiany.cn/gtnylejxjz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yuxming.cn/gtwzeoqchk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.zhengqikj.top/gtqjpbsdst.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.jqgufenzy.top/gtkryfjwpb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.hongshengwenyu.top/gttjihoufa.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.jinqigfzy.top/gtgpotdbsb.html

[B02] 多分支 else if / elif
来源：http://hz.iojbl.cn/gtfakiyodo.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.chenlongwang.top/gtlfsfthyw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.quarkkingdee.top/gtjpolufvx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhiwuduotai.top/gtwppsnpjf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.chenjidiqi.icu/gtejxrelcg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gaohongyu789.top/gtinyeeolp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.hfpthk.cn/gtqafxwtzb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.ydzc1.top/gtbafqnxfp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.dashuyun.cn/gtnpyjnuub.html

[B03] switch / match / case
来源：http://hz.wangdashe.top/gtrhelcvyo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.yj202588.top/gtkvdalpdw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.0kj1m.cn/gtyycihecy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.aizwys.cn/gtrumbwlic.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jqgufenzy.top/gtuxnqnzzz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.yj20258888.top/gtcbqiycdt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.jqgfzy.top/gtydyvdrrm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.chenlongwang.top/gtsbavgygt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.guannengcc.top/gtexosajvx.html

[B04] for 计数循环
来源：http://hz.ppjwa.cn/gtrqvxgjbg.html

Py:   for i in range(10): print(i)
来源：http://hz.guannengcc.top/gtmqmtccud.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.jianghu66.top/gtloagofoc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.redwolf501.top/gtontymazl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.sweek.top/gtfejciiew.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.zdqjudy.top/gtjqnskmnd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.sysykeji.top/gtrofsaykx.html

Ruby: 10.times { |i| puts i }
来源：http://hz.wangshuangyany.cn/gtzzatkxcp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.xinyue.icu/gtvwquakxw.html

[B05] 遍历数组 / 列表
来源：http://hz.sweek.top/gtyyvbmuom.html

Py:   for item in arr: print(item)
来源：http://hz.zhengqikj.top/gtniklszei.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.zhoulong.xyz/gtoxvoizim.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.yuxming.cn/gttdmsfxkb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.tianlin.xyz/gtndulnjtu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.cashguo.top/gtlgffcwub.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.zhoulong.xyz/gtfspaycax.html

Ruby: arr.each { |item| puts item }
来源：http://hz.vqdsnc.cn/gtmkxeowaq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.yanxiufei.cn/gtxgjnuzuu.html

[B06] 遍历字典 / 对象
来源：http://hz.ehwqpu.com/gtypbobbiy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.cqqwz.cn/gtmnwlbnnf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.jinyuanbaomall.cn/gtbjypuhkv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hnxiangtu.top/gtnejldkrq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yueranfly.top/gtmurhltwv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.yuxming.cn/gtnunpawiu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.xingfuxueyuan.xyz/gtqqfxweps.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.xinyue.icu/gtchgjpght.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.haohaochexian.top/gtfyoiwofb.html

[B07] while 循环
来源：http://hz.zhiwuduotai.top/gtceqpxnjr.html

Py:   while i < 10: i += 1
来源：http://hz.chenjidiqi.icu/gtgzhbnyge.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.ppjwa.cn/gtzghzoqhk.html

JS:   while (i < 10) { i++; }
来源：http://hz.shuidangran.top/gtduaqebxu.html

TS:   while (i < 10) { i++; }
来源：http://hz.shanyushiyangtech.top/gtmlgnohfh.html

Java: while (i < 10) { i++; }
来源：http://hz.hywenlv.cn/gteszysgfw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.andypj.xyz/gtxvceavvh.html

Ruby: while i < 10; i += 1; end
来源：http://hz.jiagoushi.top/gtlpeyhuzu.html

C#:   while (i < 10) { i++; }
来源：http://hz.0kj1m.cn/gtrlfqmfqw.html

[B08] do-while（至少执行一次）
来源：http://hz.nanxuanxn.top/gtxpoxjpyr.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.yongpay.top/gtnfjwxxjq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.chenjidiqi.icu/gtghrkzpba.html

JS:   do { i++; } while (i < 10);
来源：http://hz.nanxuanxn.top/gtqncgzahs.html

TS:   do { i++; } while (i < 10);
来源：http://hz.xinyue.icu/gtuxixybep.html

Java: do { i++; } while (i < 10);
来源：http://hz.shanyushiyangtech.top/gtuirbzlvz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.yueranfly.top/gtofaosycr.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.yanxiufei.cn/gtbwvanqmy.html

C#:   do { i++; } while (i < 10);
来源：http://hz.hnqzz.top/gtfkrxdhoz.html

[B09] break 与 continue
来源：http://hz.bjfxy.top/gthdogaddn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.tanke756.top/gtepgifaru.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.hammf.cn/gtncicfnui.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hnqzz.top/gthkozweze.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.havefunace.top/gtwxvaqgno.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gotoacloud.top/gttklkxyfl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jinqigfzy.top/gtxkzldhjm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.xuanzx.com/gtlsfzjuwf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ywan-chungtsiang.top/gtbbbrjkqp.html

[B10] 遍历同时拿索引
来源：http://hz.cashguo.top/gthwsmbgpc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.nanxuanxn.top/gtissxnssj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.hnxiangtu.top/gtryllnfcm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.xuetiantiany.cn/gtoidrqcpe.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.cheryme.top/gtxiucysyw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.zhixingplan.top/gtcqxlyjqk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.zhongyouzk.top/gtoniglytv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.sweek.top/gtrnxvuxgg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.xuanzx.com/gtaaxvitsd.html

[B11] 生成数字序列 / 区间
来源：http://hz.cheryme.top/gtvjogxfcf.html

Py:   list(range(0, 10, 2))
来源：http://hz.zhiwuduotai.top/gtobgjhbid.html

PHP:  range(0, 10, 2);
来源：http://hz.vqdsnc.cn/gtnmorgxyq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.cqqwz.cn/gtfzachbzo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jlsjyb.cn/gttjqarcbg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.fengsongda.top/gtyprbqtye.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.shzxlz.cn/gtjrynuvkk.html

Ruby: (0...10).step(2).to_a
来源：http://hz.tian-w.cn/gtsypmtvvo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.hysaishi.cn/gtpldtzfbd.html

[B12] 跳出多层循环
来源：http://hz.chenzaomai.com/gtgqzqzrxy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.bjfxy.top/gtzslpzhtd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.hysaishi.cn/gtfuwshgbk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.gotoacloud.top/gtzsrahnpg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.aizwys.cn/gtfkjuuoyq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.redwolf501.top/gtyiaudbui.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yvedp.cn/gtiblpsgki.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.wangshuangyany.cn/gtduhturrl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.xinyue.icu/gtvrxzijvg.html

[B13] 判断是否为数字
来源：http://hz.52xcode.cn/gtmnwdhzht.html

Py:   isinstance(x, (int, float))
来源：http://hz.xziqi.cn/gtcmlaleeh.html

PHP:  is_numeric($x)
来源：http://hz.jinqigfzy.top/gtpokyphoh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.redwolf501.top/gtvejcmlnt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.dashuyun.cn/gtnlrqtvkq.html

Java: x instanceof Number
来源：http://hz.zdqjudy.top/gtzfcchyya.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.nanxinkj.top/gtqikorukw.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jqgfzy.top/gtikwbdtmp.html

C#:   x is int or double or decimal
来源：http://hz.hysaishi.cn/gttgdsbqlg.html

[B14] 判断值是否在集合内
来源：http://hz.ydjk.org.cn/gtslcricef.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.shuidangran.top/gtcznucoac.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.feifeiyinyue.top/gtunwcyqvx.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.shanyushiyangtech.top/gtjssflgea.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.guannengcc.top/gtgrmcyjip.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.hywenlv.cn/gtwkilvvtg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yj202588.top/gtykofibpu.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yuanzhike.top/gtfghkopyg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.feifeiyinyue.top/gtwvojulkr.html

[B15] 布尔运算与取反
来源：http://hz.nanxuanxn.top/gtmtlrloom.html

Py:   a and b or not c
来源：http://hz.9152youxi.cn/gtvbmhszrw.html

PHP:  $a && $b || !$c
来源：http://hz.zdqjudy.top/gtxnrdnlpf.html

JS:   a && b || !c
来源：http://hz.ehwqpu.com/gtlfpwnnwi.html

TS:   a && b || !c
来源：http://hz.jinghuilouyu.cn/gtupdrgnrz.html

Java: a && b || !c
来源：http://hz.nanxuanxn.top/gtprrxhvzj.html

Go:   a && b || !c
来源：http://hz.gaohongyu789.top/gtjtjkqfig.html

Ruby: a && b || !c
来源：http://hz.snrcjt.cn/gtxnxrcitp.html

C#:   a && b || !c
来源：http://hz.yonumen.top/gtkaanggzu.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.kuanghao11.cn/gthrmadqje.html

Py:   if not data: return
来源：http://hz.dashuyun.cn/gteepeiwcg.html

PHP:  if (!$data) { return; }
来源：http://hz.jinqigufen.top/gthnfbgjyf.html

JS:   if (!data) return;
来源：http://hz.birdmap.top/gtwqwzvbjq.html

TS:   if (!data) return;
来源：http://hz.shanyushiyangkeji.top/gtuyavzail.html

Java: if (data == null) return;
来源：http://hz.gotoacloud.top/gtzzcnhopb.html

Go:   if data == nil { return }
来源：http://hz.sxryk.cn/gtcfnqoggc.html

Ruby: return if data.nil?
来源：http://hz.hfpthk.cn/gtlkcjnvur.html

C#:   if (data == null) return;
来源：http://hz.pycfn.com/gtwupuiirs.html

================================================================================
来源：http://hz.jlsjyb.cn/gtvnkunrrs.html

C. 函数与作用域
来源：http://hz.sufxvd.cn/gtggooygrw.html

================================================================================
来源：http://hz.fzhhl.top/gtkmpvyvbu.html

[C01] 定义函数
来源：http://hz.cdnleiting.top/gtpsptbgoc.html

Py:   def add(a, b): return a + b
来源：http://hz.yuanzhike.top/gtylwztlxo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj20258888.top/gtcutgmnbe.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zhengqikj.top/gtrbgacrwv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhijiandao.cn/gttvxorzhn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xziqi.cn/gtrokfbgab.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.xinyue.icu/gtllknrojk.html

Ruby: def add(a, b); a + b; end
来源：http://hz.nwbrower.top/gtlnmvupre.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.hammf.cn/gtsfykjnng.html

[C02] 默认参数
来源：http://hz.xinyue.icu/gtpcfkrgku.html

Py:   def greet(name="World"): return name
来源：http://hz.yj20258888.top/gtntoygxgq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.52xcode.cn/gtzmrmbwmg.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.sysykeji.top/gtopgfrfmr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.snrcjt.cn/gtfywdkpvl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yj202588.top/gtqorngios.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhijiandao.cn/gtjqytbqyv.html

Ruby: def greet(name = "World") = name
来源：http://hz.xuetiantiany.cn/gtqyygeppu.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.c1oappe.top/gtcuuyjrbh.html

[C03] 可变参数
来源：http://hz.yangfankeji.com/gtnxcpucxl.html

Py:   def total(*args): return sum(args)
来源：http://hz.zhengqikj.top/gtfmzcbxjo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.sysykeji.top/gthnndhrne.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.pengpengdd.cyou/gttdwxpbuf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hysaishi.cn/gtnhuehmaw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.haohaochexian.top/gtbfjcpdte.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ivvv.top/gtrwhcmham.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.guannengcc.top/gtaqzchvxj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.shuidangran.top/gtkbsjwpdx.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ydjk.org.cn/gtoulfqhnr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zdqjudy.top/gtzgbrbozv.html


<!-- 参考信息 -->