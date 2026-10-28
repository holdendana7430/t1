代发 wailian999

[A14] 注释写法
来源：http://hz.feifeiyinyue.top/gtrgsnzxfk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.sweek.top/gtmztyawzw.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.ywan-chungtsiang.top/gtqhuhcute.html

JS:   // 单行；/* 多行 */
来源：http://hz.iojbl.cn/gtkvvermyt.html

TS:   // 单行；/* 多行 */
来源：http://hz.sysykeji.top/gtoierhiym.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.c1oappe.top/gtcyzjdvmx.html

Go:   // 单行；/* 多行 */
来源：http://hz.jqgufenzy.top/gtzxxjuggw.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.ehwqpu.com/gtcuhzlman.html

C#:   // 单行；/* 多行 */
来源：http://hz.gogol.net.cn/gtkyjhzocm.html

[A15] 空值判断与默认值
来源：http://hz.xingfuxueyuan.xyz/gtmfzrxjvn.html

Py:   value = data or "默认值"
来源：http://hz.yangfankeji.com/gtvuqcfipp.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.52xcode.cn/gtnsuhixhj.html

JS:   const value = data ?? "默认值";
来源：http://hz.pycfn.com/gtjijnnagh.html

TS:   const value = data ?? "默认值";
来源：http://hz.yj20258888.top/gtfqtrqoml.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.yongpay.top/gtnirpwbmi.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.zhengqikj.top/gtkihecmgb.html

Ruby: value = data || "默认值"
来源：http://hz.zhijiandao.cn/gtjvlukgku.html

C#:   var value = data ?? "默认值";
来源：http://hz.shanyushiyangtech.top/gtqnaqhqfb.html

[A16] 真假值判断规则
来源：http://hz.svipenyu.cn/gtlnnpfyup.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.zhoulong.xyz/gtxvfwlnmm.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.pycfn.com/gthaawrbef.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.yanxiufei.cn/gtgtgvqaod.html

TS:   if (!x) {}
来源：http://hz.ywan-chungtsiang.top/gtyjzarthx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.9152youxi.cn/gtgcsdwsti.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.shanyushiyangtech.top/gthwpnlsml.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.shanyushiyangkeji.top/gtnrvojwxa.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.wangdashe.top/gthaeatcxf.html

[A17] 位运算
来源：http://hz.yonumen.top/gtxjnttmyo.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.iojbl.cn/gtwhdntkps.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.shangyingyoupin.top/gtezamqxhk.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ivvv.top/gtvyhjqbbl.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.yvedp.cn/gtcqojeskm.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.fzhhl.top/gtjjvtnzeo.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.hysaishi.cn/gtanztgbvl.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yueranfly.top/gtieghwyxe.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hysaishi.cn/gttbwzgsnf.html

[A18] 字符与 ASCII 码互转
来源：http://hz.yuanzhike.top/gtwlmtojfq.html

Py:   ord("A"); chr(65)
来源：http://hz.xziqi.cn/gtdlzhqtuy.html

PHP:  ord("A"); chr(65)
来源：http://hz.sxryk.cn/gtmqxqkciw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.zhengqikj.top/gtonlmkadk.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.yangfankeji.com/gtscmbqngr.html

Java: (int) 'A'; (char) 65
来源：http://hz.birdmap.top/gtaexklhqm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.xuetiantiany.cn/gtnpzsrtpq.html

Ruby: "A".ord; 65.chr
来源：http://hz.fengsongda.top/gtqmqiblfl.html

C#:   (int)'A'; (char)65
来源：http://hz.ywan-chungtsiang.top/gtqgpuzyox.html

[A19] 交换两个变量
来源：http://hz.wangshuangyany.cn/gtkgjxfwpm.html

Py:   a, b = b, a
来源：http://hz.jyoumei.cn/gtkavaovwz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.yj20258.top/gtibhvvxyh.html

JS:   [a, b] = [b, a];
来源：http://hz.shzxlz.cn/gtlcbjqhtj.html

TS:   [a, b] = [b, a];
来源：http://hz.shangyingyoupin.top/gtpcfgikxc.html

Java: int t = a; a = b; b = t;
来源：http://hz.52xcode.cn/gtwmdmlvxv.html

Go:   a, b = b, a
来源：http://hz.yj20258888.top/gtmtamhshy.html

Ruby: a, b = b, a
来源：http://hz.jinqigufen.top/gtnjbbubef.html

C#:   (a, b) = (b, a);
来源：http://hz.pengpengdd.cyou/gtrzrquyjt.html

[A20] 读取标准输入
来源：http://hz.ehwqpu.com/gthkvfcmjt.html

Py:   name = input("请输入：")
来源：http://hz.shanyushiyangkeji.top/gthuvmzleo.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.xinyue.icu/gtxjequwtl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.ybcxt.top/gtmyqlazqs.html

TS:   // Node.js：readline 模块
来源：http://hz.xingfuxueyuan.xyz/gthepawwbn.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.smart0.xyz/gtataltdkz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.jqgufenzy.top/gtdtvigbsr.html

Ruby: gets.chomp
来源：http://hz.yanxiufei.cn/gtltoyprec.html

C#:   Console.ReadLine();
来源：http://hz.sxryk.cn/gthrgxxkhj.html

[A21] 保留指定小数位输出
来源：http://hz.aibaodan.cn/gtgstjrziw.html

Py:   f"{3.14159:.2f}"
来源：http://hz.dianchejie.cn/gtjnuxtouz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.xinyue.icu/gtbmcjgiss.html

JS:   (3.14159).toFixed(2)
来源：http://hz.hysaishi.cn/gtqnjxteye.html

TS:   (3.14159).toFixed(2)
来源：http://hz.jianghu66.top/gtmohhapsp.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.shuidangran.top/gtllicqcfx.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.pengpengdd.cyou/gtzpinyojv.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.fengsongda.top/gtpgafbjqo.html

C#:   3.14159.ToString("F2")
来源：http://hz.ybcxt.top/gtuiysmpqv.html

[A22] 获取字符串长度
来源：http://hz.dashuyun.cn/gtzyvedfhc.html

Py:   len(s)
来源：http://hz.gzhubu.top/gtxmssvvgj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.sysykeji.top/gtwfnvmqng.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.kuanghao11.cn/gtrpeklobp.html

TS:   s.length
来源：http://hz.zhongyouzk.top/gtafpkubvu.html

Java: s.length()
来源：http://hz.yonumen.top/gtumtebgxq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.mhx1999.top/gtnfayumfv.html

Ruby: s.length
来源：http://hz.andypj.xyz/gthjkzvnba.html

C#:   s.Length
来源：http://hz.fzhhl.top/gttdhxmsts.html

[A23] 大小写转换
来源：http://hz.dianchejie.cn/gtryelddop.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.fzhhl.top/gtwhghcers.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.sxryk.cn/gtjxomsyxp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.sufxvd.cn/gtjfhpnfqy.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.daria6918.cn/gtcylhclim.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.yuxming.cn/gtatbojsux.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.guowangkeji.top/gtywhuiycn.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.ivvv.top/gtgqdnnrjc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.jqgufenzy.top/gttmtgxjua.html

[A24] 去除首尾空白
来源：http://hz.guannengcc.top/gtqxijajyw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.yuxming.cn/gtuusbughu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.jqgfzy.top/gtokzrntjb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.ydjk.org.cn/gtnbbczqwm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.9152youxi.cn/gtpfikzunl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.shuidangran.top/gtvizlzrwz.html

Go:   strings.TrimSpace(s)
来源：http://hz.jlsjyb.cn/gtlekkuecd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.jqgfzy.top/gtsgjfbntq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.redwolf501.top/gtlitpxjjf.html

[A25] 字符串比较
来源：http://hz.ywan-chungtsiang.top/gtxruopvmi.html

Py:   s1 == s2; s1 != s2
来源：http://hz.yuanzhike.top/gtviwjzkgg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.zycfv.cn/gtctfhbqxh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.shangyingyoupin.top/gtfdmlrnkj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.tian-w.cn/gtvxotbgfn.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.vqdsnc.cn/gtujyszluv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.dashuyun.cn/gtxeqrwwik.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.yonumen.top/gtbellyjti.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.dianchejie.cn/gtoyysdvvq.html

[A26] 类型转换总览
来源：http://hz.jinyuanbaomall.cn/gtdpomvvfv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.xuanzx.com/gtwfevnzep.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.ppjwa.cn/gtnsgjdqro.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.ivvv.top/gtysfdgnoh.html

TS:   Number() String() Boolean() x as number
来源：http://hz.yuanzhike.top/gtutcigasx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.kuanghao11.cn/gtydsvdcrd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.cucudq.cn/gttmhfduqk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.zhixingplan.top/gtvgayzwrz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.svipenyu.cn/gtzrnimvjs.html

================================================================================
来源：http://hz.52xcode.cn/gtsqvknwyq.html

B. 流程控制
来源：http://hz.hammf.cn/gtbztdeglv.html

================================================================================
来源：http://hz.smart0.xyz/gtxxoltnmq.html

[B01] 条件判断 if / else
来源：http://hz.hywenlv.cn/gtmtzpvsxk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.ppjwa.cn/gtgislaias.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.jqgfzy.top/gtmvjuuilr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.52xcode.cn/gthdokdqnp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.andypj.xyz/gtpdbfpqcu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.aizwys.cn/gtdhpfyvnt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.havefunace.top/gteslmicbx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.hywenlv.cn/gtmcfgumjf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.daxiang520.top/gtvcateoxz.html

[B02] 多分支 else if / elif
来源：http://hz.zhixingplan.top/gtzsujzgbs.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.yj20258888.top/gtlscqprzc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.xinyue.icu/gtphrknjvq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.52xcode.cn/gtzvrdbnsy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.svipenyu.cn/gtyubnukak.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cucudq.cn/gtietcqhtc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.shuidangran.top/gtqqceotwt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.ydzc1.top/gtxcpaymkx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yangfankeji.com/gtfmgfejaw.html

[B03] switch / match / case
来源：http://hz.shanyushiyangkeji.top/gtcnoiivft.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.cdnleiting.top/gtxwvgiekp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.ivvv.top/gtofoilirb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jinqigfzy.top/gtfwkkhdei.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jianghu66.top/gttmxgqjbw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.bjfxy.top/gteuwybifo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.sufxvd.cn/gtbozklrjl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.cashguo.top/gtoumvhykd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.guowangkeji.top/gtrxbxqpmt.html

[B04] for 计数循环
来源：http://hz.sweek.top/gtbulgoqdm.html

Py:   for i in range(10): print(i)
来源：http://hz.shangyingyoupin.top/gtecwnbqrl.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.gaohongyu789.top/gtlurouhdb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.vqdsnc.cn/gtzcbtfkae.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.xuanzx.com/gtjizyrora.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.dianchejie.cn/gthdhleplf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.smart0.xyz/gtpxhergcx.html

Ruby: 10.times { |i| puts i }
来源：http://hz.smart0.xyz/gtatxjqggr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.jqgfzy.top/gtekhqlscl.html

[B05] 遍历数组 / 列表
来源：http://hz.jqgfzy.top/gtknbdhfjq.html

Py:   for item in arr: print(item)
来源：http://hz.jiagoushi.top/gtqvslmsqy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.jlsjyb.cn/gtnvazyjpg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.nwbrower.top/gtosytxhtz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.jiagoushi.top/gtqhiwahnu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.cqqwz.cn/gtzmipxvvn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.nanxinkj.top/gtamnukzlb.html

Ruby: arr.each { |item| puts item }
来源：http://hz.jqgufenzy.top/gtuopgqfpu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.meibo888.top/gtzuizgnxt.html

[B06] 遍历字典 / 对象
来源：http://hz.shanyushiyangtech.top/gtxnowikhj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.bjfxy.top/gtbfbsnvbl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.sufxvd.cn/gthxubnzhh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.feifeiyinyue.top/gtixqrfdzr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.guannengcc.top/gtdazikmmd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.aizwys.cn/gtknxuderw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.daria6918.cn/gtiabmyctp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.yangfankeji.com/gtecjmknnx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.shzxlz.cn/gtvcxrgowc.html

[B07] while 循环
来源：http://hz.yonumen.top/gtcjloppuk.html

Py:   while i < 10: i += 1
来源：http://hz.gogol.net.cn/gtylzdjtuu.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.hywenlv.cn/gtlqdnwfay.html

JS:   while (i < 10) { i++; }
来源：http://hz.hammf.cn/gtbrakosgp.html

TS:   while (i < 10) { i++; }
来源：http://hz.cheryme.top/gtiuqyfoem.html

Java: while (i < 10) { i++; }
来源：http://hz.jinyuanbaomall.cn/gthsjjrrmm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.tian-w.cn/gtrrnhscjl.html

Ruby: while i < 10; i += 1; end
来源：http://hz.shangyingyoupin.top/gtzptnyqkd.html

C#:   while (i < 10) { i++; }
来源：http://hz.hysaishi.cn/gtpflwzmap.html

[B08] do-while（至少执行一次）
来源：http://hz.iojbl.cn/gtmjpncpfu.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.cucudq.cn/gtnicrnoxy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.nanxuanxn.top/gtqepgjmzx.html

JS:   do { i++; } while (i < 10);
来源：http://hz.snrcjt.cn/gttkwgphwl.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yangfankeji.com/gtrxikpubr.html

Java: do { i++; } while (i < 10);
来源：http://hz.52xcode.cn/gtnekhtgrn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.hammf.cn/gtnvqotzst.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.hywenlv.cn/gtcyljqsjp.html

C#:   do { i++; } while (i < 10);
来源：http://hz.sxryk.cn/gtbrkreqiz.html

[B09] break 与 continue
来源：http://hz.daria6918.cn/gtiqltihcv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.aizwys.cn/gtndmtoxsm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.zhiwuduotai.top/gtxznthdwm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.bjfxy.top/gthfxiwmsf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yuanzhike.top/gtxeakhtga.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sufxvd.cn/gtfysttggu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.ppjwa.cn/gtuuuewiuv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.havefunace.top/gtuuexpaau.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.redwolf501.top/gttjvlmgtp.html

[B10] 遍历同时拿索引
来源：http://hz.52xcode.cn/gtelzcwrav.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.wangshuangyany.cn/gthahgjhaz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.wangdashe.top/gtbdvxundv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.sweek.top/gtjxczojmv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.havefunace.top/gtgsmiuubh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.zdqjudy.top/gtvhxusqdb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.ehwqpu.com/gtoksqlnje.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.wangdashe.top/gtigdseqvl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.yj202588.top/gtmarjemhy.html

[B11] 生成数字序列 / 区间
来源：http://hz.gaohongyu789.top/gttopyyzff.html

Py:   list(range(0, 10, 2))
来源：http://hz.guowangkeji.top/gtveiobroi.html

PHP:  range(0, 10, 2);
来源：http://hz.vqdsnc.cn/gttcwicitm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.chenjidiqi.icu/gtmwtptedm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.sufxvd.cn/gtbtdxexog.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.smart0.xyz/gtwiopenwx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.xuetiantiany.cn/gtyzebwfnw.html

Ruby: (0...10).step(2).to_a
来源：http://hz.hfpthk.cn/gtzwzqixzw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.sufxvd.cn/gtcxgmskrd.html

[B12] 跳出多层循环
来源：http://hz.zhongyouzk.top/gtgqrzduah.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.ywan-chungtsiang.top/gtmwzgnqjw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.fengsongda.top/gtaomxhtsd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.nanxuanxn.top/gtayorqhkv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.aizwys.cn/gtfafwwarj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhixingplan.top/gttppxupqv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yj202588.top/gtzalckynz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.quarkkingdee.top/gtrvzfesaj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.snrcjt.cn/gtfjghitdn.html

[B13] 判断是否为数字
来源：http://hz.chenlongwang.top/gtrzthmziz.html

Py:   isinstance(x, (int, float))
来源：http://hz.jqgfzy.top/gtrzgtnmtf.html

PHP:  is_numeric($x)
来源：http://hz.chenzaomai.com/gtmpjxfdeh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yuanzhike.top/gtpncgdwzu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ehwqpu.com/gtcyddnarj.html

Java: x instanceof Number
来源：http://hz.hnqzz.top/gttnwibtiw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.shzxlz.cn/gtkqmrhbrm.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jqgfzy.top/gtgbdjfcxe.html

C#:   x is int or double or decimal
来源：http://hz.aibaodan.cn/gtwarrwulc.html

[B14] 判断值是否在集合内
来源：http://hz.yongpay.top/gtgaufveki.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.birdmap.top/gtqchidqnv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.shuidangran.top/gtlssoecza.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.ybcxt.top/gtooaxkbcj.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.xylfe.cn/gtluhodkwd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.shanyushiyangtech.top/gtpwwbwriv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.sufxvd.cn/gtrvrycvjt.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.guowangkeji.top/gteojntyun.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.zycfv.cn/gtxqsnchoh.html

[B15] 布尔运算与取反
来源：http://hz.daria6918.cn/gtiaemsxuy.html

Py:   a and b or not c
来源：http://hz.daria6918.cn/gtwfktygaf.html

PHP:  $a && $b || !$c
来源：http://hz.jianghu66.top/gtexbgfihp.html

JS:   a && b || !c
来源：http://hz.shanyushiyangtech.top/gtqmebhpbj.html

TS:   a && b || !c
来源：http://hz.gaohongyu789.top/gtulgwxefb.html

Java: a && b || !c
来源：http://hz.nwbrower.top/gtkefleyed.html

Go:   a && b || !c
来源：http://hz.wangshuangyany.cn/gtqbgqkipy.html

Ruby: a && b || !c
来源：http://hz.dianchejie.cn/gtmvvcwfav.html

C#:   a && b || !c
来源：http://hz.birdmap.top/gtkdpvlhgv.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.ybcxt.top/gtscnpwgid.html

Py:   if not data: return
来源：http://hz.cqqwz.cn/gtvjoaqsda.html

PHP:  if (!$data) { return; }
来源：http://hz.pengpengdd.cyou/gtqsemzath.html

JS:   if (!data) return;
来源：http://hz.yanxiufei.cn/gtoyeollaw.html

TS:   if (!data) return;
来源：http://hz.andypj.xyz/gtbyswbefg.html

Java: if (data == null) return;
来源：http://hz.wangshuangyany.cn/gtjkxwztlk.html

Go:   if data == nil { return }
来源：http://hz.sufxvd.cn/gtaunaajsa.html

Ruby: return if data.nil?
来源：http://hz.gogol.net.cn/gtpvmltqwo.html

C#:   if (data == null) return;
来源：http://hz.chenzaomai.com/gtakfjbwbn.html

================================================================================
来源：http://hz.cucudq.cn/gtncxskeoy.html

C. 函数与作用域
来源：http://hz.nwbrower.top/gtdjlkhstk.html

================================================================================
来源：http://hz.daria6918.cn/gtljodcvai.html

[C01] 定义函数
来源：http://hz.gotoacloud.top/gtvhoppmft.html

Py:   def add(a, b): return a + b
来源：http://hz.ybcxt.top/gtobbaeiaq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ybcxt.top/gtqaiytrto.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.jiagoushi.top/gtwcwocasa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.pengpengdd.cyou/gtxbmjmvpo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.cashguo.top/gthogpcuer.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jianghu66.top/gtpelinppx.html

Ruby: def add(a, b); a + b; end
来源：http://hz.quarkkingdee.top/gtukfylwqi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zhongyouzk.top/gtncexyqoh.html

[C02] 默认参数
来源：http://hz.hammf.cn/gtzmnvyrzk.html

Py:   def greet(name="World"): return name
来源：http://hz.zhengqikj.top/gtbiktzgxj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.shuidangran.top/gtlqmygvqv.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ppjwa.cn/gtiagsgkuf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jqgfzy.top/gttfehboas.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.gogol.net.cn/gtzjhickes.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yj202588.top/gtffapihvk.html

Ruby: def greet(name = "World") = name
来源：http://hz.zdqjudy.top/gteoqhobji.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.gzhubu.top/gtqtzkhmff.html

[C03] 可变参数
来源：http://hz.quarkkingdee.top/gtlpsiqjrm.html

Py:   def total(*args): return sum(args)
来源：http://hz.gogol.net.cn/gtqeonttpz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhengqikj.top/gtixiuhbps.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sxryk.cn/gtjyalmhai.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.pengpengdd.cyou/gtkrjpzczj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zdqjudy.top/gtizmcvrlz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ppjwa.cn/gtuszfyrja.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.snrcjt.cn/gtmtocgkbj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.chenlongwang.top/gtjayguemv.html

[C04] 命名参数 / 关键字参数
来源：http://hz.hfpthk.cn/gtmfevbahh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.wangshuangyany.cn/gttqvqhjuq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.shzxlz.cn/gtgrwuuifl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hnqzz.top/gtbsosmefs.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.dianchejie.cn/gtgktlwacf.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.aibaodan.cn/gtqzpszpjz.html


<!-- 参考信息 -->