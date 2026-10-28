代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.yj20258.top/gttewnhqze.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.jinqigfzy.top/gtkwddtvbm.html

TS:   if (!x) {}
来源：http://hz.hnxiangtu.top/gtohsfyscl.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.yj20258888.top/gtcwuroxkr.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.daxiang520.top/gttyfevacu.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.zhiwuduotai.top/gtwpcgnuok.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.yj20258.top/gtjnqoowko.html

[A17] 位运算
来源：http://hz.hnxiangtu.top/gtqcpzgbvu.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.tian-w.cn/gtbseuultz.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.gaohongyu789.top/gtvrvdxfxm.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yanxiufei.cn/gtadbowllq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.9152youxi.cn/gtbaopudzi.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.gzhubu.top/gthfpbkqey.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.svipenyu.cn/gtckzeidlk.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.tian-w.cn/gtmnbwalxr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yonumen.top/gtzyfmiqlo.html

[A18] 字符与 ASCII 码互转
来源：http://hz.ivvv.top/gtidgrlntk.html

Py:   ord("A"); chr(65)
来源：http://hz.ybcxt.top/gtmofxbsld.html

PHP:  ord("A"); chr(65)
来源：http://hz.gogol.net.cn/gtmiffdkkh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.havefunace.top/gtgdowheaz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.havefunace.top/gtkbzbnlgh.html

Java: (int) 'A'; (char) 65
来源：http://hz.yueranfly.top/gtlmopyuuq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.52xcode.cn/gtlajjtaza.html

Ruby: "A".ord; 65.chr
来源：http://hz.hysaishi.cn/gtgqeatstm.html

C#:   (int)'A'; (char)65
来源：http://hz.jqgufenzy.top/gtbvcycfjc.html

[A19] 交换两个变量
来源：http://hz.yanxiufei.cn/gtuzolaydy.html

Py:   a, b = b, a
来源：http://hz.zdqjudy.top/gtqlqowdhi.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.52xcode.cn/gterwbpijx.html

JS:   [a, b] = [b, a];
来源：http://hz.birdmap.top/gtlyzmyrek.html

TS:   [a, b] = [b, a];
来源：http://hz.cqqwz.cn/gtxwvnopgr.html

Java: int t = a; a = b; b = t;
来源：http://hz.birdmap.top/gtzzdiaddf.html

Go:   a, b = b, a
来源：http://hz.ydjk.org.cn/gtowcypdra.html

Ruby: a, b = b, a
来源：http://hz.chenzaomai.com/gtqwzwotmx.html

C#:   (a, b) = (b, a);
来源：http://hz.jianghu66.top/gtrkflparm.html

[A20] 读取标准输入
来源：http://hz.yj202588.top/gtndnfikjf.html

Py:   name = input("请输入：")
来源：http://hz.sufxvd.cn/gtglhreunm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.cqqwz.cn/gtjbmpltus.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.xuetiantiany.cn/gtcnedqgnb.html

TS:   // Node.js：readline 模块
来源：http://hz.yj20258888.top/gtfztyktud.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.gotoacloud.top/gthczliwrx.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.feifeiyinyue.top/gtzwunubae.html

Ruby: gets.chomp
来源：http://hz.jqgfzy.top/gtkwjpjphd.html

C#:   Console.ReadLine();
来源：http://hz.fengsongda.top/gtusctqsum.html

[A21] 保留指定小数位输出
来源：http://hz.yj20258888.top/gtmkghtldo.html

Py:   f"{3.14159:.2f}"
来源：http://hz.jinqigfzy.top/gtkmbutblb.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.ppjwa.cn/gtdusziqeq.html

JS:   (3.14159).toFixed(2)
来源：http://hz.sysykeji.top/gtwlskhhrt.html

TS:   (3.14159).toFixed(2)
来源：http://hz.gotoacloud.top/gtivdwhlys.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.fengsongda.top/gtxdlvysuk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.jinqigfzy.top/gteufbksrm.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.jlsjyb.cn/gtjuhcjfzx.html

C#:   3.14159.ToString("F2")
来源：http://hz.0kj1m.cn/gtkceesupk.html

[A22] 获取字符串长度
来源：http://hz.ybcxt.top/gtxvefdvio.html

Py:   len(s)
来源：http://hz.daxiang520.top/gtrhocskuf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.dianchejie.cn/gtjrlzutwa.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.pycfn.com/gtfafnsgvp.html

TS:   s.length
来源：http://hz.jinqigfzy.top/gtlzkysvwy.html

Java: s.length()
来源：http://hz.nwbrower.top/gtygjmoqrp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.zdqjudy.top/gthudoxmty.html

Ruby: s.length
来源：http://hz.sweek.top/gtvcdjqurw.html

C#:   s.Length
来源：http://hz.tianlin.xyz/gtppdrgxrj.html

[A23] 大小写转换
来源：http://hz.xziqi.cn/gturkuhqos.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.c1oappe.top/gtbcfgqlps.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.9152youxi.cn/gtwukxbsfa.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.zhongyouzk.top/gtlkheobeb.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.zhaomingkeji.xyz/gtkapmsyaa.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.havefunace.top/gtqkuemzox.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.ybcxt.top/gtryizhlst.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.chenjidiqi.icu/gtdbdpuagd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.jinghuilouyu.cn/gtvglyojkd.html

[A24] 去除首尾空白
来源：http://hz.redwolf501.top/gtcbulnkpi.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.birdmap.top/gtpweazejw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.xuanzx.com/gtyoejxsoe.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.gaohongyu789.top/gtoqtuvhsv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.fengsongda.top/gtxtishjbu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.shanyushiyangkeji.top/gtbebkpqol.html

Go:   strings.TrimSpace(s)
来源：http://hz.zhiwuduotai.top/gtvugynhya.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.daxiang520.top/gtutskcdct.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.xuanzx.com/gtmbhwtggh.html

[A25] 字符串比较
来源：http://hz.sufxvd.cn/gtaoxwsqbv.html

Py:   s1 == s2; s1 != s2
来源：http://hz.yj202588.top/gtvlvuceqn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.fengsongda.top/gtzvantmks.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.c1oappe.top/gtsnlvfcuj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.gotoacloud.top/gtuxotsdhg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.jinyuanbaomall.cn/gtjyrmlrtl.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.ppjwa.cn/gterztnidd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.fengsongda.top/gtzbjbtvaf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.ydzc1.top/gttzlvxvno.html

[A26] 类型转换总览
来源：http://hz.shanyushiyangtech.top/gtxourlqkt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.hnxiangtu.top/gtlmvokigf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.snrcjt.cn/gtowdalcvg.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.jinyuanbaomall.cn/gttxjotlfi.html

TS:   Number() String() Boolean() x as number
来源：http://hz.yuxming.cn/gtxdfufxoy.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.chenjidiqi.icu/gtazysqfes.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.kuanghao11.cn/gtjlsnjoqz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.cqqwz.cn/gtvgfzfebh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.ivvv.top/gtdupksimt.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtlabpjool.html

B. 流程控制
来源：http://hz.jinyuanbaomall.cn/gtnsmsndhm.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtchaeejcu.html

[B01] 条件判断 if / else
来源：http://hz.ppjwa.cn/gtzzzzjosm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.dianchejie.cn/gtsixasedj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.nanxinkj.top/gtfjluzkpr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.9152youxi.cn/gtvptxekwv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.hnxiangtu.top/gtaalnkfyr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.hammf.cn/gtxfiehrbc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.meibo888.top/gtylybhcrt.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.yj202588.top/gtyczjekre.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.xylfe.cn/gtccuxzylz.html

[B02] 多分支 else if / elif
来源：http://hz.ydjk.org.cn/gtilgrdyax.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.jinghuilouyu.cn/gtgnnwmtqa.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.c1oappe.top/gtutwlelui.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jinqigufen.top/gtjfmzkoog.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.fengsongda.top/gtziqqvhvr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ywan-chungtsiang.top/gttxlgbaze.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.xuetiantiany.cn/gtoruawuai.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.zhongyouzk.top/gtxenfxfhu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.sweek.top/gtoxunbags.html

[B03] switch / match / case
来源：http://hz.sysykeji.top/gtejiesexg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.bjfxy.top/gtvtwlykty.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.andypj.xyz/gtkaqazblm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.pycfn.com/gtwbzjyefu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.guowangkeji.top/gtwddcycvr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.nanxuanxn.top/gtuqldojfu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.xuanzx.com/gttahrzzax.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.hongshengwenyu.top/gtgtgmhhaq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.jqgfzy.top/gtathrqiqb.html

[B04] for 计数循环
来源：http://hz.havefunace.top/gtoxtmofjx.html

Py:   for i in range(10): print(i)
来源：http://hz.ybcxt.top/gtxitxdesk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.quarkkingdee.top/gtnxnvalbe.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.jqgufenzy.top/gtqnrtjbrj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yueranfly.top/gtdicnittf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.yuanzhike.top/gtqvilxbmb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.zhengqikj.top/gtsxybjpuy.html

Ruby: 10.times { |i| puts i }
来源：http://hz.vqdsnc.cn/gtxioskols.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.xziqi.cn/gtfnhojnqy.html

[B05] 遍历数组 / 列表
来源：http://hz.xinyue.icu/gtlvognkix.html

Py:   for item in arr: print(item)
来源：http://hz.cdnleiting.top/gtwwxejlit.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.wangdashe.top/gtegojrslc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.yuanzhike.top/gttwggflbs.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.jiagoushi.top/gtwgdhtnkk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.vqdsnc.cn/gtkliqkelj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.guannengcc.top/gtkpykafhg.html

Ruby: arr.each { |item| puts item }
来源：http://hz.ehwqpu.com/gtxfgcoigb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.quarkkingdee.top/gtindvkbdj.html

[B06] 遍历字典 / 对象
来源：http://hz.wangdashe.top/gtejqikjai.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.shzxlz.cn/gtqcqknvnz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.xuetiantiany.cn/gtlpyrvhpn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.wangshuangyany.cn/gtocshibug.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yanxiufei.cn/gtimkxnwsc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.cqqwz.cn/gttnbbevqw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.jlsjyb.cn/gtunlnkeid.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.redwolf501.top/gtcmgbbbmb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.shzxlz.cn/gtevnxaffw.html

[B07] while 循环
来源：http://hz.bjfxy.top/gtrynulbbo.html

Py:   while i < 10: i += 1
来源：http://hz.birdmap.top/gtsfimmgcz.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.hywenlv.cn/gtryrriooi.html

JS:   while (i < 10) { i++; }
来源：http://hz.fengsongda.top/gtintahsmb.html

TS:   while (i < 10) { i++; }
来源：http://hz.9152youxi.cn/gtsnzliheo.html

Java: while (i < 10) { i++; }
来源：http://hz.yanxiufei.cn/gtwygrwizv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.jqgufenzy.top/gtwbzqgjnz.html

Ruby: while i < 10; i += 1; end
来源：http://hz.tianlin.xyz/gtiuxshkzh.html

C#:   while (i < 10) { i++; }
来源：http://hz.daxiang520.top/gtbxomfuhz.html

[B08] do-while（至少执行一次）
来源：http://hz.tanke756.top/gtvoykwzuw.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.sysykeji.top/gtdwlojfap.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.nanxuanxn.top/gtqztxerad.html

JS:   do { i++; } while (i < 10);
来源：http://hz.zhaomingkeji.xyz/gtekuhhmfv.html

TS:   do { i++; } while (i < 10);
来源：http://hz.hnxiangtu.top/gtmpzwiaxb.html

Java: do { i++; } while (i < 10);
来源：http://hz.haohaochexian.top/gtezlurozc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.zhiwuduotai.top/gthwuntttp.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.kuanghao11.cn/gtythpeezv.html

C#:   do { i++; } while (i < 10);
来源：http://hz.yueranfly.top/gtgzwzgeyq.html

[B09] break 与 continue
来源：http://hz.xziqi.cn/gtncokoapx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.jinghuilouyu.cn/gtqcabpjea.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.xinyue.icu/gticycejlq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.iojbl.cn/gteboousgy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ivvv.top/gtyntvjyty.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhijiandao.cn/gtcnrfthix.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jinghuilouyu.cn/gtmptalsdn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.tanke756.top/gtopinsrkx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cheryme.top/gtffxjwxsz.html

[B10] 遍历同时拿索引
来源：http://hz.meibo888.top/gtmkizvoam.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.nanxuanxn.top/gtutslluvj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.gzhubu.top/gtuvdqrhyi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.yj20258.top/gtrnposwrn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.mhx1999.top/gtluwsykkq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.ehwqpu.com/gtdopavkbn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.gotoacloud.top/gtfpupmtrk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jinqigfzy.top/gtbtprbpau.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jinqigfzy.top/gtefgnkibk.html

[B11] 生成数字序列 / 区间
来源：http://hz.bjfxy.top/gthpwopmuh.html

Py:   list(range(0, 10, 2))
来源：http://hz.aizwys.cn/gtbdjdjmay.html

PHP:  range(0, 10, 2);
来源：http://hz.yongpay.top/gtwspisjyy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.snrcjt.cn/gtsegnyxpb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xinyue.icu/gtwfyeqgyf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.nanxuanxn.top/gtasfxochp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.daxiang520.top/gtwvwnxjgs.html

Ruby: (0...10).step(2).to_a
来源：http://hz.xingfuxueyuan.xyz/gtqppibuvb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.aibaodan.cn/gtivlfrxim.html

[B12] 跳出多层循环
来源：http://hz.shanyushiyangtech.top/gtzdzduufk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.quarkkingdee.top/gtawabuuia.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.sweek.top/gtplsjfcgf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yonumen.top/gtknpexixi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yonumen.top/gtulgyhnlf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.kuanghao11.cn/gtixbtfxdb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zhijiandao.cn/gtudeulcsl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.nwbrower.top/gtbdfyixti.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.cashguo.top/gtgiefcprb.html

[B13] 判断是否为数字
来源：http://hz.guowangkeji.top/gtrkjfmema.html

Py:   isinstance(x, (int, float))
来源：http://hz.xylfe.cn/gtnyrikmig.html

PHP:  is_numeric($x)
来源：http://hz.52xcode.cn/gtsdmxnnhi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shanyushiyangkeji.top/gtlyqpamle.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cucudq.cn/gtyjlyknqg.html

Java: x instanceof Number
来源：http://hz.tian-w.cn/gtclyrcdfe.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jinqigfzy.top/gttcjzvhsr.html

Ruby: x.is_a?(Numeric)
来源：http://hz.chenjidiqi.icu/gtfmbludpf.html

C#:   x is int or double or decimal
来源：http://hz.sxryk.cn/gtauemcsvj.html

[B14] 判断值是否在集合内
来源：http://hz.cheryme.top/gtjbzqolas.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.xinyue.icu/gtsxfczyrv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.zhengqikj.top/gthuddmlqk.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zhijiandao.cn/gtetuizrwb.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.zhoulong.xyz/gtzzhyxbxc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.hongshengwenyu.top/gtynmhbkry.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.guannengcc.top/gtrgzkszus.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.mhx1999.top/gtggpqbdzy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.havefunace.top/gtpimvkzvo.html

[B15] 布尔运算与取反
来源：http://hz.zdqjudy.top/gtnolyiwyd.html

Py:   a and b or not c
来源：http://hz.hysaishi.cn/gtwjtnaync.html

PHP:  $a && $b || !$c
来源：http://hz.sweek.top/gttxvtbaqw.html

JS:   a && b || !c
来源：http://hz.jqgfzy.top/gtmgqiicnl.html

TS:   a && b || !c
来源：http://hz.havefunace.top/gthqonpbew.html

Java: a && b || !c
来源：http://hz.jinyuanbaomall.cn/gtcufrkgqg.html

Go:   a && b || !c
来源：http://hz.hnxiangtu.top/gtrrhheotd.html

Ruby: a && b || !c
来源：http://hz.zhoulong.xyz/gtlbxabwle.html

C#:   a && b || !c
来源：http://hz.zhijiandao.cn/gtztumairx.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jinghuilouyu.cn/gtcbpbgjyv.html

Py:   if not data: return
来源：http://hz.9152youxi.cn/gtlnroctjo.html

PHP:  if (!$data) { return; }
来源：http://hz.xylfe.cn/gtxghlcawy.html

JS:   if (!data) return;
来源：http://hz.hfpthk.cn/gtlxewruql.html

TS:   if (!data) return;
来源：http://hz.ybcxt.top/gtkjpzndju.html

Java: if (data == null) return;
来源：http://hz.0kj1m.cn/gtxnpfyhto.html

Go:   if data == nil { return }
来源：http://hz.52xcode.cn/gtdjbzgdlm.html

Ruby: return if data.nil?
来源：http://hz.redwolf501.top/gtmwolgjml.html

C#:   if (data == null) return;
来源：http://hz.yj202588.top/gthmjzeozv.html

================================================================================
来源：http://hz.yuxming.cn/gtijcwnwze.html

C. 函数与作用域
来源：http://hz.ydzc1.top/gtlkkqukho.html

================================================================================
来源：http://hz.tianlin.xyz/gtvqbimnaw.html

[C01] 定义函数
来源：http://hz.wangdashe.top/gtunqqdasc.html

Py:   def add(a, b): return a + b
来源：http://hz.9152youxi.cn/gtnqtqercm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuanzhike.top/gtnfgwnxgl.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.mhx1999.top/gtkehsbati.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.kuanghao11.cn/gtuxvakzva.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xuetiantiany.cn/gtgscxmhur.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.havefunace.top/gtxxjwwghd.html

Ruby: def add(a, b); a + b; end
来源：http://hz.shanyushiyangkeji.top/gtvsremkhf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jiagoushi.top/gtzuavljku.html

[C02] 默认参数
来源：http://hz.hywenlv.cn/gtpbblbpxn.html

Py:   def greet(name="World"): return name
来源：http://hz.jinqigfzy.top/gtfafxcfgs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hywenlv.cn/gtalpnmdmk.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.redwolf501.top/gtzswwrhvz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.bjfxy.top/gtmsasngnk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.birdmap.top/gtoqmulcub.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.hywenlv.cn/gtievnwnlx.html

Ruby: def greet(name = "World") = name
来源：http://hz.guannengcc.top/gtfrecgusp.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.shanyushiyangtech.top/gttkndmkcd.html

[C03] 可变参数
来源：http://hz.pycfn.com/gtypgbjcxv.html

Py:   def total(*args): return sum(args)
来源：http://hz.mhx1999.top/gtovmrsdax.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ydzc1.top/gtecifkvht.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.gogol.net.cn/gtpzkvhcql.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hammf.cn/gtsohpctch.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ydzc1.top/gtxtfqkvig.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yanxiufei.cn/gtuejikufb.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ydjk.org.cn/gtfgvftpgi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zhijiandao.cn/gtojlbsfxc.html

[C04] 命名参数 / 关键字参数
来源：http://hz.guannengcc.top/gtqfagkurt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.tian-w.cn/gtvrmynwci.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.birdmap.top/gtmiefenmb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.wangdashe.top/gtkooppqyq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jlsjyb.cn/gtllmilxaa.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.hnqzz.top/gtvqjswtyx.html

Go:   // 无：用配置结构体参数
来源：http://hz.fzhhl.top/gtlxufyygc.html

Ruby: f(a: 1, b: 2)
来源：http://hz.sysykeji.top/gtagwbrdmc.html

C#:   f(a: 1, b: 2)
来源：http://hz.hysaishi.cn/gtpwzfxudj.html

[C05] 返回多个值
来源：http://hz.guowangkeji.top/gtooomcypz.html

Py:   return a, b
来源：http://hz.shanyushiyangtech.top/gtavjqmwrp.html

PHP:  return [$a, $b];
来源：http://hz.shangyingyoupin.top/gtzvilzfhj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.sxryk.cn/gtehynnshd.html

TS:   return { a, b };
来源：http://hz.shzxlz.cn/gtxkujxrvc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.daria6918.cn/gtljroowtt.html

Go:   return a, b
来源：http://hz.daria6918.cn/gtndfptrso.html

Ruby: return a, b
来源：http://hz.gzhubu.top/gtsajabvck.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jiagoushi.top/gtjitnljis.html

[C06] 匿名函数 / lambda
来源：http://hz.yangfankeji.com/gtcagwppvx.html

Py:   square = lambda x: x * x
来源：http://hz.sxryk.cn/gtyvmfiiaf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.chenjidiqi.icu/gtcpmmrkrq.html

JS:   const square = x => x * x;
来源：http://hz.tianlin.xyz/gtkjrcasea.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.dashuyun.cn/gtzbjeeycq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.xziqi.cn/gtsatnmygu.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yuanzhike.top/gtwjkkygwg.html

Ruby: square = ->(x) { x * x }
来源：http://hz.feifeiyinyue.top/gtlmpftstj.html


<!-- 参考信息 -->