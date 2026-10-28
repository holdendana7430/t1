代发 wailian999

Java: "第一行\n第二行"
来源：http://hz.hnxiangtu.top/gtoqxhvjqo.html

Go:   "第一行\n第二行"
来源：http://hz.jinqigufen.top/gtlzrbddcg.html

Ruby: "第一行\n第二行"
来源：http://hz.yvedp.cn/gtthwsytnf.html

C#:   "第一行\n第二行"
来源：http://hz.jianghu66.top/gtsrgqfgvb.html

[A14] 注释写法
来源：http://hz.chenzaomai.com/gtffzcnazc.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.jianghu66.top/gtjpuuauww.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.daria6918.cn/gtublkpcll.html

JS:   // 单行；/* 多行 */
来源：http://hz.zhengqikj.top/gtxnjhaeoy.html

TS:   // 单行；/* 多行 */
来源：http://hz.jinqigfzy.top/gtdrshnfed.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.tian-w.cn/gtxnxgguah.html

Go:   // 单行；/* 多行 */
来源：http://hz.zhiwuduotai.top/gtmmimbxpj.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.shangyingyoupin.top/gtebaqzwgh.html

C#:   // 单行；/* 多行 */
来源：http://hz.nanxinkj.top/gtsnagavay.html

[A15] 空值判断与默认值
来源：http://hz.gzhubu.top/gthnqqckhv.html

Py:   value = data or "默认值"
来源：http://hz.hnqzz.top/gttyefwpid.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.meibo888.top/gteodomnrc.html

JS:   const value = data ?? "默认值";
来源：http://hz.wangshuangyany.cn/gtudndnzts.html

TS:   const value = data ?? "默认值";
来源：http://hz.gogol.net.cn/gtfdpbcjtu.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.hfpthk.cn/gtncfwewtk.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.yvedp.cn/gtjzsscyuu.html

Ruby: value = data || "默认值"
来源：http://hz.zdqjudy.top/gtqnrygwkf.html

C#:   var value = data ?? "默认值";
来源：http://hz.hfpthk.cn/gtkixnfiaj.html

[A16] 真假值判断规则
来源：http://hz.yj202588.top/gtfkdvqkyy.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.shzxlz.cn/gtajbgjvvz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.316326.xyz/gtylmaircm.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.smart0.xyz/gtuzjauqim.html

TS:   if (!x) {}
来源：http://hz.0kj1m.cn/gtiqqhndht.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.nanxuanxn.top/gtossptnns.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.yongpay.top/gtkgzdiofw.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.yongpay.top/gtbajypedt.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.jqgfzy.top/gtcjipletb.html

[A17] 位运算
来源：http://hz.c1oappe.top/gtkuhftpkx.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jqgfzy.top/gthiyqyfrj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.yj20258.top/gtmkccdlik.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.9152youxi.cn/gtcfloswmc.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.jqgufenzy.top/gtapmwnbgt.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.havefunace.top/gtrlqjqzxb.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.zhijiandao.cn/gttbaatrvm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.gzhubu.top/gtqxizobhp.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.meibo888.top/gtjzqgojis.html

[A18] 字符与 ASCII 码互转
来源：http://hz.c1oappe.top/gtngipkbxc.html

Py:   ord("A"); chr(65)
来源：http://hz.xingfuxueyuan.xyz/gtbhdbayvx.html

PHP:  ord("A"); chr(65)
来源：http://hz.pycfn.com/gtfervsbwd.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.pengpengdd.cyou/gthfjbmykc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.havefunace.top/gtkxpgdxej.html

Java: (int) 'A'; (char) 65
来源：http://hz.tanke756.top/gtvhvxefmo.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.dianchejie.cn/gtibjawfxi.html

Ruby: "A".ord; 65.chr
来源：http://hz.ivvv.top/gtanpgysiq.html

C#:   (int)'A'; (char)65
来源：http://hz.smart0.xyz/gtzylkqeym.html

[A19] 交换两个变量
来源：http://hz.hysaishi.cn/gtqgpvqvhk.html

Py:   a, b = b, a
来源：http://hz.yj20258888.top/gtjgeupnlf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.ywan-chungtsiang.top/gtqpohikvy.html

JS:   [a, b] = [b, a];
来源：http://hz.ydjk.org.cn/gtbubbcdur.html

TS:   [a, b] = [b, a];
来源：http://hz.meibo888.top/gtybagnxoy.html

Java: int t = a; a = b; b = t;
来源：http://hz.ywan-chungtsiang.top/gttkdsjsgs.html

Go:   a, b = b, a
来源：http://hz.xuetiantiany.cn/gtyzlpzhst.html

Ruby: a, b = b, a
来源：http://hz.redwolf501.top/gttxqptlsa.html

C#:   (a, b) = (b, a);
来源：http://hz.yj20258.top/gtpkmzgdbp.html

[A20] 读取标准输入
来源：http://hz.ivvv.top/gtsbbufwjp.html

Py:   name = input("请输入：")
来源：http://hz.jiagoushi.top/gtgcraaveg.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.nanxuanxn.top/gtdqspoiyl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.0kj1m.cn/gtjqkcujeh.html

TS:   // Node.js：readline 模块
来源：http://hz.zhiwuduotai.top/gtwidigdkn.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.cashguo.top/gtdjszhywt.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.kuanghao11.cn/gtlemsaswx.html

Ruby: gets.chomp
来源：http://hz.fzhhl.top/gtkkgvnzno.html

C#:   Console.ReadLine();
来源：http://hz.redwolf501.top/gtulcqsvio.html

[A21] 保留指定小数位输出
来源：http://hz.zdqjudy.top/gtspbpzjok.html

Py:   f"{3.14159:.2f}"
来源：http://hz.fengsongda.top/gtckeerakx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.guowangkeji.top/gtsexjpsez.html

JS:   (3.14159).toFixed(2)
来源：http://hz.cashguo.top/gtlbveyrxf.html

TS:   (3.14159).toFixed(2)
来源：http://hz.ybcxt.top/gtxjmqjyux.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.yanxiufei.cn/gtnykyggla.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.dashuyun.cn/gtxwzlveac.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.chenzaomai.com/gtkrytphoa.html

C#:   3.14159.ToString("F2")
来源：http://hz.xylfe.cn/gtfeurnzcx.html

[A22] 获取字符串长度
来源：http://hz.gotoacloud.top/gthpxpqfmh.html

Py:   len(s)
来源：http://hz.ybcxt.top/gtffxurlcy.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.yvedp.cn/gtmtxqbpuv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.dianchejie.cn/gtbfnssncd.html

TS:   s.length
来源：http://hz.svipenyu.cn/gtfzaepqqu.html

Java: s.length()
来源：http://hz.52xcode.cn/gtaeyglmjx.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.0kj1m.cn/gtnaewsdom.html

Ruby: s.length
来源：http://hz.havefunace.top/gtqsavawwc.html

C#:   s.Length
来源：http://hz.shzxlz.cn/gtbyriqiex.html

[A23] 大小写转换
来源：http://hz.yueranfly.top/gtiaipohbu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.tianlin.xyz/gtscrbbeom.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.feifeiyinyue.top/gtjrqlwtxc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.shanyushiyangkeji.top/gtgdodrtqc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.snrcjt.cn/gtqdmquphl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.zdqjudy.top/gtinklourl.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.jinyuanbaomall.cn/gtgabxfmvm.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.ppjwa.cn/gttzdezxuh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.daxiang520.top/gtcgltdyvi.html

[A24] 去除首尾空白
来源：http://hz.yonumen.top/gtjfanirom.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.svipenyu.cn/gthjmdqidt.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.pycfn.com/gtelxxqtsm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.gaohongyu789.top/gtlrtlfjwq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.dianchejie.cn/gtfwpjtndt.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.vqdsnc.cn/gtqlkwbfiy.html

Go:   strings.TrimSpace(s)
来源：http://hz.daxiang520.top/gtidmnckxn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.yj20258888.top/gtvnzkhkim.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.gaohongyu789.top/gtrjrvwzdy.html

[A25] 字符串比较
来源：http://hz.jqgufenzy.top/gteuztcypr.html

Py:   s1 == s2; s1 != s2
来源：http://hz.0kj1m.cn/gtnsgovqet.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.sxryk.cn/gtbobiznlq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.nanxuanxn.top/gtqivwlzms.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.tianlin.xyz/gtihggtebg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.yuxming.cn/gtvqyndstd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.jinqigufen.top/gtkvhlklnt.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.svipenyu.cn/gtltdvvnsi.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.yangfankeji.com/gtcsjwbsjr.html

[A26] 类型转换总览
来源：http://hz.xylfe.cn/gtxygznvxu.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.andypj.xyz/gtdeeaulcs.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.cashguo.top/gtfjhmwqai.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.sysykeji.top/gtkmvcicoa.html

TS:   Number() String() Boolean() x as number
来源：http://hz.pengpengdd.cyou/gtmoamcsmd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.hfpthk.cn/gtjvseuzpl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.ydjk.org.cn/gtnjcnyusk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.sysykeji.top/gtridhchzs.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.ydjk.org.cn/gtehhvbfyi.html

================================================================================
来源：http://hz.smart0.xyz/gtwqcnrrwe.html

B. 流程控制
来源：http://hz.xuetiantiany.cn/gttzvxcdqv.html

================================================================================
来源：http://hz.guowangkeji.top/gtsubgeery.html

[B01] 条件判断 if / else
来源：http://hz.vqdsnc.cn/gtafskjote.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.zycfv.cn/gtczppzese.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.havefunace.top/gtffziwull.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.9152youxi.cn/gtrladvqup.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.shangyingyoupin.top/gtdcnhihvt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.ehwqpu.com/gtrtphigie.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.cheryme.top/gttqmoxgxi.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.yongpay.top/gtzddeajxy.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.gogol.net.cn/gtexpstlet.html

[B02] 多分支 else if / elif
来源：http://hz.mhx1999.top/gtiaxdgsbw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.9152youxi.cn/gtdneqoghh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.yanxiufei.cn/gtfdrnfget.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gaohongyu789.top/gtqqmasohc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shzxlz.cn/gturnejmja.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yj20258888.top/gtopfrzpjy.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.zhoulong.xyz/gtqawfefps.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.jinghuilouyu.cn/gtqvcvaidh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yvedp.cn/gtsjqzcalf.html

[B03] switch / match / case
来源：http://hz.ppjwa.cn/gtfszpbsfj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.shzxlz.cn/gtazfyvzqo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.bjfxy.top/gtrhnzlgip.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.chenlongwang.top/gttahrnorr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yvedp.cn/gthnwzwqgl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.jlsjyb.cn/gtxvwdzzql.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.0kj1m.cn/gtqonnozdg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.mhx1999.top/gturajgblk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.zhengqikj.top/gtihkobzas.html

[B04] for 计数循环
来源：http://hz.jlsjyb.cn/gttzlajdxw.html

Py:   for i in range(10): print(i)
来源：http://hz.jinghuilouyu.cn/gtaswhjcvw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.gogol.net.cn/gtzjegxldk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yvedp.cn/gtuqvehxke.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.hammf.cn/gtkpsamfgf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.wangdashe.top/gtfqummopb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.feifeiyinyue.top/gtawjmarky.html

Ruby: 10.times { |i| puts i }
来源：http://hz.guannengcc.top/gtwqmzsawd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.gzhubu.top/gtspbzoqzh.html

[B05] 遍历数组 / 列表
来源：http://hz.bjfxy.top/gtpfpywlcs.html

Py:   for item in arr: print(item)
来源：http://hz.nanxuanxn.top/gternrgobd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.pengpengdd.cyou/gtqufvrhnh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.shanyushiyangtech.top/gthwtokxds.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.tanke756.top/gtfanmbilf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.tanke756.top/gtrnxosjnp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.feifeiyinyue.top/gtxvbnymgp.html

Ruby: arr.each { |item| puts item }
来源：http://hz.feifeiyinyue.top/gtytyxramt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.0kj1m.cn/gtrrzsqvhf.html

[B06] 遍历字典 / 对象
来源：http://hz.yueranfly.top/gtankeirpo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.zhijiandao.cn/gtduzqnjbs.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.daria6918.cn/gtptkemris.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.tanke756.top/gtpjnzbjrw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.iojbl.cn/gtloovlcbx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.ivvv.top/gtwslcnvpg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.nwbrower.top/gtjxirxfho.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.jlsjyb.cn/gtbpvwivya.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.shzxlz.cn/gtuatnyriq.html

[B07] while 循环
来源：http://hz.bjfxy.top/gttzzgxpzi.html

Py:   while i < 10: i += 1
来源：http://hz.yuxming.cn/gtycxsgjoi.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yongpay.top/gtjtwqqkcl.html

JS:   while (i < 10) { i++; }
来源：http://hz.zhijiandao.cn/gtwgzamnlo.html

TS:   while (i < 10) { i++; }
来源：http://hz.daria6918.cn/gtzgdzvwmm.html

Java: while (i < 10) { i++; }
来源：http://hz.jinqigfzy.top/gtqrdsnygx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.hnxiangtu.top/gtqjagvkgs.html

Ruby: while i < 10; i += 1; end
来源：http://hz.c1oappe.top/gtknghtsxv.html

C#:   while (i < 10) { i++; }
来源：http://hz.pengpengdd.cyou/gtzlnoeesa.html

[B08] do-while（至少执行一次）
来源：http://hz.tianlin.xyz/gtjkqkstov.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.sxryk.cn/gtxmmggzfl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zhiwuduotai.top/gttgnzfyav.html

JS:   do { i++; } while (i < 10);
来源：http://hz.gaohongyu789.top/gtcwusqryp.html

TS:   do { i++; } while (i < 10);
来源：http://hz.guowangkeji.top/gtvpxvkjqu.html

Java: do { i++; } while (i < 10);
来源：http://hz.yuanzhike.top/gtasalmchp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.zhiwuduotai.top/gtymdvqskw.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.xinyue.icu/gtfxybkgfr.html

C#:   do { i++; } while (i < 10);
来源：http://hz.dianchejie.cn/gttjwxrvtk.html

[B09] break 与 continue
来源：http://hz.sxryk.cn/gtvuudltzz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.pycfn.com/gtzpjqoxti.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.xingfuxueyuan.xyz/gtdjzmwbkp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yangfankeji.com/gtssnsiokr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.mhx1999.top/gtojvxnjfg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ywan-chungtsiang.top/gtckeouuwa.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.yvedp.cn/gtbplymvip.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.xylfe.cn/gttjyfhtmr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ywan-chungtsiang.top/gtdrimuswz.html

[B10] 遍历同时拿索引
来源：http://hz.yonumen.top/gtwwmzzeuk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.guowangkeji.top/gtfhxggmjz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.sweek.top/gtxjsmougi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.yanxiufei.cn/gtcvatyktb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.bjfxy.top/gtzhuqpqfn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.cdnleiting.top/gtavfjawkk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.xuanzx.com/gtkqrhoawh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.cheryme.top/gtzqvntoiu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.yvedp.cn/gtywarepvq.html

[B11] 生成数字序列 / 区间
来源：http://hz.nanxuanxn.top/gtgisxgewu.html

Py:   list(range(0, 10, 2))
来源：http://hz.iojbl.cn/gtmszthwmx.html

PHP:  range(0, 10, 2);
来源：http://hz.jiagoushi.top/gtqqvzthmr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xylfe.cn/gtomqhqvza.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yanxiufei.cn/gtizjaxkup.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.wangdashe.top/gtkjqdoedt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jinghuilouyu.cn/gtpfcrogvx.html

Ruby: (0...10).step(2).to_a
来源：http://hz.vqdsnc.cn/gtfguolqre.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.hywenlv.cn/gtpdzeeczh.html

[B12] 跳出多层循环
来源：http://hz.kuanghao11.cn/gtnuncaphx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.dashuyun.cn/gtzomxmrhl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.yanxiufei.cn/gtbipdxqmh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yanxiufei.cn/gtognhpdjo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sxryk.cn/gtivubtymx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.ppjwa.cn/gtukxijrss.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.hfpthk.cn/gthdjjfvjm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.feifeiyinyue.top/gttpiktyls.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.shuidangran.top/gtulqbfomy.html

[B13] 判断是否为数字
来源：http://hz.jinqigfzy.top/gtsmmmujcn.html

Py:   isinstance(x, (int, float))
来源：http://hz.haohaochexian.top/gtwelnmqds.html

PHP:  is_numeric($x)
来源：http://hz.iojbl.cn/gtmyyquurl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jqgufenzy.top/gthzpnuafr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shangyingyoupin.top/gtctupjxeh.html

Java: x instanceof Number
来源：http://hz.ybcxt.top/gtbijshssg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yvedp.cn/gtsgkjvjzi.html

Ruby: x.is_a?(Numeric)
来源：http://hz.xuetiantiany.cn/gtwfbihaci.html

C#:   x is int or double or decimal
来源：http://hz.yuanzhike.top/gtuydzzmmy.html

[B14] 判断值是否在集合内
来源：http://hz.hnqzz.top/gtuaielvyi.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.cdnleiting.top/gtnxzdhixj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.sysykeji.top/gtpvcrhisl.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.redwolf501.top/gtvdrqdykc.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.nanxinkj.top/gtkrzotteo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.hnqzz.top/gttiogbtvj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.pycfn.com/gtcacewpog.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.zhengqikj.top/gteowhopco.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.svipenyu.cn/gtpxcbcxzb.html

[B15] 布尔运算与取反
来源：http://hz.aibaodan.cn/gtkmiumiow.html

Py:   a and b or not c
来源：http://hz.shangyingyoupin.top/gtamsqciqq.html

PHP:  $a && $b || !$c
来源：http://hz.jyoumei.cn/gthvsskity.html

JS:   a && b || !c
来源：http://hz.hongshengwenyu.top/gtsllyuzhr.html

TS:   a && b || !c
来源：http://hz.xinyue.icu/gthzjsigzd.html

Java: a && b || !c
来源：http://hz.9152youxi.cn/gtmuecbuyo.html

Go:   a && b || !c
来源：http://hz.zhixingplan.top/gteejghreq.html

Ruby: a && b || !c
来源：http://hz.nanxinkj.top/gtcyuebopl.html

C#:   a && b || !c
来源：http://hz.yuanzhike.top/gtgiqtvogy.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.cheryme.top/gtholwnlhj.html

Py:   if not data: return
来源：http://hz.gotoacloud.top/gtrstvrfoo.html

PHP:  if (!$data) { return; }
来源：http://hz.yj202588.top/gtfzsdbggd.html

JS:   if (!data) return;
来源：http://hz.hammf.cn/gtzipeupdg.html

TS:   if (!data) return;
来源：http://hz.quarkkingdee.top/gtmdftstzv.html

Java: if (data == null) return;
来源：http://hz.quarkkingdee.top/gtermnfatk.html

Go:   if data == nil { return }
来源：http://hz.jianghu66.top/gtinrrwzmt.html

Ruby: return if data.nil?
来源：http://hz.hnqzz.top/gtmphbyhwr.html

C#:   if (data == null) return;
来源：http://hz.redwolf501.top/gtvvdfyefx.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtpxnkgfxr.html

C. 函数与作用域
来源：http://hz.ivvv.top/gtktvuahkj.html

================================================================================
来源：http://hz.zhoulong.xyz/gtnpmotkmw.html

[C01] 定义函数
来源：http://hz.xuetiantiany.cn/gtufhrmwiv.html

Py:   def add(a, b): return a + b
来源：http://hz.cqqwz.cn/gtfxqprrnd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.daria6918.cn/gtxmryyklr.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.shzxlz.cn/gtiktjatvx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jqgfzy.top/gtvxkafsjv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xylfe.cn/gtelqdovwp.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.shanyushiyangtech.top/gtacviwevg.html

Ruby: def add(a, b); a + b; end
来源：http://hz.cheryme.top/gtycrpvygn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.hywenlv.cn/gthivvtmrr.html

[C02] 默认参数
来源：http://hz.yj20258888.top/gtmulwyncp.html

Py:   def greet(name="World"): return name
来源：http://hz.hywenlv.cn/gtyfuhovir.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.wangshuangyany.cn/gtchqscuhc.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.andypj.xyz/gtaedkfahq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.gaohongyu789.top/gtczgoxqrh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.snrcjt.cn/gtcafxzftz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.cdnleiting.top/gtdbspgwtb.html

Ruby: def greet(name = "World") = name
来源：http://hz.gaohongyu789.top/gthflolyqr.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yonumen.top/gtpxxbiwsq.html

[C03] 可变参数
来源：http://hz.jiagoushi.top/gtoyanfdkk.html

Py:   def total(*args): return sum(args)
来源：http://hz.zhiwuduotai.top/gteyqwmtva.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.tanke756.top/gtqgwvsjkk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cdnleiting.top/gtkptzywpc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yuxming.cn/gtlpvhongo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.dianchejie.cn/gtqvgqgtvb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.chenlongwang.top/gtgsjndzbw.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.guannengcc.top/gtnksqfebd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.gzhubu.top/gtomiiwizo.html

[C04] 命名参数 / 关键字参数
来源：http://hz.gzhubu.top/gtepnrheem.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yanxiufei.cn/gtlslpgoaj.html


<!-- 参考信息 -->