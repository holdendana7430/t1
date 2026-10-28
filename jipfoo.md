代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.svipenyu.cn/gtyaywoxnj.html

Ruby: "Hello, #{name}!"
来源：http://hz.chenzaomai.com/gtavpefbeg.html

C#:   $"Hello, {name}!"
来源：http://hz.zhijiandao.cn/gtvmmomqji.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.shuidangran.top/gtxaluzssm.html

Py:   "第一行\n第二行"
来源：http://hz.shanyushiyangtech.top/gtpyvzdzdn.html

PHP:  "第一行\n第二行"
来源：http://hz.feifeiyinyue.top/gtitvrlizf.html

JS:   "第一行\n第二行"
来源：http://hz.chenjidiqi.icu/gthftmoyhf.html

TS:   "第一行\n第二行"
来源：http://hz.jyoumei.cn/gtqwnnlhzd.html

Java: "第一行\n第二行"
来源：http://hz.jianghu66.top/gtrdhzdflu.html

Go:   "第一行\n第二行"
来源：http://hz.iojbl.cn/gtddozipug.html

Ruby: "第一行\n第二行"
来源：http://hz.nanxinkj.top/gtfiorhlnw.html

C#:   "第一行\n第二行"
来源：http://hz.xylfe.cn/gtidfdtxvb.html

[A14] 注释写法
来源：http://hz.gogol.net.cn/gtmovsfoaj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.cashguo.top/gtuxzqxbjy.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.cqqwz.cn/gtsttaalcl.html

JS:   // 单行；/* 多行 */
来源：http://hz.zhengqikj.top/gtlmtbtdfh.html

TS:   // 单行；/* 多行 */
来源：http://hz.shanyushiyangkeji.top/gtosjvgcai.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.shuidangran.top/gtdslzzyam.html

Go:   // 单行；/* 多行 */
来源：http://hz.andypj.xyz/gthiatvupg.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.andypj.xyz/gtufsxhkux.html

C#:   // 单行；/* 多行 */
来源：http://hz.ehwqpu.com/gtolyvwaqg.html

[A15] 空值判断与默认值
来源：http://hz.meibo888.top/gtfvfiltik.html

Py:   value = data or "默认值"
来源：http://hz.feifeiyinyue.top/gtzcymoovp.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.aibaodan.cn/gtczapuncy.html

JS:   const value = data ?? "默认值";
来源：http://hz.xziqi.cn/gtyjyvmyvp.html

TS:   const value = data ?? "默认值";
来源：http://hz.c1oappe.top/gtgcoqfsos.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.jianghu66.top/gtoquhtyzs.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.mhx1999.top/gtddihnxhc.html

Ruby: value = data || "默认值"
来源：http://hz.gaohongyu789.top/gtsniopear.html

C#:   var value = data ?? "默认值";
来源：http://hz.shzxlz.cn/gtoytkehdz.html

[A16] 真假值判断规则
来源：http://hz.aibaodan.cn/gtxxulbjlm.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.yj202588.top/gtmysowngi.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.jinyuanbaomall.cn/gtcbhqkpea.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.nanxinkj.top/gtaunnxtki.html

TS:   if (!x) {}
来源：http://hz.hfpthk.cn/gtczqhmwvv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.shanyushiyangkeji.top/gtriusybua.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.wangshuangyany.cn/gtmuctyztn.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.sweek.top/gtkuipigvy.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.ywan-chungtsiang.top/gtabwklhjx.html

[A17] 位运算
来源：http://hz.tian-w.cn/gtrrlkrpkj.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yj202588.top/gtruaamnqf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.jinyuanbaomall.cn/gtrhakbukx.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xingfuxueyuan.xyz/gtoyablhkd.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.nwbrower.top/gtxbrzbuoq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yonumen.top/gtyzlgxlwv.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.gzhubu.top/gtitorxgwn.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.shanyushiyangtech.top/gtpukbjusd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.gotoacloud.top/gtuwmcmacf.html

[A18] 字符与 ASCII 码互转
来源：http://hz.jqgfzy.top/gthrtjnmhu.html

Py:   ord("A"); chr(65)
来源：http://hz.sweek.top/gtiegdiyfz.html

PHP:  ord("A"); chr(65)
来源：http://hz.c1oappe.top/gtelcjroau.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.chenzaomai.com/gtvfozjqqy.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.hywenlv.cn/gtnpwakham.html

Java: (int) 'A'; (char) 65
来源：http://hz.feifeiyinyue.top/gtxzbqqtzo.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.sysykeji.top/gtpomdzupv.html

Ruby: "A".ord; 65.chr
来源：http://hz.jqgufenzy.top/gtwvkglhdh.html

C#:   (int)'A'; (char)65
来源：http://hz.yj20258.top/gtssbnzaql.html

[A19] 交换两个变量
来源：http://hz.52xcode.cn/gtyowsmnti.html

Py:   a, b = b, a
来源：http://hz.bjfxy.top/gtchhmiqyq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.shuidangran.top/gtruwsdzyy.html

JS:   [a, b] = [b, a];
来源：http://hz.meibo888.top/gtfdbeaqvh.html

TS:   [a, b] = [b, a];
来源：http://hz.hongshengwenyu.top/gtxryxvuud.html

Java: int t = a; a = b; b = t;
来源：http://hz.jlsjyb.cn/gtcgtwtknj.html

Go:   a, b = b, a
来源：http://hz.iojbl.cn/gtfjcxjrrt.html

Ruby: a, b = b, a
来源：http://hz.xziqi.cn/gtepbqrhzt.html

C#:   (a, b) = (b, a);
来源：http://hz.chenjidiqi.icu/gtjmtbjosw.html

[A20] 读取标准输入
来源：http://hz.yongpay.top/gtenuhqmwc.html

Py:   name = input("请输入：")
来源：http://hz.feifeiyinyue.top/gtcaaukgcz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.daria6918.cn/gtztvspbvj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.quarkkingdee.top/gtdemxijrt.html

TS:   // Node.js：readline 模块
来源：http://hz.shzxlz.cn/gtdksxdrjz.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.gaohongyu789.top/gtbfienpxn.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.daxiang520.top/gtmzdtweoq.html

Ruby: gets.chomp
来源：http://hz.sysykeji.top/gtuchlaoqe.html

C#:   Console.ReadLine();
来源：http://hz.yj20258.top/gtgufewpxj.html

[A21] 保留指定小数位输出
来源：http://hz.daria6918.cn/gtzvwvmsnf.html

Py:   f"{3.14159:.2f}"
来源：http://hz.shanyushiyangkeji.top/gtlugvbdqo.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.bjfxy.top/gtrmdndnsq.html

JS:   (3.14159).toFixed(2)
来源：http://hz.jyoumei.cn/gtpbwevrun.html

TS:   (3.14159).toFixed(2)
来源：http://hz.iojbl.cn/gtkpfduhaq.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.zhengqikj.top/gtuuommpyb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.birdmap.top/gtqerndtdu.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.aizwys.cn/gtwtsytpij.html

C#:   3.14159.ToString("F2")
来源：http://hz.yueranfly.top/gtscnrihtm.html

[A22] 获取字符串长度
来源：http://hz.pycfn.com/gtmlidxlil.html

Py:   len(s)
来源：http://hz.ybcxt.top/gtzuspqpkv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.yuxming.cn/gtbelbrnrs.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.ppjwa.cn/gtlvqpurjh.html

TS:   s.length
来源：http://hz.guannengcc.top/gtkcpqdevy.html

Java: s.length()
来源：http://hz.xingfuxueyuan.xyz/gtqergstrg.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.hnxiangtu.top/gtxitprnai.html

Ruby: s.length
来源：http://hz.hfpthk.cn/gtifupbajo.html

C#:   s.Length
来源：http://hz.smart0.xyz/gtwxjswhbs.html

[A23] 大小写转换
来源：http://hz.meibo888.top/gtqksecvdy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.zhixingplan.top/gtctvtngmi.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.svipenyu.cn/gtkoydlcvx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.quarkkingdee.top/gtxrinouwq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.snrcjt.cn/gtpncdkrul.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.aibaodan.cn/gtorhzujab.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.ywan-chungtsiang.top/gtbkdagums.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.xingfuxueyuan.xyz/gthytilpiw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.shangyingyoupin.top/gtnvupzktt.html

[A24] 去除首尾空白
来源：http://hz.gaohongyu789.top/gtwmprbiso.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.jinqigufen.top/gtjzdszlby.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.jqgufenzy.top/gtgzivvatc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.nanxuanxn.top/gtuafcribb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.aizwys.cn/gtfxmzjkdz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.snrcjt.cn/gtzsdomvny.html

Go:   strings.TrimSpace(s)
来源：http://hz.pycfn.com/gtjpoksezx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.yvedp.cn/gtgoeexuay.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.jinyuanbaomall.cn/gtwdizkisr.html

[A25] 字符串比较
来源：http://hz.xuetiantiany.cn/gtgfwlgdcq.html

Py:   s1 == s2; s1 != s2
来源：http://hz.jqgufenzy.top/gteagmmvle.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.0kj1m.cn/gtovlrtevw.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.havefunace.top/gtroxrmhka.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.shuidangran.top/gtgopegenn.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.zhoulong.xyz/gtaxbaplcq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.jinqigufen.top/gtzrkduiam.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.52xcode.cn/gtcspocrzc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.xziqi.cn/gttuhnryas.html

[A26] 类型转换总览
来源：http://hz.jyoumei.cn/gtnkiifwuq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.shuidangran.top/gtemdtjeuz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.yj202588.top/gthqqwvnme.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.nanxuanxn.top/gtnhdkxpqa.html

TS:   Number() String() Boolean() x as number
来源：http://hz.xuanzx.com/gtmbitwyoc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.hnxiangtu.top/gtugdkueja.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.yangfankeji.com/gtecpbzpvf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.redwolf501.top/gtynedzweo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.ydjk.org.cn/gtkybzuwlc.html

================================================================================
来源：http://hz.gzhubu.top/gtrzvecxpi.html

B. 流程控制
来源：http://hz.cucudq.cn/gtfwxjnnir.html

================================================================================
来源：http://hz.hfpthk.cn/gtbaxadzcp.html

[B01] 条件判断 if / else
来源：http://hz.haohaochexian.top/gtrpmxnpds.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.hywenlv.cn/gtkmkmbmrc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.ydjk.org.cn/gtqqwpoguf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.shzxlz.cn/gtzlbtfbyz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.dashuyun.cn/gtkyumxfpb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.ivvv.top/gtfzvzgoti.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.dashuyun.cn/gtvzqvawal.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.snrcjt.cn/gtbqmbdfzg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.tian-w.cn/gtdoqjtxup.html

[B02] 多分支 else if / elif
来源：http://hz.ywan-chungtsiang.top/gtzvikodko.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.svipenyu.cn/gtvjmrzous.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.dashuyun.cn/gtezrovwrv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yuanzhike.top/gtwkvoprkn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xuetiantiany.cn/gtwmoieqyx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zycfv.cn/gtyezojpax.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.tanke756.top/gtwnjjnktc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.gogol.net.cn/gteahielvk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shangyingyoupin.top/gtczreymll.html

[B03] switch / match / case
来源：http://hz.sysykeji.top/gtlxiihmtb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.dashuyun.cn/gtsrqeocop.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.zycfv.cn/gtodxmmgje.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.xziqi.cn/gtdlgybrcc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.hnxiangtu.top/gtprepepxn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.birdmap.top/gtcttzwsis.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.sweek.top/gtrbzmdmdx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.ybcxt.top/gtcrhaazor.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.zhengqikj.top/gthoibzbfq.html

[B04] for 计数循环
来源：http://hz.guannengcc.top/gtcfbtskix.html

Py:   for i in range(10): print(i)
来源：http://hz.yonumen.top/gtonzffziz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.fengsongda.top/gtsgzmuuop.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.hywenlv.cn/gtnpibaibk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yj20258888.top/gtlfdefifv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.gogol.net.cn/gtvsthrqat.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.hfpthk.cn/gtwdzfephz.html

Ruby: 10.times { |i| puts i }
来源：http://hz.snrcjt.cn/gtbwocjmtd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.yongpay.top/gtnpprozxx.html

[B05] 遍历数组 / 列表
来源：http://hz.gogol.net.cn/gtbkeeoedv.html

Py:   for item in arr: print(item)
来源：http://hz.dianchejie.cn/gtodcmvhzs.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.hywenlv.cn/gtvxxuwdke.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.iojbl.cn/gtqutlqfgo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.shanyushiyangkeji.top/gtbggscwzj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.xylfe.cn/gtzjtvfkiq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.yuxming.cn/gtdmhocghw.html

Ruby: arr.each { |item| puts item }
来源：http://hz.smart0.xyz/gtarixdntb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.nanxinkj.top/gtqugyxong.html

[B06] 遍历字典 / 对象
来源：http://hz.gzhubu.top/gtgmoowcyw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.quarkkingdee.top/gtndbnwyye.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.316326.xyz/gtxehwapsu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ivvv.top/gtdogqwaba.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhongyouzk.top/gtkkkjhpcb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.yj20258.top/gtbihkgdfd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.jqgufenzy.top/gtoxslwbum.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.aibaodan.cn/gtpokcavvh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.jqgufenzy.top/gtadgigdbf.html

[B07] while 循环
来源：http://hz.zhijiandao.cn/gtgiwqecya.html

Py:   while i < 10: i += 1
来源：http://hz.wangshuangyany.cn/gtwpmoefuz.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.fengsongda.top/gtkakbcbxd.html

JS:   while (i < 10) { i++; }
来源：http://hz.zhiwuduotai.top/gtvsvvdwzz.html

TS:   while (i < 10) { i++; }
来源：http://hz.iojbl.cn/gtpxzawmnh.html

Java: while (i < 10) { i++; }
来源：http://hz.gotoacloud.top/gtomuivyon.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.chenzaomai.com/gtjmknzufj.html

Ruby: while i < 10; i += 1; end
来源：http://hz.yanxiufei.cn/gtduyippfz.html

C#:   while (i < 10) { i++; }
来源：http://hz.aibaodan.cn/gtuobwvgys.html

[B08] do-while（至少执行一次）
来源：http://hz.shzxlz.cn/gttrzewbve.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.vqdsnc.cn/gtqaxdkkbm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.svipenyu.cn/gtfhkdfvnd.html

JS:   do { i++; } while (i < 10);
来源：http://hz.tanke756.top/gtoziimcze.html

TS:   do { i++; } while (i < 10);
来源：http://hz.quarkkingdee.top/gtdlovlpfs.html

Java: do { i++; } while (i < 10);
来源：http://hz.0kj1m.cn/gtljlikcby.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.hongshengwenyu.top/gtbehcnojz.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.jyoumei.cn/gtpumtpiuo.html

C#:   do { i++; } while (i < 10);
来源：http://hz.birdmap.top/gthbfnywzi.html

[B09] break 与 continue
来源：http://hz.hywenlv.cn/gtvlcrmfos.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.yvedp.cn/gtknomxccb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.dianchejie.cn/gtxypshpez.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.kuanghao11.cn/gtohwreknc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gogol.net.cn/gteccedztb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hywenlv.cn/gtfucbjieg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.gzhubu.top/gthkgqckvo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.aizwys.cn/gtgxnamuws.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.0kj1m.cn/gtvfcmatyt.html

[B10] 遍历同时拿索引
来源：http://hz.tian-w.cn/gtwhkgitkv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.birdmap.top/gtbnhjixed.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.snrcjt.cn/gtfmnjbvjp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.sufxvd.cn/gtjhgiyeex.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.smart0.xyz/gtxnvkmuhf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.xingfuxueyuan.xyz/gtdfzdgjev.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.tianlin.xyz/gtswgkrsde.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.gotoacloud.top/gtrhfelkcv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.dashuyun.cn/gtfetyqpqq.html

[B11] 生成数字序列 / 区间
来源：http://hz.jinqigfzy.top/gtshkzlqxz.html

Py:   list(range(0, 10, 2))
来源：http://hz.kuanghao11.cn/gttoqlcsph.html

PHP:  range(0, 10, 2);
来源：http://hz.c1oappe.top/gtxhqyhmze.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.pengpengdd.cyou/gtkjmsujru.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.birdmap.top/gtgpuxxzmk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.shuidangran.top/gtzqpbwunz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.cashguo.top/gtkpznuida.html

Ruby: (0...10).step(2).to_a
来源：http://hz.0kj1m.cn/gtpddxdbvy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.shangyingyoupin.top/gtfqhycfst.html

[B12] 跳出多层循环
来源：http://hz.xuanzx.com/gtcgwjfhhm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.jqgufenzy.top/gtptgwhwaj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.chenjidiqi.icu/gtvtugktkm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.shuidangran.top/gtifxholjr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.quarkkingdee.top/gtnjdtrver.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.0kj1m.cn/gtrhfraknb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.xylfe.cn/gtmwxyfiup.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.hfpthk.cn/gttsellbwd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.havefunace.top/gtbmzfvomn.html

[B13] 判断是否为数字
来源：http://hz.ywan-chungtsiang.top/gtbjzmdatg.html

Py:   isinstance(x, (int, float))
来源：http://hz.smart0.xyz/gtaaxyzjuq.html

PHP:  is_numeric($x)
来源：http://hz.chenlongwang.top/gtetmroeyc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.316326.xyz/gttsqcxvrp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.gzhubu.top/gtmwrypazo.html

Java: x instanceof Number
来源：http://hz.shanyushiyangtech.top/gtkmousltn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yj20258.top/gtalyeueiw.html

Ruby: x.is_a?(Numeric)
来源：http://hz.tian-w.cn/gthwxuxpcr.html

C#:   x is int or double or decimal
来源：http://hz.yuxming.cn/gtyiiezldi.html

[B14] 判断值是否在集合内
来源：http://hz.shzxlz.cn/gtuacedjlu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zhongyouzk.top/gtilnspxyc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yj20258888.top/gtixegywkv.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.haohaochexian.top/gtkklgpqxd.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.0kj1m.cn/gtcfkbkcij.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.xuanzx.com/gteyekzayo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.ydzc1.top/gtdhbffuhq.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.jianghu66.top/gtwnqzqyoi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jiagoushi.top/gtarpanjdp.html

[B15] 布尔运算与取反
来源：http://hz.cdnleiting.top/gthbrypklf.html

Py:   a and b or not c
来源：http://hz.ywan-chungtsiang.top/gtvjwmeecz.html

PHP:  $a && $b || !$c
来源：http://hz.tianlin.xyz/gtwssrodfr.html

JS:   a && b || !c
来源：http://hz.xziqi.cn/gtzyqwbvpd.html

TS:   a && b || !c
来源：http://hz.quarkkingdee.top/gtussgkbdy.html

Java: a && b || !c
来源：http://hz.jinqigfzy.top/gtystvbrrk.html

Go:   a && b || !c
来源：http://hz.316326.xyz/gttsbozxxr.html

Ruby: a && b || !c
来源：http://hz.zdqjudy.top/gtlxudlurb.html

C#:   a && b || !c
来源：http://hz.andypj.xyz/gtolesawvr.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yuanzhike.top/gtpfqtcvkj.html

Py:   if not data: return
来源：http://hz.hnqzz.top/gttrdnfkvw.html

PHP:  if (!$data) { return; }
来源：http://hz.pycfn.com/gtfxbbtiwc.html

JS:   if (!data) return;
来源：http://hz.chenlongwang.top/gtxvejsiuk.html

TS:   if (!data) return;
来源：http://hz.andypj.xyz/gtaoijfpia.html

Java: if (data == null) return;
来源：http://hz.cdnleiting.top/gtdurtaqod.html

Go:   if data == nil { return }
来源：http://hz.jqgufenzy.top/gtxencmqtf.html

Ruby: return if data.nil?
来源：http://hz.jiagoushi.top/gtcwclhyzi.html

C#:   if (data == null) return;
来源：http://hz.chenjidiqi.icu/gtewlrkeoz.html

================================================================================
来源：http://hz.meibo888.top/gthyhxoueo.html

C. 函数与作用域
来源：http://hz.jqgfzy.top/gtwuisfaym.html

================================================================================
来源：http://hz.nanxuanxn.top/gtjmohgggy.html

[C01] 定义函数
来源：http://hz.vqdsnc.cn/gtdybxnuqz.html

Py:   def add(a, b): return a + b
来源：http://hz.ydzc1.top/gtfzfnmeml.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hongshengwenyu.top/gtdhkkbikh.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.sweek.top/gtaxruxcuq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.wangdashe.top/gtdllkxier.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jqgufenzy.top/gtcqnmciyx.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.fzhhl.top/gtasijrlsk.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jinqigfzy.top/gtlylpnqos.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yueranfly.top/gthsvzlxfo.html

[C02] 默认参数
来源：http://hz.guowangkeji.top/gtrgmenhzc.html

Py:   def greet(name="World"): return name
来源：http://hz.meibo888.top/gtcmhkgywl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jinyuanbaomall.cn/gtytfvwmse.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yj20258888.top/gthtmexbiq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.sysykeji.top/gtxtjrfifi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.andypj.xyz/gtuxdkjjgt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yonumen.top/gtxkfwzmnm.html

Ruby: def greet(name = "World") = name
来源：http://hz.yvedp.cn/gtftyadxgs.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.nanxinkj.top/gtrjukohgf.html

[C03] 可变参数
来源：http://hz.dianchejie.cn/gtyiemicmk.html

Py:   def total(*args): return sum(args)
来源：http://hz.shanyushiyangkeji.top/gtbcwryvux.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.shzxlz.cn/gtjagcdhxc.html


<!-- 参考信息 -->