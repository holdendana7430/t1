代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.gzhubu.top/gtyrnownhv.html

Go:   // 手写双层循环
来源：http://hz.xinyue.icu/gtudovvbqi.html

Ruby: nested.flatten
来源：http://hz.zhongyouzk.top/gtesnvhwbv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.aibaodan.cn/gthcfnxfii.html

[D19] 按字段分组
来源：http://hz.cheryme.top/gtcgjkomix.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.iojbl.cn/gtspavcfjl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.quarkkingdee.top/gtnoqydzpy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.shanyushiyangtech.top/gtvehslofv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.iojbl.cn/gtjsnqdyef.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.hnxiangtu.top/gtujnxyyaf.html

Go:   // 手写 map[string][]T
来源：http://hz.guowangkeji.top/gtsadtifau.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.wangshuangyany.cn/gtdpyehsvz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.daxiang520.top/gttetqjiqm.html

[D20] 统计每个元素出现次数
来源：http://hz.jyoumei.cn/gtwhbwmznn.html

Py:   Counter(arr)
来源：http://hz.haohaochexian.top/gtydtovxyl.html

PHP:  array_count_values($arr);
来源：http://hz.daria6918.cn/gtglrhvfef.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xylfe.cn/gtugstclor.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinqigufen.top/gtoaewqiff.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.xuanzx.com/gtwlylswvz.html

Go:   // 手写 map[T]int
来源：http://hz.nanxuanxn.top/gtycolshdu.html

Ruby: arr.tally
来源：http://hz.jyoumei.cn/gtpjvwcxut.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ybcxt.top/gtvdgjrukj.html

[D21] 判断是否包含某元素
来源：http://hz.cqqwz.cn/gtxkxsiydg.html

Py:   x in arr
来源：http://hz.dashuyun.cn/gtkoefitdx.html

PHP:  in_array($x, $arr, true);
来源：http://hz.tanke756.top/gtsxmdxgtr.html

JS:   arr.includes(x)
来源：http://hz.yj20258888.top/gtfptsbwfr.html

TS:   arr.includes(x)
来源：http://hz.gotoacloud.top/gtqrlyidbj.html

Java: list.contains(x)
来源：http://hz.chenzaomai.com/gttpynzxcy.html

Go:   slices.Contains(arr, x)
来源：http://hz.tian-w.cn/gtdpibbscz.html

Ruby: arr.include?(x)
来源：http://hz.shangyingyoupin.top/gtwfzmpahs.html

C#:   list.Contains(x)
来源：http://hz.jinyuanbaomall.cn/gtkypgsenn.html

[D22] 复制数组（避免共享引用）
来源：http://hz.quarkkingdee.top/gtrqyvfmyt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ydzc1.top/gtqdlipknz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zhixingplan.top/gthxrlxwdf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ywan-chungtsiang.top/gtgujkdgvd.html

TS:   [...arr];
来源：http://hz.kuanghao11.cn/gtoifwwxur.html

Java: new ArrayList<>(list);
来源：http://hz.chenzaomai.com/gtgabjsdpz.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.gaohongyu789.top/gtqwmrbzao.html

Ruby: arr.dup;  arr.clone
来源：http://hz.gogol.net.cn/gtebwgtwni.html

C#:   new List<int>(list);
来源：http://hz.jinqigufen.top/gtzkvxfpeq.html

[D23] reduce 累积计算
来源：http://hz.ppjwa.cn/gttkltuhsx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.daria6918.cn/gtlydxjadi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.pycfn.com/gtuzflsymf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yuanzhike.top/gtonyqnbmv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yj20258888.top/gtkummnnii.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.sxryk.cn/gtkhtawnpg.html

Go:   // 手写循环
来源：http://hz.hysaishi.cn/gtfjwbugzm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.fzhhl.top/gtqjcnsbjb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.havefunace.top/gtvxaopnhk.html

[D24] 字典 / Map 基本操作
来源：http://hz.tanke756.top/gtkhocjyfd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jinyuanbaomall.cn/gtxwjkkzar.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.dianchejie.cn/gtqbqrwllc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.0kj1m.cn/gtyvzhbujk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.quarkkingdee.top/gttaatctqv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.sufxvd.cn/gtjrqveglf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ppjwa.cn/gtultvsojb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jinyuanbaomall.cn/gtypymlkyl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jinghuilouyu.cn/gtnaoynkdv.html

[D25] Set 集合去重与交并差
来源：http://hz.yangfankeji.com/gtsjblfzbb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hysaishi.cn/gtxrcunamt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zhixingplan.top/gtvnlfwdrj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yonumen.top/gthfiiophp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.snrcjt.cn/gteormpfqe.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yuanzhike.top/gtlrmbmqef.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yj202588.top/gtztvpnmgq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.gaohongyu789.top/gtrsgzpiob.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.ydzc1.top/gtoxqcpzxa.html

[D26] 数组转字符串
来源：http://hz.yueranfly.top/gttkookzmh.html

Py:   ", ".join(map(str, arr))
来源：http://hz.cashguo.top/gtluudexge.html

PHP:  implode(", ", $arr);
来源：http://hz.shanyushiyangkeji.top/gtztzbqqmc.html

JS:   arr.join(", ")
来源：http://hz.yuanzhike.top/gtrsmfkjyv.html

TS:   arr.join(", ")
来源：http://hz.yj202588.top/gtyqwijohh.html

Java: String.join(", ", list)
来源：http://hz.birdmap.top/gtwaauccxe.html

Go:   strings.Join(strs, ", ")
来源：http://hz.daria6918.cn/gthdgtudnm.html

Ruby: arr.join(", ")
来源：http://hz.cheryme.top/gtvwtxyrme.html

C#:   string.Join(", ", list)
来源：http://hz.yj20258.top/gtvyqgwswn.html

================================================================================
来源：http://hz.chenlongwang.top/gtxcdyzsfc.html

E. 字符串处理
来源：http://hz.svipenyu.cn/gtvxoiosqs.html

================================================================================
来源：http://hz.quarkkingdee.top/gtdzkppnhs.html

[E01] 拼接字符串
来源：http://hz.jlsjyb.cn/gtxwstjbkj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yonumen.top/gtuqvnwipe.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhaomingkeji.xyz/gtbfqjheoh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.aizwys.cn/gtivnkfcye.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nwbrower.top/gtbxkbectm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ywan-chungtsiang.top/gtcetknljx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yj20258.top/gtngbjxlno.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.snrcjt.cn/gtztypdqpr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.snrcjt.cn/gtypnlqzhr.html

[E02] 重复字符串
来源：http://hz.316326.xyz/gthcyyctwd.html

Py:   "ab" * 3
来源：http://hz.yangfankeji.com/gtbrgjysmn.html

PHP:  str_repeat("ab", 3);
来源：http://hz.0kj1m.cn/gthokfckjn.html

JS:   "ab".repeat(3)
来源：http://hz.52xcode.cn/gtktcqylvv.html

TS:   "ab".repeat(3)
来源：http://hz.ppjwa.cn/gtzmwwfkfq.html

Java: "ab".repeat(3)
来源：http://hz.c1oappe.top/gthqrbfpna.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.pengpengdd.cyou/gtrpsnnror.html

Ruby: "ab" * 3
来源：http://hz.meibo888.top/gtuuztsatj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.shanyushiyangkeji.top/gtrrhhwqsw.html

[E03] 截取子串
来源：http://hz.wangdashe.top/gtihnliivf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zhijiandao.cn/gtlxsotfir.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xuetiantiany.cn/gtjwqdoozf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhoulong.xyz/gtzftjhftc.html

TS:   s.slice(1, 4)
来源：http://hz.zhixingplan.top/gtdyagyosz.html

Java: s.substring(1, 4)
来源：http://hz.zhijiandao.cn/gtxjlwlwev.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.cucudq.cn/gtiuhqxtci.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zhongyouzk.top/gtdjyefdep.html

C#:   s.Substring(1, 3)
来源：http://hz.ywan-chungtsiang.top/gtdraayqqc.html

[E04] 查找子串位置
来源：http://hz.zhongyouzk.top/gtsovfwbna.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jinqigfzy.top/gtzkipjttz.html

PHP:  strpos($s, "x");
来源：http://hz.fengsongda.top/gtqwqeqrcv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.dianchejie.cn/gtleteiujd.html

TS:   s.indexOf("x")
来源：http://hz.tianlin.xyz/gtaumqsmaj.html

Java: s.indexOf("x")
来源：http://hz.cashguo.top/gtzlaxvdbu.html

Go:   strings.Index(s, "x")
来源：http://hz.kuanghao11.cn/gtrclbdksw.html

Ruby: s.index("x")
来源：http://hz.jqgfzy.top/gtonargbyr.html

C#:   s.IndexOf("x")
来源：http://hz.sysykeji.top/gtxqgfbwua.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.wangdashe.top/gtvrchgvpi.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.gaohongyu789.top/gtsswvzjii.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jyoumei.cn/gtxxaqppou.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.tanke756.top/gtmcnriuaa.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.sxryk.cn/gtzcbcqneu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.9152youxi.cn/gtthidwsmr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jinyuanbaomall.cn/gtdpghllpd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.fzhhl.top/gtybxujeuf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.cdnleiting.top/gtmhmyxmxp.html

[E06] 替换子串
来源：http://hz.c1oappe.top/gtcxfepnkt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.chenlongwang.top/gtzblzxjua.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jiagoushi.top/gtcwbvgcyk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xuetiantiany.cn/gtlripyfbi.html

TS:   s.replaceAll("a", "b")
来源：http://hz.shuidangran.top/gtksxvnybw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.tanke756.top/gtsezcenrh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.shzxlz.cn/gtimvaqcjm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yongpay.top/gtlljmsqpd.html

C#:   s.Replace("a", "b")
来源：http://hz.hnqzz.top/gtapbsjvjl.html

[E07] 按分隔符拆分
来源：http://hz.shangyingyoupin.top/gtqtfcitqb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ppjwa.cn/gtdfjzbplw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ydjk.org.cn/gtwngiwwhn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.hywenlv.cn/gtnogdvtoh.html

TS:   s.split(",")
来源：http://hz.redwolf501.top/gttwdtvvky.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.andypj.xyz/gtzglrvvbb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.aizwys.cn/gtrivcyuuy.html

Ruby: s.split(",");  s.split
来源：http://hz.gzhubu.top/gtssftlpat.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.9152youxi.cn/gthbsqpdtv.html

[E08] 数组按分隔符合并
来源：http://hz.gzhubu.top/gtdfdfujxq.html

Py:   ",".join(items)
来源：http://hz.jinqigufen.top/gtjveykxsg.html

PHP:  implode(",", $items);
来源：http://hz.andypj.xyz/gtvzykictc.html

JS:   items.join(",")
来源：http://hz.shzxlz.cn/gtvzxztrda.html

TS:   items.join(",")
来源：http://hz.fzhhl.top/gtwghouhff.html

Java: String.join(",", items)
来源：http://hz.chenzaomai.com/gtyeeyuumh.html

Go:   strings.Join(items, ",")
来源：http://hz.nanxinkj.top/gtlxfciqep.html

Ruby: items.join(",")
来源：http://hz.sweek.top/gtkhcecusp.html

C#:   string.Join(",", items)
来源：http://hz.tianlin.xyz/gtyjpqrxeh.html

[E09] 去除所有空白字符
来源：http://hz.sysykeji.top/gtgfzjoqzv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.cashguo.top/gthyjbmpwi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.gaohongyu789.top/gtczemyego.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.wangdashe.top/gtffztchzk.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.haohaochexian.top/gtrwugdbzk.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.daxiang520.top/gtbsbssziq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jlsjyb.cn/gtyfxpiqii.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shangyingyoupin.top/gtdzfffpcf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhixingplan.top/gtqlzjqmdw.html

[E10] 左侧补零 / 定长填充
来源：http://hz.gaohongyu789.top/gtnteufimo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.haohaochexian.top/gtlwpcenbo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yvedp.cn/gtlxwgnhtu.html

JS:   "7".padStart(3, "0")
来源：http://hz.cdnleiting.top/gthorwlbjr.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhoulong.xyz/gtijmyzswo.html

Java: String.format("%03d", 7)
来源：http://hz.ywan-chungtsiang.top/gtjvsscnbb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.redwolf501.top/gtrhdlsfsb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.nwbrower.top/gtjkaycilv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.chenlongwang.top/gtwukasyvx.html

[E11] 反转字符串
来源：http://hz.jqgfzy.top/gttuumvabt.html

Py:   s[::-1]
来源：http://hz.smart0.xyz/gtpiljzrza.html

PHP:  strrev($s);
来源：http://hz.cucudq.cn/gtygsfhgpj.html

JS:   [...s].reverse().join("")
来源：http://hz.hnxiangtu.top/gtoplgovbq.html

TS:   [...s].reverse().join("")
来源：http://hz.quarkkingdee.top/gtotpqeazc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.0kj1m.cn/gttdsqystg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yanxiufei.cn/gtrdyhtfjt.html

Ruby: s.reverse
来源：http://hz.cdnleiting.top/gtkhqlemge.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hywenlv.cn/gtpyixcdok.html

[E12] 统计某字符出现次数
来源：http://hz.bjfxy.top/gtwuzkyrli.html

Py:   s.count("a")
来源：http://hz.shanyushiyangtech.top/gtaognungk.html

PHP:  substr_count($s, "a");
来源：http://hz.xinyue.icu/gtsdywcluo.html

JS:   s.split("a").length - 1
来源：http://hz.ivvv.top/gtaoslxhfi.html

TS:   s.split("a").length - 1
来源：http://hz.daxiang520.top/gtkjhziimh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.shzxlz.cn/gtrubpmjhj.html

Go:   strings.Count(s, "a")
来源：http://hz.bjfxy.top/gtmrlsibwl.html

Ruby: s.count("a")
来源：http://hz.hysaishi.cn/gtyyrpivbt.html

C#:   s.Count(c => c == 'a')
来源：http://hz.hammf.cn/gthcfplogw.html

[E13] 逐字符遍历
来源：http://hz.andypj.xyz/gtivrlqkau.html

Py:   for ch in s: print(ch)
来源：http://hz.ppjwa.cn/gtwspkktmk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cashguo.top/gtgolmlxlk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.chenzaomai.com/gtfpryrujc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yangfankeji.com/gtlwrlcsdw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.redwolf501.top/gtnxudynqd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zdqjudy.top/gtqapuxjyt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jyoumei.cn/gteclzhdjr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yonumen.top/gtqdrenhsf.html

[E14] URL 编码与 Base64
来源：http://hz.gzhubu.top/gtnzztopbn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yangfankeji.com/gtsnwkpduv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhengqikj.top/gtpphrkeco.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yj20258.top/gtprxhhwdi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.nwbrower.top/gtjjhoiynh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jlsjyb.cn/gtxnjkcytv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.sweek.top/gtjtxgjxcn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hnxiangtu.top/gtpzuycane.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.birdmap.top/gtoolulytj.html

[E15] HTML 转义 / 反转义
来源：http://hz.feifeiyinyue.top/gtjepdkrsq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yuxming.cn/gtazeqxrin.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yongpay.top/gtwuthinby.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.daria6918.cn/gtqpfvvpuy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yj20258888.top/gtvxaynjhh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jqgufenzy.top/gtidozngij.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.chenlongwang.top/gtdhmouqdh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jqgufenzy.top/gtekiolvit.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.52xcode.cn/gtjcrnsuws.html

[E16] 数字千分位
来源：http://hz.jinyuanbaomall.cn/gtbjkxlfas.html

Py:   f"{1234567:,}"
来源：http://hz.nanxinkj.top/gtrebrcyug.html

PHP:  number_format(1234567);
来源：http://hz.gogol.net.cn/gthomtheca.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.pengpengdd.cyou/gtxjxlwqct.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.cqqwz.cn/gttmzovlek.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yongpay.top/gtplrrzgwy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ybcxt.top/gtvvmsfqen.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.shangyingyoupin.top/gtxwmoueus.html

C#:   1234567.ToString("N0")
来源：http://hz.52xcode.cn/gtnqpcdrnq.html

[E17] 首字母大写
来源：http://hz.yangfankeji.com/gtsuetzgsb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.cdnleiting.top/gtujllkwxd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.tianlin.xyz/gtzzvcphzp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tian-w.cn/gtyjcifcqv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.fengsongda.top/gtnekysiou.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.sysykeji.top/gtdcttkzqt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.aibaodan.cn/gtyomqntpw.html

Ruby: s.capitalize
来源：http://hz.ydzc1.top/gtrctcwvbz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.hongshengwenyu.top/gtrrbzkvkw.html

[E18] 模板占位符替换
来源：http://hz.yanxiufei.cn/gtcywodyle.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.dashuyun.cn/gtpuyulefc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.sysykeji.top/gtytdptemv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinyuanbaomall.cn/gtczolhvlj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jyoumei.cn/gtdiyurgma.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.daria6918.cn/gteirodgdm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ywan-chungtsiang.top/gtrxjigcep.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yuanzhike.top/gtgqqfonlv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ehwqpu.com/gtdtxmnjvz.html

[E19] 多行文本按行拆分
来源：http://hz.nanxuanxn.top/gtbmfqmnjj.html

Py:   s.splitlines()
来源：http://hz.daria6918.cn/gtwdayawai.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hfpthk.cn/gtsvpgmvmj.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhongyouzk.top/gtuxznmwmt.html

TS:   s.split(/\r?\n/)
来源：http://hz.ivvv.top/gtcyhfwwre.html

Java: s.lines().toList()
来源：http://hz.dashuyun.cn/gtbrvcwobu.html

Go:   strings.Split(s, "\n")
来源：http://hz.bjfxy.top/gtpszjvpfc.html

Ruby: s.lines
来源：http://hz.yueranfly.top/gtskivivzf.html

C#:   s.Split('\n')
来源：http://hz.c1oappe.top/gtaoeztfts.html

[E20] 判断字符串是否为空
来源：http://hz.hywenlv.cn/gtsehuxycn.html

Py:   if not s:
来源：http://hz.cheryme.top/gtbbnydnei.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.aibaodan.cn/gtexikqega.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.tanke756.top/gtrxsrbnsk.html

TS:   if (s === "") {}
来源：http://hz.ehwqpu.com/gtusxnpvwa.html

Java: if (s.isEmpty()) {}
来源：http://hz.svipenyu.cn/gtsgqxewdt.html

Go:   if s == "" {}
来源：http://hz.shanyushiyangkeji.top/gtcyqhirhy.html

Ruby: if s.empty?
来源：http://hz.zdqjudy.top/gtwffhdwuw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.tanke756.top/gtdspzclhg.html

[E21] 超长截断加省略号
来源：http://hz.jqgfzy.top/gtyqdoymaw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yuanzhike.top/gtacouglul.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.quarkkingdee.top/gtjgsmtzsi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.quarkkingdee.top/gtgzqdudit.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.haohaochexian.top/gtrufywgbn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhoulong.xyz/gttpuplens.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.bjfxy.top/gtbdzehymv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ivvv.top/gttsrnkfoe.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.nwbrower.top/gtohxptrqd.html

[E22] 字节长度与字符长度
来源：http://hz.dianchejie.cn/gtacpoehjc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhengqikj.top/gtwdzpqhiw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenlongwang.top/gtuyzwjnpw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhijiandao.cn/gtufhhclrr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ywan-chungtsiang.top/gtuxtkwzgb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.cqqwz.cn/gtadziooab.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jlsjyb.cn/gtdvhyizkn.html

Ruby: s.bytesize;  s.length
来源：http://hz.kuanghao11.cn/gtbyifmfuq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.andypj.xyz/gtiybrtzvy.html

================================================================================
来源：http://hz.dashuyun.cn/gtqdxemnys.html

F. 文件与目录
来源：http://hz.jqgufenzy.top/gtvfmgbgpj.html

================================================================================
来源：http://hz.yuanzhike.top/gtlucyrfzd.html

[F01] 读取整个文件
来源：http://hz.dianchejie.cn/gtmcpafotb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ybcxt.top/gtrvojrwzl.html

PHP:  file_get_contents("a.txt");
来源：http://hz.nanxinkj.top/gtzfcavbdg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gogol.net.cn/gtfravvaru.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.sysykeji.top/gthjrbjuux.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xylfe.cn/gticzotyxy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.ehwqpu.com/gtyiogcpwm.html

Ruby: File.read("a.txt")
来源：http://hz.ydzc1.top/gtnpxgnwep.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jinqigfzy.top/gtkfrxcxtt.html

[F02] 逐行读取文件
来源：http://hz.zhiwuduotai.top/gtxoahzvba.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.vqdsnc.cn/gtwnfkqxua.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.sxryk.cn/gteakqkhtt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yueranfly.top/gtqbkozknn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.dashuyun.cn/gtfbyehtkg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.iojbl.cn/gtdnlefchb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.aizwys.cn/gthzymxmce.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jinghuilouyu.cn/gtozblhyrf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.daxiang520.top/gtpfvpyrha.html

[F03] 写入文件（覆盖）
来源：http://hz.jinghuilouyu.cn/gtoatzdydd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.fzhhl.top/gtespmjrmr.html


<!-- 参考信息 -->