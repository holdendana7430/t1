代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://hz.shanyushiyangkeji.top/gtngadxyye.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.dianchejie.cn/gtynouqrfr.html

Go:   // 单行；/* 多行 */
来源：http://hz.ydzc1.top/gtedfxuiuy.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.ppjwa.cn/gtxiijoodu.html

C#:   // 单行；/* 多行 */
来源：http://hz.shanyushiyangkeji.top/gtdmiuijyi.html

[A15] 空值判断与默认值
来源：http://hz.gaohongyu789.top/gtvgcnrbrx.html

Py:   value = data or "默认值"
来源：http://hz.jinqigfzy.top/gtkkcxobgp.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.hnqzz.top/gtqdkjzstc.html

JS:   const value = data ?? "默认值";
来源：http://hz.hnqzz.top/gtyacqsbav.html

TS:   const value = data ?? "默认值";
来源：http://hz.vqdsnc.cn/gtypwoaduk.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.jianghu66.top/gtvncrbvvt.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.hysaishi.cn/gtrjcopvtn.html

Ruby: value = data || "默认值"
来源：http://hz.jqgfzy.top/gtbvreqaqs.html

C#:   var value = data ?? "默认值";
来源：http://hz.kuanghao11.cn/gttjszhzpd.html

[A16] 真假值判断规则
来源：http://hz.shuidangran.top/gtlivicceh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.aizwys.cn/gtfmpvrodj.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.hywenlv.cn/gtunoeneoh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.nanxuanxn.top/gtobslszpw.html

TS:   if (!x) {}
来源：http://hz.hammf.cn/gttzmgrnux.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.sxryk.cn/gthtksiflk.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.zhixingplan.top/gtsrymgafg.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.jqgufenzy.top/gtwgxndalp.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.quarkkingdee.top/gtxcayewhs.html

[A17] 位运算
来源：http://hz.sysykeji.top/gtqxvqxmcb.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.redwolf501.top/gteyqguekf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.xziqi.cn/gtolkkuovv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yonumen.top/gtxiunquvh.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.ywan-chungtsiang.top/gtgdtqzlpf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.shangyingyoupin.top/gtbccdkgkc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.zhijiandao.cn/gtqjrpnjri.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.dashuyun.cn/gtfskvpfmf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yongpay.top/gtfyazlybf.html

[A18] 字符与 ASCII 码互转
来源：http://hz.dianchejie.cn/gtebqrocah.html

Py:   ord("A"); chr(65)
来源：http://hz.sweek.top/gtaajnskvy.html

PHP:  ord("A"); chr(65)
来源：http://hz.yvedp.cn/gthopegrto.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.gaohongyu789.top/gtuwgiddkq.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.ywan-chungtsiang.top/gtotrjuuhv.html

Java: (int) 'A'; (char) 65
来源：http://hz.yongpay.top/gthcbcwtrc.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.hnxiangtu.top/gtklpliskr.html

Ruby: "A".ord; 65.chr
来源：http://hz.ydjk.org.cn/gthqbbpkjl.html

C#:   (int)'A'; (char)65
来源：http://hz.sxryk.cn/gtzvttqqbf.html

[A19] 交换两个变量
来源：http://hz.bjfxy.top/gtwphelitp.html

Py:   a, b = b, a
来源：http://hz.zhixingplan.top/gtuoejmtid.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.haohaochexian.top/gtgifttjzj.html

JS:   [a, b] = [b, a];
来源：http://hz.zhoulong.xyz/gtuwnfkgqj.html

TS:   [a, b] = [b, a];
来源：http://hz.jiagoushi.top/gtvlgzvlcr.html

Java: int t = a; a = b; b = t;
来源：http://hz.yanxiufei.cn/gtkbftscgm.html

Go:   a, b = b, a
来源：http://hz.wangshuangyany.cn/gtcvcbqlgh.html

Ruby: a, b = b, a
来源：http://hz.ydzc1.top/gtxhacaxrx.html

C#:   (a, b) = (b, a);
来源：http://hz.zhengqikj.top/gtunvpivzc.html

[A20] 读取标准输入
来源：http://hz.jianghu66.top/gtlspzzhwy.html

Py:   name = input("请输入：")
来源：http://hz.zycfv.cn/gtxttcqrmn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.shanyushiyangtech.top/gtqbjszgos.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.vqdsnc.cn/gtfachpiue.html

TS:   // Node.js：readline 模块
来源：http://hz.zdqjudy.top/gtyyxxwfjj.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.zhijiandao.cn/gtoekhnhxw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.jinqigfzy.top/gtpkjbszha.html

Ruby: gets.chomp
来源：http://hz.redwolf501.top/gtjautubka.html

C#:   Console.ReadLine();
来源：http://hz.cheryme.top/gtzhdzpdpd.html

[A21] 保留指定小数位输出
来源：http://hz.andypj.xyz/gtuqbjojna.html

Py:   f"{3.14159:.2f}"
来源：http://hz.yj20258.top/gtjffoditt.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.zdqjudy.top/gtkdnkaokr.html

JS:   (3.14159).toFixed(2)
来源：http://hz.shanyushiyangkeji.top/gternbfztm.html

TS:   (3.14159).toFixed(2)
来源：http://hz.nwbrower.top/gtokgvxnlv.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.ybcxt.top/gtojaqlvlf.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.cashguo.top/gtkkjzplkb.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.andypj.xyz/gtrlpfelfo.html

C#:   3.14159.ToString("F2")
来源：http://hz.sweek.top/gtjifoolkv.html

[A22] 获取字符串长度
来源：http://hz.shanyushiyangkeji.top/gttrgksspz.html

Py:   len(s)
来源：http://hz.jinqigfzy.top/gtjmahinvh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.xziqi.cn/gtnxrqzxqx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.yuxming.cn/gtdcdmyhnb.html

TS:   s.length
来源：http://hz.smart0.xyz/gtksovhfhp.html

Java: s.length()
来源：http://hz.gogol.net.cn/gtbvjpdceb.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.jyoumei.cn/gtkocwuynn.html

Ruby: s.length
来源：http://hz.pycfn.com/gteddjtrgh.html

C#:   s.Length
来源：http://hz.daxiang520.top/gtzzeqyang.html

[A23] 大小写转换
来源：http://hz.jiagoushi.top/gtlwekgcgi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.tanke756.top/gtkrvlbtvy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.xuetiantiany.cn/gtlqadxcdd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.jinyuanbaomall.cn/gtwzaocwdv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.xziqi.cn/gtyojcykjq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.snrcjt.cn/gtmeksgmvz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.yonumen.top/gtpuvayawl.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.cashguo.top/gtbqewqiid.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.52xcode.cn/gtkkjtuphk.html

[A24] 去除首尾空白
来源：http://hz.pycfn.com/gtnrjkzplx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.iojbl.cn/gtonpsdenk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.xinyue.icu/gtjtjapipv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zhoulong.xyz/gtpyseoswk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.chenjidiqi.icu/gtffzduysq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.daria6918.cn/gtornckcpx.html

Go:   strings.TrimSpace(s)
来源：http://hz.guannengcc.top/gtikrqprag.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.hnqzz.top/gttmnnqpzq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.ybcxt.top/gtuyhcjntx.html

[A25] 字符串比较
来源：http://hz.sufxvd.cn/gtrbcnqkgr.html

Py:   s1 == s2; s1 != s2
来源：http://hz.gotoacloud.top/gtjcfezbdt.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.jlsjyb.cn/gtuiawfhxj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yj202588.top/gtmxewyrlf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.sufxvd.cn/gtquczmzdl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.yongpay.top/gtchiwrbqg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.guowangkeji.top/gteltekcez.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.yj20258888.top/gtlpigblkg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.zhoulong.xyz/gtscvyhgvc.html

[A26] 类型转换总览
来源：http://hz.pengpengdd.cyou/gttblkcfpa.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.shuidangran.top/gtcxyehjft.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.jinghuilouyu.cn/gttfiycxmn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.cheryme.top/gtonmvbytk.html

TS:   Number() String() Boolean() x as number
来源：http://hz.havefunace.top/gttfhflerd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.xziqi.cn/gtqdsfeduq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.redwolf501.top/gtnxbmgoth.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.hnqzz.top/gtydhladij.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.jlsjyb.cn/gtfulshypd.html

================================================================================
来源：http://hz.yj20258888.top/gtllubtmke.html

B. 流程控制
来源：http://hz.tian-w.cn/gtzlynbmyx.html

================================================================================
来源：http://hz.52xcode.cn/gtwwmxophb.html

[B01] 条件判断 if / else
来源：http://hz.vqdsnc.cn/gttbvrjcgx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.zhiwuduotai.top/gtljofyfwn.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.ppjwa.cn/gtokdingzf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.daria6918.cn/gtemxzajwz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.jyoumei.cn/gtncpjvfwh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.ywan-chungtsiang.top/gtuvbogffq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.zhongyouzk.top/gtiwbshgsg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.jqgfzy.top/gtyrrdhmuk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.xylfe.cn/gtcuudhwsf.html

[B02] 多分支 else if / elif
来源：http://hz.nanxuanxn.top/gtsgrzpzzd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.jlsjyb.cn/gtcgziwexm.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.c1oappe.top/gtwymnpafu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cqqwz.cn/gtezailqlq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.sysykeji.top/gtcrbwvjaj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ehwqpu.com/gtsjbmeext.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.quarkkingdee.top/gtrapigeul.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.havefunace.top/gtlzspjlvz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.sweek.top/gtmmqxneyo.html

[B03] switch / match / case
来源：http://hz.ybcxt.top/gttbjzjgfw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.yuanzhike.top/gtfprjrdho.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.yangfankeji.com/gtfvfrsjha.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.sufxvd.cn/gtfofdukza.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jinghuilouyu.cn/gtafwokdyd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.yj202588.top/gtkhmfjkxe.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.shanyushiyangkeji.top/gttnruvjck.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.shzxlz.cn/gtvdksqiiq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.jianghu66.top/gtddhlmvnu.html

[B04] for 计数循环
来源：http://hz.fzhhl.top/gtbxvrmpym.html

Py:   for i in range(10): print(i)
来源：http://hz.dianchejie.cn/gtknfcctvt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.mhx1999.top/gtmzxfneea.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.hnxiangtu.top/gtllpveyhj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.vqdsnc.cn/gtrmbowzlm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.hfpthk.cn/gtiyfiztwg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.fengsongda.top/gtzpkpmphl.html

Ruby: 10.times { |i| puts i }
来源：http://hz.iojbl.cn/gtgzvfstzz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.jiagoushi.top/gtevxpsyjm.html

[B05] 遍历数组 / 列表
来源：http://hz.ydzc1.top/gtdbqihqao.html

Py:   for item in arr: print(item)
来源：http://hz.shanyushiyangtech.top/gtorhoywds.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.shangyingyoupin.top/gtsdkcqvxx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhongyouzk.top/gtelhsefpx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.xuetiantiany.cn/gtziqqfbox.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.vqdsnc.cn/gtjaykhdlm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.iojbl.cn/gtyvxwdzbp.html

Ruby: arr.each { |item| puts item }
来源：http://hz.snrcjt.cn/gtxdjneubq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.aizwys.cn/gtbckjjyxb.html

[B06] 遍历字典 / 对象
来源：http://hz.zycfv.cn/gttgzxmfig.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.jlsjyb.cn/gtynguqabf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.shanyushiyangtech.top/gtfxykxaof.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.aibaodan.cn/gtvuqclyss.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xinyue.icu/gtclwzotju.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.zhixingplan.top/gtsmmnkcti.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.sxryk.cn/gtkqsnjqnv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.xylfe.cn/gtajknnhhq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.iojbl.cn/gtbjssyafs.html

[B07] while 循环
来源：http://hz.ydzc1.top/gtcfoxahti.html

Py:   while i < 10: i += 1
来源：http://hz.zhijiandao.cn/gtdmdsqpjk.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.andypj.xyz/gtskbpozuu.html

JS:   while (i < 10) { i++; }
来源：http://hz.sxryk.cn/gttafaykde.html

TS:   while (i < 10) { i++; }
来源：http://hz.nwbrower.top/gtszfolccy.html

Java: while (i < 10) { i++; }
来源：http://hz.yj20258888.top/gtkoxyehor.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.hfpthk.cn/gtubxhwqap.html

Ruby: while i < 10; i += 1; end
来源：http://hz.xinyue.icu/gtklzeshmt.html

C#:   while (i < 10) { i++; }
来源：http://hz.ivvv.top/gtpzzxxklb.html

[B08] do-while（至少执行一次）
来源：http://hz.nwbrower.top/gtjxhxfxiy.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.zhaomingkeji.xyz/gtpdmxdbqw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.gotoacloud.top/gtvfmfsxfy.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yueranfly.top/gtzplphhys.html

TS:   do { i++; } while (i < 10);
来源：http://hz.daria6918.cn/gtqwztpghe.html

Java: do { i++; } while (i < 10);
来源：http://hz.jinqigufen.top/gtpfchdnqi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.hysaishi.cn/gtekobuhmb.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.cqqwz.cn/gtcdxdksus.html

C#:   do { i++; } while (i < 10);
来源：http://hz.nanxinkj.top/gtxplhrnwe.html

[B09] break 与 continue
来源：http://hz.fengsongda.top/gtaqdclcke.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.zdqjudy.top/gtfcfjphmu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.gotoacloud.top/gtkfpcybaz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jyoumei.cn/gtpnemdavs.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.wangshuangyany.cn/gtrcqcgqcr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.bjfxy.top/gtawbzajmi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.vqdsnc.cn/gtuunamulg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.feifeiyinyue.top/gtcpzpyefa.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hysaishi.cn/gtvzkkfyvb.html

[B10] 遍历同时拿索引
来源：http://hz.nwbrower.top/gtzkgodkko.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.yonumen.top/gtiplpxaep.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yangfankeji.com/gtmedqcmhs.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.hnqzz.top/gtwcerhnsm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.shangyingyoupin.top/gtfwnzcnjg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.xziqi.cn/gtzsukhhit.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yonumen.top/gtpewwddse.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.nanxinkj.top/gtxzrkwmqg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.zhijiandao.cn/gtdascsxrb.html

[B11] 生成数字序列 / 区间
来源：http://hz.guowangkeji.top/gtdleeiyha.html

Py:   list(range(0, 10, 2))
来源：http://hz.haohaochexian.top/gtdaeydrzp.html

PHP:  range(0, 10, 2);
来源：http://hz.jqgufenzy.top/gtnmktfzbo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.vqdsnc.cn/gtemonacpm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhongyouzk.top/gtqhryidcy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.xylfe.cn/gttjagvrju.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zhoulong.xyz/gtwulqgqjq.html

Ruby: (0...10).step(2).to_a
来源：http://hz.cashguo.top/gtnhcgulnx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.cashguo.top/gtkbwxdplo.html

[B12] 跳出多层循环
来源：http://hz.nanxinkj.top/gtxluojxvw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.sysykeji.top/gtkepwjsvi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.sysykeji.top/gtpujhbojt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cdnleiting.top/gtuzlvsuwk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.daria6918.cn/gtsmuivqaz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.meibo888.top/gtbgpvmnmq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yueranfly.top/gtofcpcaxp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yanxiufei.cn/gtdrulvuff.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.ppjwa.cn/gtizkepjpv.html

[B13] 判断是否为数字
来源：http://hz.ivvv.top/gtjzyvtqgr.html

Py:   isinstance(x, (int, float))
来源：http://hz.shzxlz.cn/gtresfgqrk.html

PHP:  is_numeric($x)
来源：http://hz.ppjwa.cn/gtyoommyep.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yj202588.top/gthqpvgcwg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhongyouzk.top/gtynvuzwrp.html

Java: x instanceof Number
来源：http://hz.yueranfly.top/gtgvlqbaak.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.gaohongyu789.top/gtsczyxgiv.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jlsjyb.cn/gtfmhcpvhg.html

C#:   x is int or double or decimal
来源：http://hz.jinqigufen.top/gthtopargg.html

[B14] 判断值是否在集合内
来源：http://hz.jinqigufen.top/gtbnannupn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.meibo888.top/gtpsiujvov.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.redwolf501.top/gtvjohdwnf.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.c1oappe.top/gthdcnaert.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.guannengcc.top/gtkccowces.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yuanzhike.top/gthucofjly.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.shuidangran.top/gttdfhljxb.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.hnqzz.top/gtrsakfpba.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.wangdashe.top/gttydrvprg.html

[B15] 布尔运算与取反
来源：http://hz.gaohongyu789.top/gtcbwrttne.html

Py:   a and b or not c
来源：http://hz.vqdsnc.cn/gtovedglcs.html

PHP:  $a && $b || !$c
来源：http://hz.ppjwa.cn/gtsvvlsfoy.html

JS:   a && b || !c
来源：http://hz.kuanghao11.cn/gtswuxdvzl.html

TS:   a && b || !c
来源：http://hz.pengpengdd.cyou/gtbgrtopbv.html

Java: a && b || !c
来源：http://hz.svipenyu.cn/gtwrebbzcu.html

Go:   a && b || !c
来源：http://hz.chenlongwang.top/gtqzujhqcm.html

Ruby: a && b || !c
来源：http://hz.zhiwuduotai.top/gtnouvdlxm.html

C#:   a && b || !c
来源：http://hz.jianghu66.top/gtajckmzcp.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yanxiufei.cn/gttcthqqry.html

Py:   if not data: return
来源：http://hz.quarkkingdee.top/gthdqmlszl.html

PHP:  if (!$data) { return; }
来源：http://hz.dianchejie.cn/gtotqpreno.html

JS:   if (!data) return;
来源：http://hz.shanyushiyangtech.top/gtpsvklnmg.html

TS:   if (!data) return;
来源：http://hz.xuanzx.com/gthwfcbbzw.html

Java: if (data == null) return;
来源：http://hz.yangfankeji.com/gtujqxeyuz.html

Go:   if data == nil { return }
来源：http://hz.cucudq.cn/gttluqnwgu.html

Ruby: return if data.nil?
来源：http://hz.cqqwz.cn/gtxwpzscqw.html

C#:   if (data == null) return;
来源：http://hz.cqqwz.cn/gtglzcddjx.html

================================================================================
来源：http://hz.hnqzz.top/gtmjakkcrc.html

C. 函数与作用域
来源：http://hz.meibo888.top/gtcdhmgdww.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtzuaysceb.html

[C01] 定义函数
来源：http://hz.chenlongwang.top/gtddeeqind.html

Py:   def add(a, b): return a + b
来源：http://hz.quarkkingdee.top/gttsyoegke.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenjidiqi.icu/gtrmjajxvj.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.daria6918.cn/gtajegxuyv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gotoacloud.top/gtblqiocdd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.chenjidiqi.icu/gtqmqxqwkw.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.shuidangran.top/gtmcnrdwcx.html

Ruby: def add(a, b); a + b; end
来源：http://hz.cqqwz.cn/gtopdosmkp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.birdmap.top/gtxtbktcmw.html

[C02] 默认参数
来源：http://hz.jinqigfzy.top/gtrcjwveyv.html

Py:   def greet(name="World"): return name
来源：http://hz.52xcode.cn/gtvzjwxidz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.aizwys.cn/gthffelowd.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.shangyingyoupin.top/gthjorwona.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.cheryme.top/gtvlaihfwv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.hnxiangtu.top/gtajtqsljs.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.cdnleiting.top/gtdrzhxoda.html

Ruby: def greet(name = "World") = name
来源：http://hz.xuetiantiany.cn/gtptsvqbnw.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jlsjyb.cn/gttiqroisl.html

[C03] 可变参数
来源：http://hz.dianchejie.cn/gtmqkhmnch.html

Py:   def total(*args): return sum(args)
来源：http://hz.zdqjudy.top/gtimqxmeif.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yanxiufei.cn/gtdtedqqsc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sxryk.cn/gtcnpzsptx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.fengsongda.top/gtpphjphoq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ehwqpu.com/gterfxiiai.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.xziqi.cn/gtkerrhojd.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.mhx1999.top/gtttmvqskf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.fzhhl.top/gtbhwgsrdw.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ydjk.org.cn/gtbhwysxap.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.xinyue.icu/gthndknzyh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhoulong.xyz/gteklakcnm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jyoumei.cn/gtnwwofflb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.hongshengwenyu.top/gtrgmlktgq.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.pengpengdd.cyou/gthjemhlnq.html

Go:   // 无：用配置结构体参数
来源：http://hz.zhixingplan.top/gtxjrdpdxg.html

Ruby: f(a: 1, b: 2)
来源：http://hz.shuidangran.top/gtxawltprb.html

C#:   f(a: 1, b: 2)
来源：http://hz.haohaochexian.top/gtzvsckxaw.html

[C05] 返回多个值
来源：http://hz.cucudq.cn/gtaewbygdy.html


<!-- 参考信息 -->