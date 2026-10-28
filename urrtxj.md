代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.shuidangran.top/gtyrgxggiq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.gotoacloud.top/gtyvaslqfr.html

Go:   // 手写 map[string][]T
来源：http://hz.fzhhl.top/gtbxmjqmvp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hywenlv.cn/gtrobwcjmb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.fzhhl.top/gtyjqgfvfr.html

[D20] 统计每个元素出现次数
来源：http://hz.shuidangran.top/gtqjpmlwup.html

Py:   Counter(arr)
来源：http://hz.wangdashe.top/gtftkjigei.html

PHP:  array_count_values($arr);
来源：http://hz.gzhubu.top/gtqpwsqbhp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ybcxt.top/gtxvhkeufk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shzxlz.cn/gtjdjavgpk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.9152youxi.cn/gtdoexpmnq.html

Go:   // 手写 map[T]int
来源：http://hz.ydzc1.top/gtiqpdikln.html

Ruby: arr.tally
来源：http://hz.sufxvd.cn/gtziposhgf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhongyouzk.top/gtkedhjjaa.html

[D21] 判断是否包含某元素
来源：http://hz.wangdashe.top/gtsrlykvue.html

Py:   x in arr
来源：http://hz.jiagoushi.top/gtkgghtopd.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cucudq.cn/gtruphpwey.html

JS:   arr.includes(x)
来源：http://hz.andypj.xyz/gtogudyvmb.html

TS:   arr.includes(x)
来源：http://hz.gzhubu.top/gtfffoxupy.html

Java: list.contains(x)
来源：http://hz.smart0.xyz/gtisgbrsmi.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhoulong.xyz/gtodcsdtsj.html

Ruby: arr.include?(x)
来源：http://hz.ybcxt.top/gttnsxfobh.html

C#:   list.Contains(x)
来源：http://hz.zhixingplan.top/gtyihrfbwx.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shuidangran.top/gtmbrsqlky.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.redwolf501.top/gtvqqvphyh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.pycfn.com/gtnfixtzpi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jinyuanbaomall.cn/gtjucemgyc.html

TS:   [...arr];
来源：http://hz.ywan-chungtsiang.top/gtbiiwdspp.html

Java: new ArrayList<>(list);
来源：http://hz.ehwqpu.com/gtgmsksxds.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.havefunace.top/gtritsdrqa.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jinqigfzy.top/gtwhltfdag.html

C#:   new List<int>(list);
来源：http://hz.mhx1999.top/gtwcgfsija.html

[D23] reduce 累积计算
来源：http://hz.vqdsnc.cn/gtwqsrzuyv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.svipenyu.cn/gttiigyzsq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.daria6918.cn/gtnvnijyrz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.iojbl.cn/gtzbcumqav.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jqgufenzy.top/gtnoszkdel.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.ydjk.org.cn/gtklqhhqzt.html

Go:   // 手写循环
来源：http://hz.sweek.top/gtacnebvcg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jianghu66.top/gtlyhzrqbt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.tanke756.top/gtfqtykjxc.html

[D24] 字典 / Map 基本操作
来源：http://hz.bjfxy.top/gtzjoovpft.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hongshengwenyu.top/gtsatdbfnh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yj202588.top/gtaejiwfum.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.snrcjt.cn/gtzwiimvme.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hysaishi.cn/gtxlusisrf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hnqzz.top/gtrgzvezts.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.shanyushiyangtech.top/gtdoevjmjn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.sufxvd.cn/gtvtwhpddj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhiwuduotai.top/gtdlbnzhky.html

[D25] Set 集合去重与交并差
来源：http://hz.quarkkingdee.top/gtycegvrfh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhengqikj.top/gthstrussc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jiagoushi.top/gtinbylofo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.gotoacloud.top/gtvzmizkuh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.andypj.xyz/gtepxnwsqt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.kuanghao11.cn/gtyddusqmv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.mhx1999.top/gtplcrayat.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.aizwys.cn/gtkuyrmftg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yueranfly.top/gtzveqbsxn.html

[D26] 数组转字符串
来源：http://hz.sxryk.cn/gtyyzeteah.html

Py:   ", ".join(map(str, arr))
来源：http://hz.c1oappe.top/gtewcowvyn.html

PHP:  implode(", ", $arr);
来源：http://hz.birdmap.top/gtgxxeiuoj.html

JS:   arr.join(", ")
来源：http://hz.tanke756.top/gtgegfienc.html

TS:   arr.join(", ")
来源：http://hz.hnqzz.top/gtqskwxbar.html

Java: String.join(", ", list)
来源：http://hz.hywenlv.cn/gtirkhmefw.html

Go:   strings.Join(strs, ", ")
来源：http://hz.shzxlz.cn/gtwyixmrcw.html

Ruby: arr.join(", ")
来源：http://hz.dianchejie.cn/gtouhxsllp.html

C#:   string.Join(", ", list)
来源：http://hz.xingfuxueyuan.xyz/gtcmktcybr.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtlbrwfonv.html

E. 字符串处理
来源：http://hz.shzxlz.cn/gtllesjuul.html

================================================================================
来源：http://hz.jinqigufen.top/gtxjmsamgm.html

[E01] 拼接字符串
来源：http://hz.yongpay.top/gtndahqtkf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.redwolf501.top/gtfpgzpunc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.xylfe.cn/gtvrksyraw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.kuanghao11.cn/gthiibvntk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinqigfzy.top/gthxxbyhhe.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.sufxvd.cn/gtxrjftzxf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.ydjk.org.cn/gtpctarubo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yj20258.top/gtafkerzvo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hongshengwenyu.top/gtowxiohtf.html

[E02] 重复字符串
来源：http://hz.yvedp.cn/gtexpedzwu.html

Py:   "ab" * 3
来源：http://hz.tianlin.xyz/gtltwskbmp.html

PHP:  str_repeat("ab", 3);
来源：http://hz.shuidangran.top/gttcwyflkj.html

JS:   "ab".repeat(3)
来源：http://hz.shuidangran.top/gtdakqybmu.html

TS:   "ab".repeat(3)
来源：http://hz.yangfankeji.com/gthdjdzste.html

Java: "ab".repeat(3)
来源：http://hz.yueranfly.top/gtukxkeauf.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ywan-chungtsiang.top/gthswjrkyb.html

Ruby: "ab" * 3
来源：http://hz.zhoulong.xyz/gtqcdkqsak.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yanxiufei.cn/gtxzqjabbg.html

[E03] 截取子串
来源：http://hz.kuanghao11.cn/gtgrumtvuy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cheryme.top/gtmpqwwhsy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.nanxuanxn.top/gtznigseuc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.andypj.xyz/gtejcopczr.html

TS:   s.slice(1, 4)
来源：http://hz.yangfankeji.com/gtgrywgzcc.html

Java: s.substring(1, 4)
来源：http://hz.ppjwa.cn/gtomdlwmww.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ehwqpu.com/gtncdflmlw.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jqgfzy.top/gtnadzzbky.html

C#:   s.Substring(1, 3)
来源：http://hz.dashuyun.cn/gtscuwvbgi.html

[E04] 查找子串位置
来源：http://hz.andypj.xyz/gtzfohrfcr.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhijiandao.cn/gtuepgvxmy.html

PHP:  strpos($s, "x");
来源：http://hz.smart0.xyz/gtthlepsxf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.wangdashe.top/gtqqfnmuui.html

TS:   s.indexOf("x")
来源：http://hz.shanyushiyangtech.top/gtermnhztu.html

Java: s.indexOf("x")
来源：http://hz.yj202588.top/gtazxhcuqi.html

Go:   strings.Index(s, "x")
来源：http://hz.chenzaomai.com/gttmqkudia.html

Ruby: s.index("x")
来源：http://hz.zhongyouzk.top/gtubmujlwc.html

C#:   s.IndexOf("x")
来源：http://hz.jyoumei.cn/gtbbbnixsc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zhaomingkeji.xyz/gtjdccqrkh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.haohaochexian.top/gtxuzbsqjm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.sxryk.cn/gtbqnoztzn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.c1oappe.top/gtedrarsna.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.cheryme.top/gttskegboo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.c1oappe.top/gteftgfkec.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.fzhhl.top/gtuycdkvss.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xingfuxueyuan.xyz/gtcvpqntrr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hfpthk.cn/gtfrjdsbjj.html

[E06] 替换子串
来源：http://hz.snrcjt.cn/gtvhvalhze.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.snrcjt.cn/gtsovhksma.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.sweek.top/gthveuqbdd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.dashuyun.cn/gtdeafivlq.html

TS:   s.replaceAll("a", "b")
来源：http://hz.chenjidiqi.icu/gtazxdymti.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yonumen.top/gtidiqnjlb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yj20258888.top/gtsjpfepuu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.haohaochexian.top/gtzhhtxaky.html

C#:   s.Replace("a", "b")
来源：http://hz.jianghu66.top/gtoytcvqlq.html

[E07] 按分隔符拆分
来源：http://hz.sxryk.cn/gtbfhtyney.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zhixingplan.top/gthnicmafc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.tanke756.top/gtbwnhsedv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhixingplan.top/gtuzwayapa.html

TS:   s.split(",")
来源：http://hz.zhijiandao.cn/gtvttgnavw.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.ywan-chungtsiang.top/gtdiehnmgs.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ywan-chungtsiang.top/gtjdvrheoc.html

Ruby: s.split(",");  s.split
来源：http://hz.gotoacloud.top/gtjdnfjfln.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.meibo888.top/gtfkspkwwf.html

[E08] 数组按分隔符合并
来源：http://hz.cheryme.top/gtgorptegf.html

Py:   ",".join(items)
来源：http://hz.xuetiantiany.cn/gtzhcbwhza.html

PHP:  implode(",", $items);
来源：http://hz.svipenyu.cn/gtyctfmzie.html

JS:   items.join(",")
来源：http://hz.316326.xyz/gtrcddhucq.html

TS:   items.join(",")
来源：http://hz.ehwqpu.com/gtihwhirkz.html

Java: String.join(",", items)
来源：http://hz.yueranfly.top/gtpagrfdpq.html

Go:   strings.Join(items, ",")
来源：http://hz.wangshuangyany.cn/gtawnnbubh.html

Ruby: items.join(",")
来源：http://hz.yj20258.top/gtsnvliavp.html

C#:   string.Join(",", items)
来源：http://hz.jiagoushi.top/gtqbbnrtto.html

[E09] 去除所有空白字符
来源：http://hz.yj20258.top/gtkdqcewks.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yonumen.top/gtqtedvvrf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.meibo888.top/gtvyockksx.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jqgfzy.top/gtrmgidavv.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jyoumei.cn/gtqkhnrpev.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.ehwqpu.com/gtxcmrbeus.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yvedp.cn/gtqxlkvudr.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jqgufenzy.top/gtkvvxjrbv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.nanxuanxn.top/gtrogzqlaf.html

[E10] 左侧补零 / 定长填充
来源：http://hz.guowangkeji.top/gtwbwmomwf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hammf.cn/gtqtyqkjzy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.daria6918.cn/gtiwlilxds.html

JS:   "7".padStart(3, "0")
来源：http://hz.guowangkeji.top/gttyymuxec.html

TS:   "7".padStart(3, "0")
来源：http://hz.vqdsnc.cn/gtledlaggx.html

Java: String.format("%03d", 7)
来源：http://hz.meibo888.top/gtzdcfmlzv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.cucudq.cn/gttbcyifpt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhongyouzk.top/gtgrdbupbg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shangyingyoupin.top/gtwvwpqxvj.html

[E11] 反转字符串
来源：http://hz.jinqigfzy.top/gtmnxswqox.html

Py:   s[::-1]
来源：http://hz.sysykeji.top/gtlfysybgf.html

PHP:  strrev($s);
来源：http://hz.cheryme.top/gtmnjrdepw.html

JS:   [...s].reverse().join("")
来源：http://hz.guowangkeji.top/gtxiiohuze.html

TS:   [...s].reverse().join("")
来源：http://hz.ywan-chungtsiang.top/gtubmauqiz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.haohaochexian.top/gtyyrikevq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ivvv.top/gtlathoajb.html

Ruby: s.reverse
来源：http://hz.ppjwa.cn/gtsjzgwftt.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zycfv.cn/gtflewsbrp.html

[E12] 统计某字符出现次数
来源：http://hz.yanxiufei.cn/gtitnrrclq.html

Py:   s.count("a")
来源：http://hz.wangshuangyany.cn/gtddwwsqzl.html

PHP:  substr_count($s, "a");
来源：http://hz.zhoulong.xyz/gtcjqgjdpn.html

JS:   s.split("a").length - 1
来源：http://hz.zycfv.cn/gthzlooeqi.html

TS:   s.split("a").length - 1
来源：http://hz.hnqzz.top/gtozifqltg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.cheryme.top/gtaugjnuvb.html

Go:   strings.Count(s, "a")
来源：http://hz.jinqigufen.top/gtkwxdcrmr.html

Ruby: s.count("a")
来源：http://hz.sweek.top/gtkqdnajxn.html

C#:   s.Count(c => c == 'a')
来源：http://hz.gzhubu.top/gtiwfayydo.html

[E13] 逐字符遍历
来源：http://hz.yueranfly.top/gtfjwtiwfz.html

Py:   for ch in s: print(ch)
来源：http://hz.zhixingplan.top/gtiamlllsa.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.wangdashe.top/gtpoytuszw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hywenlv.cn/gtjuzszqld.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.pycfn.com/gthastwidg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shuidangran.top/gtxyaitxrr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cheryme.top/gtdigtbcuz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.0kj1m.cn/gtngicqkff.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.cucudq.cn/gtknpthuqo.html

[E14] URL 编码与 Base64
来源：http://hz.redwolf501.top/gtehyfgtns.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shanyushiyangkeji.top/gtwaujqesh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.xingfuxueyuan.xyz/gtobiemqgh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zycfv.cn/gtzjlbpqbz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.nwbrower.top/gtppwkhozs.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ehwqpu.com/gtqpknrjxj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.nwbrower.top/gtspmqgzct.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yuxming.cn/gtrsdxckoz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ehwqpu.com/gtltismlpo.html

[E15] HTML 转义 / 反转义
来源：http://hz.aibaodan.cn/gtbrvlhbdp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.sufxvd.cn/gtnptukapb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hfpthk.cn/gtaqiphisd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.shanyushiyangkeji.top/gtfeofrvhe.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.wangshuangyany.cn/gtrnvjxjcg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.daria6918.cn/gtnvdvmwov.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.0kj1m.cn/gtctgcashv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.guowangkeji.top/gtarxnpeiv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jinghuilouyu.cn/gtclovgtxl.html

[E16] 数字千分位
来源：http://hz.aizwys.cn/gtuvywipbf.html

Py:   f"{1234567:,}"
来源：http://hz.cheryme.top/gthapupgsu.html

PHP:  number_format(1234567);
来源：http://hz.shangyingyoupin.top/gtgwratgoj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ydzc1.top/gtepwulrff.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.wangshuangyany.cn/gtxuizmeny.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.tian-w.cn/gtbewtethi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.cdnleiting.top/gtxidafvsa.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.redwolf501.top/gteujkzibv.html

C#:   1234567.ToString("N0")
来源：http://hz.zycfv.cn/gtxywrcblj.html

[E17] 首字母大写
来源：http://hz.sweek.top/gttlfnkbit.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.ywan-chungtsiang.top/gtufavpyyo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.shuidangran.top/gtadhtyfez.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tianlin.xyz/gtaydrggrl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sufxvd.cn/gthfdxyxai.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.pycfn.com/gtbgorgzwa.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shuidangran.top/gttbfbysyh.html

Ruby: s.capitalize
来源：http://hz.chenzaomai.com/gtbbptxqcf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.tanke756.top/gtrraucacp.html

[E18] 模板占位符替换
来源：http://hz.yongpay.top/gtiwmomrup.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.birdmap.top/gtezjtnkux.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.shuidangran.top/gttuvbfeqv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenzaomai.com/gttzwsdkym.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jlsjyb.cn/gtetfolfxs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.snrcjt.cn/gtdhuakxzv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.sysykeji.top/gtvknebccp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhoulong.xyz/gtfeumpnhl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.chenzaomai.com/gtnsdhuizu.html

[E19] 多行文本按行拆分
来源：http://hz.yanxiufei.cn/gtktrhxpfs.html

Py:   s.splitlines()
来源：http://hz.yueranfly.top/gtscdivspd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.guannengcc.top/gtjhjdgbxz.html

JS:   s.split(/\r?\n/)
来源：http://hz.redwolf501.top/gtrxzceaaw.html

TS:   s.split(/\r?\n/)
来源：http://hz.pengpengdd.cyou/gtccswzzoy.html

Java: s.lines().toList()
来源：http://hz.chenjidiqi.icu/gtafgybezj.html

Go:   strings.Split(s, "\n")
来源：http://hz.tian-w.cn/gtybivcmcq.html

Ruby: s.lines
来源：http://hz.sxryk.cn/gtvskcsdjx.html

C#:   s.Split('\n')
来源：http://hz.cheryme.top/gthoxtknqd.html

[E20] 判断字符串是否为空
来源：http://hz.zhoulong.xyz/gtgxgggenu.html

Py:   if not s:
来源：http://hz.sxryk.cn/gtcsmbczyw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.feifeiyinyue.top/gtuxoynewo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ivvv.top/gtylbweuyf.html

TS:   if (s === "") {}
来源：http://hz.aizwys.cn/gthrpsbjlb.html

Java: if (s.isEmpty()) {}
来源：http://hz.gaohongyu789.top/gtxstfqepy.html

Go:   if s == "" {}
来源：http://hz.snrcjt.cn/gtsxqxmusr.html

Ruby: if s.empty?
来源：http://hz.fengsongda.top/gtmufbhqtq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hfpthk.cn/gtmhyumwck.html

[E21] 超长截断加省略号
来源：http://hz.cucudq.cn/gtcedtfcro.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhoulong.xyz/gtfrosofyf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhoulong.xyz/gthvrgkbmz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.aibaodan.cn/gtymslthuv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.havefunace.top/gtftyatkep.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.fengsongda.top/gtympymonq.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.cheryme.top/gtllcvfikf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hnxiangtu.top/gttpokbehx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.nanxuanxn.top/gtyrrhlqqr.html

[E22] 字节长度与字符长度
来源：http://hz.shanyushiyangtech.top/gtbojfrerl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.cheryme.top/gtqcmcjmcq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hnqzz.top/gtximvpsft.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ydzc1.top/gtvrovejfg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.chenlongwang.top/gtegkalobq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.wangshuangyany.cn/gtmcenyamb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ywan-chungtsiang.top/gtalxjvait.html

Ruby: s.bytesize;  s.length
来源：http://hz.redwolf501.top/gtpjdrvmrm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yj20258888.top/gthooicakj.html

================================================================================
来源：http://hz.dashuyun.cn/gtvqfzisgc.html

F. 文件与目录
来源：http://hz.aibaodan.cn/gttluoubra.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtwzpqhvmd.html

[F01] 读取整个文件
来源：http://hz.tanke756.top/gtotlmmstm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ydjk.org.cn/gtyuocjpjd.html

PHP:  file_get_contents("a.txt");
来源：http://hz.fengsongda.top/gtxxxuhees.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jiagoushi.top/gtztvvtduv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.tian-w.cn/gtmjuuqhsa.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.wangdashe.top/gtdscgjkmj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.pycfn.com/gtuvvacvof.html

Ruby: File.read("a.txt")
来源：http://hz.smart0.xyz/gtobwbcicw.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xuanzx.com/gtwpqhlyog.html

[F02] 逐行读取文件
来源：http://hz.yuanzhike.top/gttkfcrufl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.chenjidiqi.icu/gtzuymxdew.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hammf.cn/gtavcaahqf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.aibaodan.cn/gtwryexjin.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.guannengcc.top/gtjvoslxtq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.gotoacloud.top/gtoqytzpzo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.cashguo.top/gtofutpeqt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.shanyushiyangkeji.top/gtxmkafjlb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jlsjyb.cn/gtbghynghj.html

[F03] 写入文件（覆盖）
来源：http://hz.0kj1m.cn/gtlpuxlcls.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shanyushiyangtech.top/gtjopzylls.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.feifeiyinyue.top/gtftjetskt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhiwuduotai.top/gtgbxhkvll.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sysykeji.top/gtzoxoolnz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.pycfn.com/gtiwlcwmxb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.smart0.xyz/gtqzfnqmsp.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.mhx1999.top/gtafotawdp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jyoumei.cn/gtjfeyuegq.html

[F04] 追加写入文件
来源：http://hz.gzhubu.top/gtevmgsvlk.html


<!-- 参考信息 -->