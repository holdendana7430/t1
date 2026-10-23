代发 wailian999

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3bblaakia.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ntykydre.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3akcjulrd.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3sgocgoyy.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3bcmscmdt.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3qeodkpwk.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3xzmsuokr.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3risnpnmu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3qnrwndam.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3vgeojjyk.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3hghuhpig.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3vcadimeh.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3exhlmzus.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3vwspvipe.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3calsmbve.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3dujcdwgu.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3mvicgwhr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3dmgtalsm.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vtopywtf.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3lpthvfud.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xivqzznt.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3tgmvcmdu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ibixftlc.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3xfaxuwob.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pidzsorm.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bhkzkmvg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3yhzjztvf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3mwunyqlx.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3qweonvzk.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jtupmsyq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uwvzfegy.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3exifldxi.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3dtgqqejl.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xvhctzwo.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3caetlyzr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3cgwdegrh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3fcbztxex.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ljphhoax.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3twedomqo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cxnrgves.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ojtyjhwk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3aficdked.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3nlmkxsjf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ovnyfldi.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3vfjujxav.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3lsbbozim.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3zuvkirxr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3euflzkum.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3lrgwyevd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3vuxzictb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3hfgeybpq.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ubkrnyee.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3yifzvnrg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3punavzxv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zzweweum.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mtosxort.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ajkbixjw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3nunvvzqr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3fvtxnfcm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3frxyqejb.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3bgttghah.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3mvftlmpd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3opyfrfzb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3vurbcsjm.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3szobbgkm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3txjntlta.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3jmjvrzzf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qdmcweye.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ookzwfzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tmertenx.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3osapvkrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jifftjnz.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3vzlxwyoo.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3krfugznp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmatmqwd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vtvsxehg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ksdgmmsr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3visboatf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3yiqlzpgw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3pqonvkuy.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3fnpggklw.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3dhisjuqy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3khwuirum.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmwkkplv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vsgireyr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jgicbicd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xrmiacrn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3krfdcmya.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3yarsknfs.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lixrwkyf.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3yafdfmdu.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3qzkxkjlv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3guzeonip.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3thfuzeja.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3oxivrniq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwprviyo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3tsjnsvtq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3knqguakt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3zjgjcned.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3dsmhccbg.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3zrfifhca.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3saxtkmde.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3greyahce.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3sezmvvjn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3luuihsew.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3dartzhlv.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3cismyiwo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3lbpwxcaw.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3qxotrofb.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3dwhmlgml.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhhkxotw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wlfusdtx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3mqzuqdcn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3avrjsctn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ottwgabp.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3dywmfgte.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3viurkmqf.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3bfwpgssm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3igwrszxk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3wogqilma.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3mtjnyovp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ewdxymbt.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3lebutujk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3zlkhlmse.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3wypxbxqe.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3xoskepys.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3fezfrxos.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3dbyjvhdd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3cpggtvgd.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cqiyfums.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qshgtfyu.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwcxltgb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3ufyqeopv.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3vlcgtlzm.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ibdxsofb.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ocnulbbd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3vsmdosno.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yeytnklt.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lvmrytam.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3efbnjayc.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vzzzvoum.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3gyoyigou.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ipjqgjxe.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ucybnmoc.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ciivrvra.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3xucgzuuz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsunztpk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3onfcsodn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3igkzfniv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mazvruyi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3vsyysszq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3bfqiiynu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3agjgyiwf.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3lmnwhteu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3bqcvnpgx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3vopdtmjg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3beiwzite.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3czddoivc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqppjobq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3esluaxri.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3iuxriaty.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3dseqjztp.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3pmppotir.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3erzqxwkw.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3effqlgpm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xqusbfrt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3aqcrdzkz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3lspiqtmb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3zwmarykg.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3wahqlhcd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3wotnrtex.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3kjmzezei.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3hjysphuo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3cnaktidg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rtlhzwsq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3gzaputod.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bxrrexgp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3fuximbgo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3funktreb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3wlbtsjjh.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3nartbkdu.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3kwjhyyux.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3fskitopi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ufdpodwi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yghmzmah.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3hnihohmo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ififxtfj.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3phdkdlda.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3vpujuhfw.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3dfvoiazj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3qmklsubi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3kpfpvpeu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gobomctt.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ktnwwkkf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wibaxggn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3buesqefb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3hfespgfa.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3snoypddv.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3nusbtxbn.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ntoxhntq.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3nxezuhde.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jbbbwbvj.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tjykeipl.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tirgonwl.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rrwgnsbk.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bjchrtqk.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pmfauxpp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3jixredgw.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3mxzjhbft.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3hbyqkisp.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ecvussuj.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jjwxxcjr.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3iuxbqmyo.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3jwzfqhen.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3gwccpjiu.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kzfnucsm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tqfveigk.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3qqlqusnp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wilgzxeo.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3exuqzfed.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kccezilo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ulchzreo.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmglowbk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kuddnpcz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hztyytpx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3dmkbbnxx.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3zqucilsq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mmolyoff.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3cdxjxusp.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3txsaivkp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ihzllkon.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmtpnrra.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ergbmnja.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3xyqjveqa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3rvljrxab.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3lysxraky.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3yfnsfunr.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3gsddokgv.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ktyfabtu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3njdifwte.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ayodavpr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3wetzjzqy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3rxqihwbc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3qlzmsuzw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3agicikjl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3gxbnjedp.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3fbtzdtls.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3qwxtvkfm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ccysekbb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3wgqchngy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3uvidsayo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3qovtdgdl.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3knijfyee.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3upneqtsu.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3aptiryqm.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3yxsbhcea.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3blqxpmfd.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3izhxiatv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3esbakbwo.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3tmhhoziw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3pyfikect.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3udviummn.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3skvlnacd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ebgjztdq.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3qmghvdsu.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3tabmpliz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3rbheoonu.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ltmrbnhg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tmdqzchf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tecpqeuy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3ihmlwjnb.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3gjskqrbn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ihxsrbqc.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3mpbfitka.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3cikptmjd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3pqdaojxt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3drcwhjzl.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3rmucqndl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qndzodco.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3jozbcnvh.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3utzmccih.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3kchdnvtx.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3cwctycnz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ibczkhpe.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3xoggzdbf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnkbmqty.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gidphyxy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3cfuylaai.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ipvbyduy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3xuzuolkm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pfqjajfi.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3livavnxw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tqwvzein.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3bwfeiifg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3hqseorrm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3xqodhgif.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ncnehgke.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3qxnzqtvm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3jjxkkrbq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3vsjnjxht.html


<!-- 参考信息 -->