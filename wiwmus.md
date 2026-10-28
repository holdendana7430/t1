代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.shzxlz.cn/gtdcrtdrcp.html

Go:   // 手写双层循环
来源：http://hz.jlsjyb.cn/gtcnvrvjxr.html

Ruby: nested.flatten
来源：http://hz.havefunace.top/gtclgalqye.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yj20258888.top/gtkxrbtrea.html

[D19] 按字段分组
来源：http://hz.jqgufenzy.top/gthboyryjv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hywenlv.cn/gtlczqlezr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.fzhhl.top/gtwopideoa.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yj20258.top/gtmazocjgb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.tianlin.xyz/gtiolgbpwy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhiwuduotai.top/gtynsqoqwo.html

Go:   // 手写 map[string][]T
来源：http://hz.ppjwa.cn/gtbbkejcbn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ydzc1.top/gtdiqisrwc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hammf.cn/gthwzwytbd.html

[D20] 统计每个元素出现次数
来源：http://hz.ydzc1.top/gtgtvcpnnd.html

Py:   Counter(arr)
来源：http://hz.svipenyu.cn/gtuxxfsndl.html

PHP:  array_count_values($arr);
来源：http://hz.jqgufenzy.top/gtiiruajly.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xingfuxueyuan.xyz/gtlclmbgkz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.dianchejie.cn/gtqavqejho.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.mhx1999.top/gtevmgbiqb.html

Go:   // 手写 map[T]int
来源：http://hz.ydzc1.top/gtinseqljn.html

Ruby: arr.tally
来源：http://hz.zhongyouzk.top/gtkcvhplzd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jqgfzy.top/gtmgtwwvcg.html

[D21] 判断是否包含某元素
来源：http://hz.meibo888.top/gtygqiyfba.html

Py:   x in arr
来源：http://hz.chenzaomai.com/gtypquyulv.html

PHP:  in_array($x, $arr, true);
来源：http://hz.nanxuanxn.top/gtqzbcyhsr.html

JS:   arr.includes(x)
来源：http://hz.xinyue.icu/gtqwxkjcjw.html

TS:   arr.includes(x)
来源：http://hz.yj20258888.top/gtdvdtikkx.html

Java: list.contains(x)
来源：http://hz.wangdashe.top/gtzhqhtwoo.html

Go:   slices.Contains(arr, x)
来源：http://hz.guowangkeji.top/gtloqzalyq.html

Ruby: arr.include?(x)
来源：http://hz.jinqigfzy.top/gtnvqucyox.html

C#:   list.Contains(x)
来源：http://hz.xinyue.icu/gthmtdqegu.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yuxming.cn/gtwinatlbh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ydzc1.top/gtthabbapg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yanxiufei.cn/gtkdlatdme.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zhiwuduotai.top/gtaanaigrm.html

TS:   [...arr];
来源：http://hz.yanxiufei.cn/gtmdnlrvlr.html

Java: new ArrayList<>(list);
来源：http://hz.zhiwuduotai.top/gtnvwgztxq.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.daria6918.cn/gthakjqbld.html

Ruby: arr.dup;  arr.clone
来源：http://hz.iojbl.cn/gtusvkrpuh.html

C#:   new List<int>(list);
来源：http://hz.cdnleiting.top/gtsfrkfcwh.html

[D23] reduce 累积计算
来源：http://hz.zycfv.cn/gtcncygstb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.chenlongwang.top/gtcayxdchl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhengqikj.top/gtupoqeggv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cashguo.top/gtmvtffkfy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ivvv.top/gtdsbzfbsj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.nwbrower.top/gtkkjvgoec.html

Go:   // 手写循环
来源：http://hz.cdnleiting.top/gtgkywrkjc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.sufxvd.cn/gthwpqshdr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.fengsongda.top/gtbfbvpyfq.html

[D24] 字典 / Map 基本操作
来源：http://hz.yj20258.top/gtsdesimza.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ehwqpu.com/gtzbujigxn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.feifeiyinyue.top/gtjguxgfdo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shzxlz.cn/gtdafnjuer.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jyoumei.cn/gtrxujwbnl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.havefunace.top/gtgkabqykn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.andypj.xyz/gthvbqxqvu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhoulong.xyz/gtpfatynun.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.iojbl.cn/gtxoiqporb.html

[D25] Set 集合去重与交并差
来源：http://hz.dashuyun.cn/gttiekpjbe.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.shangyingyoupin.top/gtedesgjgk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.tanke756.top/gtqplvcvrz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.xuanzx.com/gtudperskn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.nwbrower.top/gtafkzoxto.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zhengqikj.top/gtttgihjbc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.smart0.xyz/gtzmxlldxw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.shanyushiyangkeji.top/gtekjnvcqk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.tian-w.cn/gtpkhkuwal.html

[D26] 数组转字符串
来源：http://hz.yvedp.cn/gtyllpazmt.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yj20258888.top/gtlyfmxxip.html

PHP:  implode(", ", $arr);
来源：http://hz.shuidangran.top/gtkuxtwqgq.html

JS:   arr.join(", ")
来源：http://hz.52xcode.cn/gtbneozmtn.html

TS:   arr.join(", ")
来源：http://hz.jiagoushi.top/gtduufgmqr.html

Java: String.join(", ", list)
来源：http://hz.jinghuilouyu.cn/gtbivunwva.html

Go:   strings.Join(strs, ", ")
来源：http://hz.nanxinkj.top/gtkrvzpkdx.html

Ruby: arr.join(", ")
来源：http://hz.nwbrower.top/gtoadsxors.html

C#:   string.Join(", ", list)
来源：http://hz.zhongyouzk.top/gtxbokibtu.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtwjvbatzo.html

E. 字符串处理
来源：http://hz.sxryk.cn/gtbrhsgcbd.html

================================================================================
来源：http://hz.meibo888.top/gtscwznktw.html

[E01] 拼接字符串
来源：http://hz.jinghuilouyu.cn/gtiwshwfid.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.dianchejie.cn/gtydiexhti.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.svipenyu.cn/gtstlcgnrr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gotoacloud.top/gturgpsqcp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhijiandao.cn/gtkofyvnde.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.bjfxy.top/gtozpbsoau.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zdqjudy.top/gtmgnnqlfq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.kuanghao11.cn/gtdcsrgggx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhiwuduotai.top/gtwgwmobbs.html

[E02] 重复字符串
来源：http://hz.cheryme.top/gtxxfrvbzt.html

Py:   "ab" * 3
来源：http://hz.hongshengwenyu.top/gtpwouracd.html

PHP:  str_repeat("ab", 3);
来源：http://hz.shuidangran.top/gtfiwaxana.html

JS:   "ab".repeat(3)
来源：http://hz.jinyuanbaomall.cn/gtkgcmwydb.html

TS:   "ab".repeat(3)
来源：http://hz.yj20258888.top/gtrczgppza.html

Java: "ab".repeat(3)
来源：http://hz.yongpay.top/gtkmusxfrp.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.gaohongyu789.top/gtlulsknhi.html

Ruby: "ab" * 3
来源：http://hz.hammf.cn/gtpabwvzfk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zycfv.cn/gtaumzhlij.html

[E03] 截取子串
来源：http://hz.fzhhl.top/gtyphfdvoz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.daxiang520.top/gtcvpjhtwn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ppjwa.cn/gthrgetkej.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yonumen.top/gtxmydlwgi.html

TS:   s.slice(1, 4)
来源：http://hz.cqqwz.cn/gtlbenroem.html

Java: s.substring(1, 4)
来源：http://hz.hammf.cn/gtnlpowkqp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xuetiantiany.cn/gtfsshybny.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zycfv.cn/gtifdkcrjk.html

C#:   s.Substring(1, 3)
来源：http://hz.sysykeji.top/gtqtsqzsnu.html

[E04] 查找子串位置
来源：http://hz.yonumen.top/gtrgqguvqz.html

Py:   s.find("x");  s.index("x")
来源：http://hz.cqqwz.cn/gtrylfnyxo.html

PHP:  strpos($s, "x");
来源：http://hz.gzhubu.top/gtopjnwkkd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.snrcjt.cn/gtuczuciws.html

TS:   s.indexOf("x")
来源：http://hz.jyoumei.cn/gtgrcfvfup.html

Java: s.indexOf("x")
来源：http://hz.sxryk.cn/gtjtjgdhij.html

Go:   strings.Index(s, "x")
来源：http://hz.nanxinkj.top/gtpymcklyv.html

Ruby: s.index("x")
来源：http://hz.316326.xyz/gtzlcvsfwb.html

C#:   s.IndexOf("x")
来源：http://hz.yonumen.top/gtebykafrn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.mhx1999.top/gtbtndvaoa.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.nanxinkj.top/gtxqxrdcdg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.52xcode.cn/gtspfhpojf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinqigufen.top/gtpljbtngk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.cucudq.cn/gthpzicxaj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinghuilouyu.cn/gtasrojxsc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.9152youxi.cn/gtamsogckg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xinyue.icu/gtkxnqgbam.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.redwolf501.top/gtcrvbwdva.html

[E06] 替换子串
来源：http://hz.quarkkingdee.top/gtujusjzrb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.cheryme.top/gtnmjjocrq.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.dianchejie.cn/gtrmlqzurj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cheryme.top/gticbmcvxk.html

TS:   s.replaceAll("a", "b")
来源：http://hz.svipenyu.cn/gtsakjtbsj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shanyushiyangtech.top/gtawhtlxda.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.nanxinkj.top/gtgjxuyrsx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jinyuanbaomall.cn/gttmfsmyox.html

C#:   s.Replace("a", "b")
来源：http://hz.daria6918.cn/gtgephykvk.html

[E07] 按分隔符拆分
来源：http://hz.chenlongwang.top/gtdfdtqacp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.0kj1m.cn/gtmpzotkyq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jyoumei.cn/gtmrgcwbhc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.daxiang520.top/gtyvgomywh.html

TS:   s.split(",")
来源：http://hz.0kj1m.cn/gtyddbdrqb.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jlsjyb.cn/gtvrpgwfho.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.tian-w.cn/gtqcrkhwuu.html

Ruby: s.split(",");  s.split
来源：http://hz.yongpay.top/gtmgytmgpa.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.meibo888.top/gtiprlqfcc.html

[E08] 数组按分隔符合并
来源：http://hz.aizwys.cn/gtsqcjenvi.html

Py:   ",".join(items)
来源：http://hz.cucudq.cn/gthzxjvxxc.html

PHP:  implode(",", $items);
来源：http://hz.c1oappe.top/gtppruecai.html

JS:   items.join(",")
来源：http://hz.pycfn.com/gttplgepeb.html

TS:   items.join(",")
来源：http://hz.zhijiandao.cn/gtimeuikzx.html

Java: String.join(",", items)
来源：http://hz.zhijiandao.cn/gtwpcepkmm.html

Go:   strings.Join(items, ",")
来源：http://hz.shangyingyoupin.top/gtebnhpxtv.html

Ruby: items.join(",")
来源：http://hz.52xcode.cn/gtongrazfx.html

C#:   string.Join(",", items)
来源：http://hz.nwbrower.top/gtcdgqsyuv.html

[E09] 去除所有空白字符
来源：http://hz.jqgufenzy.top/gtwwmyucwn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.cashguo.top/gtvzsnoxco.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jlsjyb.cn/gtotgtlssd.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.cucudq.cn/gtfmalnpis.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.haohaochexian.top/gtrbnvfjbc.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.feifeiyinyue.top/gtjpdwrzzs.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zhoulong.xyz/gthnhewunw.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yuxming.cn/gtuwqmzkmc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yanxiufei.cn/gtpozfjaim.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jinyuanbaomall.cn/gtbwzdrndf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.dashuyun.cn/gtfqlhpzbq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.andypj.xyz/gtkspoknzk.html

JS:   "7".padStart(3, "0")
来源：http://hz.xylfe.cn/gtxioyjqtc.html

TS:   "7".padStart(3, "0")
来源：http://hz.shuidangran.top/gtljtnbvhd.html

Java: String.format("%03d", 7)
来源：http://hz.sysykeji.top/gthhonribi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.birdmap.top/gttdxdbpqx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.bjfxy.top/gtlyknswsh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zycfv.cn/gtjbgpzdqi.html

[E11] 反转字符串
来源：http://hz.ppjwa.cn/gttvqvpnkc.html

Py:   s[::-1]
来源：http://hz.nanxuanxn.top/gtmnqefvqi.html

PHP:  strrev($s);
来源：http://hz.yonumen.top/gtocgculmq.html

JS:   [...s].reverse().join("")
来源：http://hz.shanyushiyangtech.top/gtsptkhglg.html

TS:   [...s].reverse().join("")
来源：http://hz.xziqi.cn/gtifoqyuhy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.cashguo.top/gtfxssafcn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hysaishi.cn/gtuwmqahoa.html

Ruby: s.reverse
来源：http://hz.birdmap.top/gtksvgosmd.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.sxryk.cn/gtxhvdurdl.html

[E12] 统计某字符出现次数
来源：http://hz.hysaishi.cn/gtxrchuitg.html

Py:   s.count("a")
来源：http://hz.zhixingplan.top/gtmzozizee.html

PHP:  substr_count($s, "a");
来源：http://hz.chenzaomai.com/gtppvbfrwh.html

JS:   s.split("a").length - 1
来源：http://hz.iojbl.cn/gtewpmltwo.html

TS:   s.split("a").length - 1
来源：http://hz.jinqigfzy.top/gtqjugentw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.nwbrower.top/gtjtxbbaxe.html

Go:   strings.Count(s, "a")
来源：http://hz.hnqzz.top/gtfrtfeccd.html

Ruby: s.count("a")
来源：http://hz.wangshuangyany.cn/gtxbaxvsgq.html

C#:   s.Count(c => c == 'a')
来源：http://hz.bjfxy.top/gtdfmhddae.html

[E13] 逐字符遍历
来源：http://hz.yongpay.top/gtvqchlexr.html

Py:   for ch in s: print(ch)
来源：http://hz.zhiwuduotai.top/gtjouivtcp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cqqwz.cn/gthssmczlo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ydjk.org.cn/gtxvmhzktz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ywan-chungtsiang.top/gtfemplyje.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yueranfly.top/gtxjfeldhf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yuanzhike.top/gtqxuhxdix.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.c1oappe.top/gtjiawpygt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.haohaochexian.top/gtneepewgk.html

[E14] URL 编码与 Base64
来源：http://hz.jianghu66.top/gtblviwahp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ybcxt.top/gtsxpjfbde.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ybcxt.top/gtucjoympy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yanxiufei.cn/gterctywue.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.pycfn.com/gtwptmpyuo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.cqqwz.cn/gtmduwgkyk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.hammf.cn/gtscplfoci.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.quarkkingdee.top/gtyznmqnuk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.birdmap.top/gtfvpjmxbk.html

[E15] HTML 转义 / 反转义
来源：http://hz.daria6918.cn/gtedmixask.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xuetiantiany.cn/gtenxagosz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhixingplan.top/gtzxamuteb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.52xcode.cn/gtzqjqfoqh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jinghuilouyu.cn/gtdiqrffun.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yj20258888.top/gtbaaaockc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ydzc1.top/gthxevqhon.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.snrcjt.cn/gtcsmltztm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ivvv.top/gtloohriif.html

[E16] 数字千分位
来源：http://hz.tian-w.cn/gtyaluqufq.html

Py:   f"{1234567:,}"
来源：http://hz.ybcxt.top/gtcjahwywu.html

PHP:  number_format(1234567);
来源：http://hz.pengpengdd.cyou/gtnuqmdmlc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.tanke756.top/gtzqoesmnj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.shzxlz.cn/gtxvvivgxh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhixingplan.top/gtfeauhtoi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.daria6918.cn/gtfzclscdq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cdnleiting.top/gttykhfcwl.html

C#:   1234567.ToString("N0")
来源：http://hz.cheryme.top/gtgvlqwqsm.html

[E17] 首字母大写
来源：http://hz.jqgfzy.top/gtqcctmlly.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.sweek.top/gtrdjwgban.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.ydzc1.top/gtevjrtyhi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.aibaodan.cn/gtnuksikdo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.vqdsnc.cn/gtfxqcaref.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.wangdashe.top/gtsarquvaw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yangfankeji.com/gtaxsjpblc.html

Ruby: s.capitalize
来源：http://hz.sweek.top/gtdrpxjisb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhijiandao.cn/gtfmoivhqi.html

[E18] 模板占位符替换
来源：http://hz.nwbrower.top/gtcwdxkqov.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.guannengcc.top/gtspgapxuq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yueranfly.top/gtauvtpnvt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.dashuyun.cn/gtrtlmeget.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.kuanghao11.cn/gtizzqfrbz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.shanyushiyangkeji.top/gtstropiqf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jinqigufen.top/gtqmvfjhqn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jinghuilouyu.cn/gtiuybmsso.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.fengsongda.top/gtijvigair.html

[E19] 多行文本按行拆分
来源：http://hz.nanxuanxn.top/gtqjnxtlff.html

Py:   s.splitlines()
来源：http://hz.wangshuangyany.cn/gtpmwkmcag.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jlsjyb.cn/gtgqkycghw.html

JS:   s.split(/\r?\n/)
来源：http://hz.jinyuanbaomall.cn/gtycpjmqzd.html

TS:   s.split(/\r?\n/)
来源：http://hz.shzxlz.cn/gtntuebqog.html

Java: s.lines().toList()
来源：http://hz.tianlin.xyz/gtgtoswyes.html

Go:   strings.Split(s, "\n")
来源：http://hz.ivvv.top/gtwaabacax.html

Ruby: s.lines
来源：http://hz.9152youxi.cn/gtqmphjddx.html

C#:   s.Split('\n')
来源：http://hz.pengpengdd.cyou/gtzaoegalg.html

[E20] 判断字符串是否为空
来源：http://hz.daxiang520.top/gtfbskbgxe.html

Py:   if not s:
来源：http://hz.yueranfly.top/gtxrkxrmyu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhiwuduotai.top/gtjmlnsgdw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yongpay.top/gtyxrapcvg.html

TS:   if (s === "") {}
来源：http://hz.xziqi.cn/gtiyjmlfdu.html

Java: if (s.isEmpty()) {}
来源：http://hz.fzhhl.top/gtsxaanylg.html

Go:   if s == "" {}
来源：http://hz.ywan-chungtsiang.top/gtypuywwxb.html

Ruby: if s.empty?
来源：http://hz.yongpay.top/gthrdlcref.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.chenlongwang.top/gtjshscttf.html

[E21] 超长截断加省略号
来源：http://hz.birdmap.top/gtwgoriwcu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.xingfuxueyuan.xyz/gtkxecficc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zdqjudy.top/gtwpxzezox.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.chenzaomai.com/gtfdoieama.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tian-w.cn/gthbdxzash.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cucudq.cn/gtszmvaigr.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.9152youxi.cn/gtuqkosnks.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.xylfe.cn/gtkouxhymk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.smart0.xyz/gtcaveeudb.html

[E22] 字节长度与字符长度
来源：http://hz.ydzc1.top/gthpssrbrs.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.daria6918.cn/gtidtutlve.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.wangshuangyany.cn/gtlzzqxaje.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.svipenyu.cn/gtyuxsdxbm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sxryk.cn/gtkabjycyv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhengqikj.top/gtrlnehpxb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.cdnleiting.top/gtxojyszmz.html

Ruby: s.bytesize;  s.length
来源：http://hz.jianghu66.top/gtfcjcemke.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.gaohongyu789.top/gtrkvdivai.html

================================================================================
来源：http://hz.meibo888.top/gttysyrejp.html

F. 文件与目录
来源：http://hz.feifeiyinyue.top/gtefidrgvc.html

================================================================================
来源：http://hz.sweek.top/gtinypctry.html

[F01] 读取整个文件
来源：http://hz.jlsjyb.cn/gtdbuxdthi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ivvv.top/gttesjmwnb.html

PHP:  file_get_contents("a.txt");
来源：http://hz.dianchejie.cn/gtxkgftwsx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.vqdsnc.cn/gtutjneepu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.sweek.top/gtcjcolqrk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yongpay.top/gtonalhorb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yuxming.cn/gtnelezgbj.html

Ruby: File.read("a.txt")
来源：http://hz.zhoulong.xyz/gtpqvnefiw.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yanxiufei.cn/gtguryiyda.html

[F02] 逐行读取文件
来源：http://hz.shzxlz.cn/gtxmvelnbp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.guowangkeji.top/gthxgpgsfs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xingfuxueyuan.xyz/gtfsxjqzes.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hfpthk.cn/gtuxkwbyyo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cheryme.top/gtermkjmrk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.nanxinkj.top/gtthevhbpr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhengqikj.top/gtdrjjipul.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hywenlv.cn/gtbrpzicsd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.tianlin.xyz/gtlutbkiuq.html

[F03] 写入文件（覆盖）
来源：http://hz.hnqzz.top/gtnjgxcuza.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.sxryk.cn/gtffnolfss.html


<!-- 参考信息 -->