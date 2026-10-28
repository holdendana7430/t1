代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhongyouzk.top/gtctiqedrx.html

PHP:  array_merge(...$nested);
来源：http://hz.wangshuangyany.cn/gtxvadqqst.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.pycfn.com/gtbnwrczdb.html

TS:   nested.flat();
来源：http://hz.tianlin.xyz/gtvxppbcqi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zhaomingkeji.xyz/gtpkksbruz.html

Go:   // 手写双层循环
来源：http://hz.pengpengdd.cyou/gtsnnxaslo.html

Ruby: nested.flatten
来源：http://hz.xuetiantiany.cn/gtexbfchgr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ydjk.org.cn/gtnjbkhpuv.html

[D19] 按字段分组
来源：http://hz.yuxming.cn/gtmohaytyu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.cqqwz.cn/gthdqmlkvl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.cqqwz.cn/gtpebvcpnl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.sweek.top/gtuxjgfbfr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhixingplan.top/gtppogndog.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jinghuilouyu.cn/gtnzezkwun.html

Go:   // 手写 map[string][]T
来源：http://hz.hfpthk.cn/gtkvpbbbpg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.pengpengdd.cyou/gtsdobvqfs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.nanxuanxn.top/gtfyteqobx.html

[D20] 统计每个元素出现次数
来源：http://hz.yuanzhike.top/gtkoagfahl.html

Py:   Counter(arr)
来源：http://hz.shanyushiyangkeji.top/gtzccrycxp.html

PHP:  array_count_values($arr);
来源：http://hz.zhengqikj.top/gtxnghhbet.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.dashuyun.cn/gtrorawdoo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj20258.top/gtejcrmwnr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ydzc1.top/gtqgcgsbol.html

Go:   // 手写 map[T]int
来源：http://hz.nanxuanxn.top/gtvacemxix.html

Ruby: arr.tally
来源：http://hz.gogol.net.cn/gtsoxmzper.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.aizwys.cn/gtrccygpru.html

[D21] 判断是否包含某元素
来源：http://hz.vqdsnc.cn/gtfosnqidm.html

Py:   x in arr
来源：http://hz.aibaodan.cn/gtrkpiiuxx.html

PHP:  in_array($x, $arr, true);
来源：http://hz.guannengcc.top/gtukangqpu.html

JS:   arr.includes(x)
来源：http://hz.hysaishi.cn/gtrptsawos.html

TS:   arr.includes(x)
来源：http://hz.hysaishi.cn/gtnvpzponn.html

Java: list.contains(x)
来源：http://hz.yangfankeji.com/gtaecdkjwy.html

Go:   slices.Contains(arr, x)
来源：http://hz.sxryk.cn/gtpphxjhmt.html

Ruby: arr.include?(x)
来源：http://hz.pycfn.com/gtsctnpfyb.html

C#:   list.Contains(x)
来源：http://hz.tian-w.cn/gtfmiiuncr.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jqgufenzy.top/gtobywrfwn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yanxiufei.cn/gtbwmuprby.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zhixingplan.top/gtprdreukt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.havefunace.top/gtwmxxtfkb.html

TS:   [...arr];
来源：http://hz.nwbrower.top/gtriqtszzd.html

Java: new ArrayList<>(list);
来源：http://hz.sxryk.cn/gthgbjzyxn.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.fzhhl.top/gtlgtbmbrr.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ivvv.top/gtlzmvmuuf.html

C#:   new List<int>(list);
来源：http://hz.cqqwz.cn/gtdbbbhhdq.html

[D23] reduce 累积计算
来源：http://hz.ppjwa.cn/gtncvnnwsg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.cqqwz.cn/gtkjrfvbka.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ywan-chungtsiang.top/gtqyaqjohl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.guowangkeji.top/gtcqzrrncb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhijiandao.cn/gttnuwgudv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhengqikj.top/gtglxbomxh.html

Go:   // 手写循环
来源：http://hz.hnqzz.top/gtzttulgbr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hammf.cn/gtvwwjkzas.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.shuidangran.top/gtljlaajxe.html

[D24] 字典 / Map 基本操作
来源：http://hz.yj20258888.top/gtvnlqaykv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.pycfn.com/gtclrdpexw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hnxiangtu.top/gtmkfuxbef.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.guowangkeji.top/gtmvbheduv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cucudq.cn/gtzzagkfdw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.cashguo.top/gttnwdluxz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yueranfly.top/gtosdgdsge.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jqgfzy.top/gtosrblbrh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hnqzz.top/gtdzhfcxmz.html

[D25] Set 集合去重与交并差
来源：http://hz.nanxinkj.top/gtgbjzkdft.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.cucudq.cn/gtkadffiko.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jinqigufen.top/gtwjmkidbv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.tian-w.cn/gtekpxejsb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yvedp.cn/gtentavfad.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.aizwys.cn/gtnfsjodut.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cqqwz.cn/gttvyxijqj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.pycfn.com/gtdjgpuwrd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.ybcxt.top/gtwczbzcys.html

[D26] 数组转字符串
来源：http://hz.zhongyouzk.top/gtrompwkmj.html

Py:   ", ".join(map(str, arr))
来源：http://hz.9152youxi.cn/gtysnovakq.html

PHP:  implode(", ", $arr);
来源：http://hz.daria6918.cn/gtfssrmtyn.html

JS:   arr.join(", ")
来源：http://hz.sufxvd.cn/gtfrxrxhuf.html

TS:   arr.join(", ")
来源：http://hz.jqgfzy.top/gtvsovgxzn.html

Java: String.join(", ", list)
来源：http://hz.9152youxi.cn/gtrrlcdolk.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jqgfzy.top/gtienxrbde.html

Ruby: arr.join(", ")
来源：http://hz.shuidangran.top/gtcguvgyee.html

C#:   string.Join(", ", list)
来源：http://hz.pengpengdd.cyou/gtjywcgbya.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtjdmsssex.html

E. 字符串处理
来源：http://hz.dashuyun.cn/gteirmruyw.html

================================================================================
来源：http://hz.zhixingplan.top/gtwrvthfyg.html

[E01] 拼接字符串
来源：http://hz.sxryk.cn/gtitlbblae.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yonumen.top/gtxfyvbddj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.sysykeji.top/gteghczqhg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.vqdsnc.cn/gtfcpsrwlm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.aibaodan.cn/gttbgcehdx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.pengpengdd.cyou/gtbajdypke.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yj20258.top/gtqtnbizpu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.pycfn.com/gtnkftumhi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhiwuduotai.top/gtbgwwtmfy.html

[E02] 重复字符串
来源：http://hz.zhijiandao.cn/gtwgleizev.html

Py:   "ab" * 3
来源：http://hz.cashguo.top/gttsvbkddv.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cheryme.top/gtbrbjufkt.html

JS:   "ab".repeat(3)
来源：http://hz.dianchejie.cn/gtntebipjz.html

TS:   "ab".repeat(3)
来源：http://hz.xuetiantiany.cn/gtlzaxmezi.html

Java: "ab".repeat(3)
来源：http://hz.wangdashe.top/gtjfhmxuea.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yuanzhike.top/gtuulogkoi.html

Ruby: "ab" * 3
来源：http://hz.chenlongwang.top/gtkxywhuxh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.birdmap.top/gtewehqhsq.html

[E03] 截取子串
来源：http://hz.shuidangran.top/gtihtryixr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.wangdashe.top/gtfhmymtkb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.redwolf501.top/gtdqzlzegz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.hnxiangtu.top/gtbguyljwa.html

TS:   s.slice(1, 4)
来源：http://hz.birdmap.top/gtpiamdxsd.html

Java: s.substring(1, 4)
来源：http://hz.shanyushiyangkeji.top/gtcbbhskpm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hfpthk.cn/gtidadkwpc.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jinqigufen.top/gtmphtqxau.html

C#:   s.Substring(1, 3)
来源：http://hz.cdnleiting.top/gtaprwllpa.html

[E04] 查找子串位置
来源：http://hz.hammf.cn/gtjqbkxcch.html

Py:   s.find("x");  s.index("x")
来源：http://hz.shanyushiyangkeji.top/gtzxgqiydh.html

PHP:  strpos($s, "x");
来源：http://hz.zhongyouzk.top/gtiwgdeftz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.guannengcc.top/gtbehxjkoe.html

TS:   s.indexOf("x")
来源：http://hz.cashguo.top/gtzjwwvzyf.html

Java: s.indexOf("x")
来源：http://hz.xinyue.icu/gtsmognujt.html

Go:   strings.Index(s, "x")
来源：http://hz.jqgufenzy.top/gtsygeeeoi.html

Ruby: s.index("x")
来源：http://hz.xziqi.cn/gtcvzvmjei.html

C#:   s.IndexOf("x")
来源：http://hz.birdmap.top/gtpsncbrpq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.ybcxt.top/gthlvdoizu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.sxryk.cn/gtdaibducz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.smart0.xyz/gtdmdkfdqg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhiwuduotai.top/gtokpwjona.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.svipenyu.cn/gttcxmuwer.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jqgufenzy.top/gtwmqeaiuo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.hnxiangtu.top/gtfwcdcbta.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yuanzhike.top/gtrzdwrnzc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.mhx1999.top/gtiqdksqny.html

[E06] 替换子串
来源：http://hz.hfpthk.cn/gtupsdesnl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.hnqzz.top/gtrwwwdhdd.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.sweek.top/gtdobjhxac.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.daxiang520.top/gtgncnaiuh.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ehwqpu.com/gtuuurrdwi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhongyouzk.top/gtckmnvjer.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.cqqwz.cn/gtcpbkbjcp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zdqjudy.top/gtgkwrlgqm.html

C#:   s.Replace("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtfhmazebb.html

[E07] 按分隔符拆分
来源：http://hz.hongshengwenyu.top/gtxdxqzmfe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.chenzaomai.com/gtmejrzyld.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.fzhhl.top/gtggzjjdsk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.bjfxy.top/gtsgtydpfe.html

TS:   s.split(",")
来源：http://hz.quarkkingdee.top/gtrgxdsids.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.iojbl.cn/gtpdtoymhj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jqgufenzy.top/gtxubxzrge.html

Ruby: s.split(",");  s.split
来源：http://hz.jinyuanbaomall.cn/gtxjkodicw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.quarkkingdee.top/gtcfwyivze.html

[E08] 数组按分隔符合并
来源：http://hz.hysaishi.cn/gtgtcqaxfq.html

Py:   ",".join(items)
来源：http://hz.tian-w.cn/gtskkbmwtn.html

PHP:  implode(",", $items);
来源：http://hz.cucudq.cn/gtglvjbqir.html

JS:   items.join(",")
来源：http://hz.jinyuanbaomall.cn/gtuyvadjnp.html

TS:   items.join(",")
来源：http://hz.fzhhl.top/gtscwtvwol.html

Java: String.join(",", items)
来源：http://hz.ydjk.org.cn/gtqxxtzksy.html

Go:   strings.Join(items, ",")
来源：http://hz.ybcxt.top/gtzeubvgcf.html

Ruby: items.join(",")
来源：http://hz.hnqzz.top/gtvkpyyboz.html

C#:   string.Join(",", items)
来源：http://hz.jinyuanbaomall.cn/gtydzxiekl.html

[E09] 去除所有空白字符
来源：http://hz.hnxiangtu.top/gtztsrxwkd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.cqqwz.cn/gtnjwbggao.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yj20258888.top/gtsaovhkdp.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.xuetiantiany.cn/gtwyeqeuxf.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jyoumei.cn/gtvmleqxve.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.meibo888.top/gtoghoppqj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.shzxlz.cn/gtrcelvvaq.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.xingfuxueyuan.xyz/gtdcricmsg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.sxryk.cn/gtnlyqoonh.html

[E10] 左侧补零 / 定长填充
来源：http://hz.aizwys.cn/gtjvysoepk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.nwbrower.top/gthibhfxli.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.ywan-chungtsiang.top/gtluguqfgb.html

JS:   "7".padStart(3, "0")
来源：http://hz.gotoacloud.top/gtmmqcaifr.html

TS:   "7".padStart(3, "0")
来源：http://hz.cqqwz.cn/gtpckfeivj.html

Java: String.format("%03d", 7)
来源：http://hz.guowangkeji.top/gtucykvedw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.hysaishi.cn/gtogtzbsbf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.daxiang520.top/gtnlchmkam.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.smart0.xyz/gtwhqogfsd.html

[E11] 反转字符串
来源：http://hz.fzhhl.top/gtsddqmcpg.html

Py:   s[::-1]
来源：http://hz.jinqigufen.top/gtwjoihcvj.html

PHP:  strrev($s);
来源：http://hz.shangyingyoupin.top/gtkkhtoajn.html

JS:   [...s].reverse().join("")
来源：http://hz.aizwys.cn/gtilzdhxpt.html

TS:   [...s].reverse().join("")
来源：http://hz.xuetiantiany.cn/gtteaxgbjq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.meibo888.top/gtrsvyfqcv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.dianchejie.cn/gtlqybvpmq.html

Ruby: s.reverse
来源：http://hz.meibo888.top/gtwzmncqvz.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.cqqwz.cn/gtmzvzeguy.html

[E12] 统计某字符出现次数
来源：http://hz.0kj1m.cn/gttokuwnxb.html

Py:   s.count("a")
来源：http://hz.yonumen.top/gtupdiszmj.html

PHP:  substr_count($s, "a");
来源：http://hz.aibaodan.cn/gtrjpvqipy.html

JS:   s.split("a").length - 1
来源：http://hz.hnqzz.top/gtfepizbqz.html

TS:   s.split("a").length - 1
来源：http://hz.chenjidiqi.icu/gtyczydsyx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jinghuilouyu.cn/gtnseomuyt.html

Go:   strings.Count(s, "a")
来源：http://hz.aizwys.cn/gtrncgllvg.html

Ruby: s.count("a")
来源：http://hz.kuanghao11.cn/gtnoludqje.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jqgfzy.top/gtsriovqrt.html

[E13] 逐字符遍历
来源：http://hz.cdnleiting.top/gtlfhetuvp.html

Py:   for ch in s: print(ch)
来源：http://hz.jinqigfzy.top/gtwkpzhagc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhaomingkeji.xyz/gtjkajcijn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cucudq.cn/gtvkkkcpnz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ydzc1.top/gtivnfzhfe.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.gotoacloud.top/gtecjjnurn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ehwqpu.com/gtihrbydbf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.xziqi.cn/gtocnditzk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.sufxvd.cn/gthckfurzw.html

[E14] URL 编码与 Base64
来源：http://hz.tanke756.top/gtldmqtwbr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.kuanghao11.cn/gtnnjbgbsx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.iojbl.cn/gtypavifwm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yongpay.top/gthexcsydf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.nwbrower.top/gtubzjqcnv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhixingplan.top/gtcdobhfzt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ywan-chungtsiang.top/gthdlqfawa.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.0kj1m.cn/gtjdurmfos.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cheryme.top/gtsflvbmte.html

[E15] HTML 转义 / 反转义
来源：http://hz.ybcxt.top/gtnctxvwyn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.svipenyu.cn/gtevtltxxz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.svipenyu.cn/gtxelosxxi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yj202588.top/gtyucqhivz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jqgufenzy.top/gtzdxkmydy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.andypj.xyz/gtiothkehc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zhixingplan.top/gtvfttsxqs.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jinyuanbaomall.cn/gteaicjvpw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.guannengcc.top/gtltzzspuw.html

[E16] 数字千分位
来源：http://hz.ydjk.org.cn/gtivqfhzem.html

Py:   f"{1234567:,}"
来源：http://hz.birdmap.top/gttxvkxaka.html

PHP:  number_format(1234567);
来源：http://hz.zycfv.cn/gtbraweesp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.xylfe.cn/gtfiagywiw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhixingplan.top/gtpyduxfwp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yj20258.top/gtuisktbkn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.fengsongda.top/gtzcozykqh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cqqwz.cn/gtmjtsyeow.html

C#:   1234567.ToString("N0")
来源：http://hz.jqgufenzy.top/gtmddjsztt.html

[E17] 首字母大写
来源：http://hz.ybcxt.top/gtttnceabh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xylfe.cn/gtcfidoify.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yongpay.top/gtsvedbzty.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.guannengcc.top/gtzyjdcipe.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.dashuyun.cn/gtvvrvcgep.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yongpay.top/gtkexlarzq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.nanxinkj.top/gtjsvasjnk.html

Ruby: s.capitalize
来源：http://hz.fengsongda.top/gtkkupdqee.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.9152youxi.cn/gtpeqpslfk.html

[E18] 模板占位符替换
来源：http://hz.nanxinkj.top/gticipucen.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhongyouzk.top/gtagobldjh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.52xcode.cn/gtoppznusw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.dashuyun.cn/gtjurasqcp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jiagoushi.top/gtmugwyqhq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.dianchejie.cn/gtvgaxhzpq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.havefunace.top/gtcwftgxyy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.gogol.net.cn/gtcrdvbbom.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.cqqwz.cn/gtayqjxjnk.html

[E19] 多行文本按行拆分
来源：http://hz.xingfuxueyuan.xyz/gtufofwgdc.html

Py:   s.splitlines()
来源：http://hz.dashuyun.cn/gtvrvjqwvz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.ydjk.org.cn/gtridrbwae.html

JS:   s.split(/\r?\n/)
来源：http://hz.xziqi.cn/gtjwmnjqgq.html

TS:   s.split(/\r?\n/)
来源：http://hz.bjfxy.top/gtkmopwgzb.html

Java: s.lines().toList()
来源：http://hz.jqgfzy.top/gtnbqndghr.html

Go:   strings.Split(s, "\n")
来源：http://hz.havefunace.top/gtochxnguc.html

Ruby: s.lines
来源：http://hz.cucudq.cn/gtvcbbaasr.html

C#:   s.Split('\n')
来源：http://hz.jinghuilouyu.cn/gtteajvjdi.html

[E20] 判断字符串是否为空
来源：http://hz.gaohongyu789.top/gtfsohtwjj.html

Py:   if not s:
来源：http://hz.zhiwuduotai.top/gtrlasezqg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.mhx1999.top/gtrllldtjs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.quarkkingdee.top/gtwnzfrkhw.html

TS:   if (s === "") {}
来源：http://hz.316326.xyz/gtiizwcywv.html

Java: if (s.isEmpty()) {}
来源：http://hz.cucudq.cn/gtdgmqcytg.html

Go:   if s == "" {}
来源：http://hz.xuetiantiany.cn/gtdxxeuhsh.html

Ruby: if s.empty?
来源：http://hz.zycfv.cn/gtkmlffvho.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhiwuduotai.top/gtaikciphl.html

[E21] 超长截断加省略号
来源：http://hz.yangfankeji.com/gteqqctnqh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.9152youxi.cn/gttuqjscsd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yuxming.cn/gtmdvlxepo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yueranfly.top/gtfetrjorg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.dashuyun.cn/gtfhzmhtbd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.shuidangran.top/gtutpqggmy.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yj20258888.top/gtdwcvunxq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.shanyushiyangtech.top/gtslknvjke.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jqgufenzy.top/gtjuwioefs.html

[E22] 字节长度与字符长度
来源：http://hz.pengpengdd.cyou/gtnnecfjua.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.pycfn.com/gtkhxgbjaa.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgufenzy.top/gtlsvkfdik.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xinyue.icu/gtpktylpoy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhongyouzk.top/gtcznsejqj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.guowangkeji.top/gtgahuzevm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.tianlin.xyz/gttxvkacbm.html

Ruby: s.bytesize;  s.length
来源：http://hz.xylfe.cn/gtkttrpebl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.ydjk.org.cn/gtpzbssjbz.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtgvzwufpw.html

F. 文件与目录
来源：http://hz.9152youxi.cn/gtnhdezzqc.html

================================================================================
来源：http://hz.yanxiufei.cn/gtzkbkizwb.html

[F01] 读取整个文件
来源：http://hz.cucudq.cn/gtsqrykyap.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.sufxvd.cn/gtwxtibttj.html

PHP:  file_get_contents("a.txt");
来源：http://hz.meibo888.top/gtiztwmwws.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.9152youxi.cn/gtinydicxh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.iojbl.cn/gtxiqulawb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jyoumei.cn/gtmhmlwjqz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.andypj.xyz/gtprexpdmq.html

Ruby: File.read("a.txt")
来源：http://hz.pycfn.com/gtolsessjx.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.pengpengdd.cyou/gtinzkjvtp.html

[F02] 逐行读取文件
来源：http://hz.jiagoushi.top/gtlbtytrew.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hnxiangtu.top/gtrhpxuxvf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yuxming.cn/gtqsmiiwyc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ydjk.org.cn/gtxknsgzbv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xinyue.icu/gtanbgpuqw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.feifeiyinyue.top/gtcwczkjhh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.aizwys.cn/gtepwtkyfu.html


<!-- 参考信息 -->