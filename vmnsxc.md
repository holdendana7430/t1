代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://hz.xziqi.cn/gtpwxxhqrs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yueranfly.top/gtxmqpheks.html

TS:   Math.max(...arr);
来源：http://hz.haohaochexian.top/gtoluautcp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hongshengwenyu.top/gterkesuli.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hnqzz.top/gtrvdccfyp.html

Ruby: arr.max;  arr.min
来源：http://hz.chenjidiqi.icu/gtjrkxqboc.html

C#:   list.Max();  list.Min()
来源：http://hz.sysykeji.top/gtbeknxcnp.html

[D18] 扁平化嵌套数组
来源：http://hz.gogol.net.cn/gtzgalbkeq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xuanzx.com/gtgdovrrha.html

PHP:  array_merge(...$nested);
来源：http://hz.vqdsnc.cn/gtwapmimkl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yanxiufei.cn/gtpwqemwxw.html

TS:   nested.flat();
来源：http://hz.jinyuanbaomall.cn/gtyrrmpezj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ybcxt.top/gtzzmhoxpu.html

Go:   // 手写双层循环
来源：http://hz.gzhubu.top/gtiyhudnsp.html

Ruby: nested.flatten
来源：http://hz.zhoulong.xyz/gtljolrvsl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yuanzhike.top/gtkpdrocdl.html

[D19] 按字段分组
来源：http://hz.zhijiandao.cn/gtoeqprdvt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yj202588.top/gtfbixoikn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.gogol.net.cn/gtirzvwkmp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.tanke756.top/gtuaeurvkw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.havefunace.top/gtlwbwvzgz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhijiandao.cn/gtmszcheac.html

Go:   // 手写 map[string][]T
来源：http://hz.gzhubu.top/gtuunttoke.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.wangshuangyany.cn/gtgtgrwkus.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhixingplan.top/gthseevlal.html

[D20] 统计每个元素出现次数
来源：http://hz.xylfe.cn/gthcusgkmw.html

Py:   Counter(arr)
来源：http://hz.jinyuanbaomall.cn/gtfpkxjpbb.html

PHP:  array_count_values($arr);
来源：http://hz.xziqi.cn/gtciptyyhe.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.fengsongda.top/gtdgibuhcm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.bjfxy.top/gtohzbrveu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.nanxinkj.top/gtdfzdlbfk.html

Go:   // 手写 map[T]int
来源：http://hz.hammf.cn/gtpolcnbkr.html

Ruby: arr.tally
来源：http://hz.cdnleiting.top/gtiuweahln.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.pengpengdd.cyou/gtqnzwkwwi.html

[D21] 判断是否包含某元素
来源：http://hz.yj202588.top/gtymtaucgc.html

Py:   x in arr
来源：http://hz.bjfxy.top/gtmakywqhp.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yueranfly.top/gtgoythhcq.html

JS:   arr.includes(x)
来源：http://hz.yuxming.cn/gtsiiwneea.html

TS:   arr.includes(x)
来源：http://hz.meibo888.top/gthxhoarly.html

Java: list.contains(x)
来源：http://hz.smart0.xyz/gtwwymctdu.html

Go:   slices.Contains(arr, x)
来源：http://hz.kuanghao11.cn/gtnqewpehf.html

Ruby: arr.include?(x)
来源：http://hz.jinqigfzy.top/gthdlcusff.html

C#:   list.Contains(x)
来源：http://hz.jinyuanbaomall.cn/gtqzvpctnq.html

[D22] 复制数组（避免共享引用）
来源：http://hz.gaohongyu789.top/gtdzbcyhcn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.nanxinkj.top/gtryhfbbek.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yonumen.top/gtgloqpcgf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.meibo888.top/gtgzipyhab.html

TS:   [...arr];
来源：http://hz.zycfv.cn/gtjehfekoz.html

Java: new ArrayList<>(list);
来源：http://hz.hywenlv.cn/gtdwzdscvy.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hnxiangtu.top/gtytpygwpe.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zycfv.cn/gtwznzhlvz.html

C#:   new List<int>(list);
来源：http://hz.sysykeji.top/gtgrftfydd.html

[D23] reduce 累积计算
来源：http://hz.svipenyu.cn/gtfhbnxyms.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.cheryme.top/gtsqsqbxrc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.svipenyu.cn/gtnetoxdgs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.havefunace.top/gtxodesdcc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhengqikj.top/gtsgzzoort.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.aibaodan.cn/gtlkxhiuzk.html

Go:   // 手写循环
来源：http://hz.316326.xyz/gtqfhgejnj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yj20258888.top/gtsdeinxdz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.vqdsnc.cn/gtxascwxqi.html

[D24] 字典 / Map 基本操作
来源：http://hz.jqgufenzy.top/gtevdkosjm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.cashguo.top/gtwadlrjin.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hysaishi.cn/gtkxvzykqb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zycfv.cn/gtxqgirdqa.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.zdqjudy.top/gtxogaleaw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ehwqpu.com/gtiprocfss.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jinyuanbaomall.cn/gtnswvohnk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.feifeiyinyue.top/gtuvdrljiw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.guowangkeji.top/gtswtgnbsd.html

[D25] Set 集合去重与交并差
来源：http://hz.hongshengwenyu.top/gtkvsmqxue.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.guannengcc.top/gtoeukywfu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.52xcode.cn/gtqumjnzkt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.shanyushiyangtech.top/gtvtbfcxxp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yj20258888.top/gthnsfqjck.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.tianlin.xyz/gtvenqiicc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.quarkkingdee.top/gtcocprclu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yuanzhike.top/gtuskfmhuc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.nanxuanxn.top/gtonsgkvdc.html

[D26] 数组转字符串
来源：http://hz.xinyue.icu/gtrrqxhmhs.html

Py:   ", ".join(map(str, arr))
来源：http://hz.andypj.xyz/gtrpydzgly.html

PHP:  implode(", ", $arr);
来源：http://hz.shanyushiyangtech.top/gtgvyywgdr.html

JS:   arr.join(", ")
来源：http://hz.guowangkeji.top/gteubzrcld.html

TS:   arr.join(", ")
来源：http://hz.tian-w.cn/gtniymtbnh.html

Java: String.join(", ", list)
来源：http://hz.aizwys.cn/gtfruqwfzc.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhijiandao.cn/gtullogghi.html

Ruby: arr.join(", ")
来源：http://hz.sysykeji.top/gtcljvhtvb.html

C#:   string.Join(", ", list)
来源：http://hz.svipenyu.cn/gttxglfvvk.html

================================================================================
来源：http://hz.316326.xyz/gthfphntnq.html

E. 字符串处理
来源：http://hz.gaohongyu789.top/gtsvhicfmk.html

================================================================================
来源：http://hz.redwolf501.top/gtztykbuiq.html

[E01] 拼接字符串
来源：http://hz.wangshuangyany.cn/gtqoxtpzyx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.dashuyun.cn/gtgmolrerp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.shuidangran.top/gtxqvqdndn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ydjk.org.cn/gtnklnrsqi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xuetiantiany.cn/gtwttrptaf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yanxiufei.cn/gtxasezqnc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.tanke756.top/gtljhwfgrv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.cqqwz.cn/gtlabppedv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jinghuilouyu.cn/gtqcgkwcay.html

[E02] 重复字符串
来源：http://hz.xylfe.cn/gtutoairzm.html

Py:   "ab" * 3
来源：http://hz.yanxiufei.cn/gtoycvghaa.html

PHP:  str_repeat("ab", 3);
来源：http://hz.meibo888.top/gtecqzdinr.html

JS:   "ab".repeat(3)
来源：http://hz.cheryme.top/gtwthtexdn.html

TS:   "ab".repeat(3)
来源：http://hz.zhengqikj.top/gtmdtmmsps.html

Java: "ab".repeat(3)
来源：http://hz.tianlin.xyz/gtavewgjgc.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.nwbrower.top/gtxzlxovls.html

Ruby: "ab" * 3
来源：http://hz.pycfn.com/gtpwyomfnr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.c1oappe.top/gtbeuwtowl.html

[E03] 截取子串
来源：http://hz.xinyue.icu/gtddzuxddf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.shanyushiyangkeji.top/gtnwsqzjxw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.chenlongwang.top/gtkcbvlemz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zdqjudy.top/gtzynguapx.html

TS:   s.slice(1, 4)
来源：http://hz.sxryk.cn/gtniuezbnx.html

Java: s.substring(1, 4)
来源：http://hz.dianchejie.cn/gtfigegrgr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhongyouzk.top/gttmvowatl.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.daxiang520.top/gtfyslpvfa.html

C#:   s.Substring(1, 3)
来源：http://hz.guowangkeji.top/gthkaapfog.html

[E04] 查找子串位置
来源：http://hz.yangfankeji.com/gtqksopqks.html

Py:   s.find("x");  s.index("x")
来源：http://hz.bjfxy.top/gtmthzdsdk.html

PHP:  strpos($s, "x");
来源：http://hz.nanxinkj.top/gtluadmxpy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ydjk.org.cn/gtcqorfmed.html

TS:   s.indexOf("x")
来源：http://hz.tanke756.top/gtfxvdxxcj.html

Java: s.indexOf("x")
来源：http://hz.gotoacloud.top/gtliecxcrb.html

Go:   strings.Index(s, "x")
来源：http://hz.hysaishi.cn/gtfeggvhnd.html

Ruby: s.index("x")
来源：http://hz.0kj1m.cn/gtryjdzwda.html

C#:   s.IndexOf("x")
来源：http://hz.aizwys.cn/gtswvbzegc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.sxryk.cn/gtbfajrufk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhixingplan.top/gtrjvcgahq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yj20258.top/gtrsygewqn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zycfv.cn/gttgenwkga.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zdqjudy.top/gtozadnmzw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jiagoushi.top/gthtgdlgtk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.pycfn.com/gthwgugqgb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jqgufenzy.top/gtksjpyeod.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.aizwys.cn/gtysgfnnas.html

[E06] 替换子串
来源：http://hz.yongpay.top/gttbpnvwcy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.snrcjt.cn/gttkmmrnwv.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.0kj1m.cn/gtvazkiwzx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtnrvutnwx.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yueranfly.top/gtuaitocch.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.quarkkingdee.top/gtfagejwmh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.xziqi.cn/gtauvwhxqy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ywan-chungtsiang.top/gtokyymcnp.html

C#:   s.Replace("a", "b")
来源：http://hz.pycfn.com/gtqkjsiurd.html

[E07] 按分隔符拆分
来源：http://hz.redwolf501.top/gtilgddjje.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.haohaochexian.top/gtsmeplkrt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jiagoushi.top/gtshsyhbid.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yangfankeji.com/gtstsgqtmd.html

TS:   s.split(",")
来源：http://hz.yj202588.top/gtuhbosryh.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yj20258.top/gtxbpodznr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yj20258888.top/gtbpvrfzok.html

Ruby: s.split(",");  s.split
来源：http://hz.cheryme.top/gtonrjdoay.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.shuidangran.top/gtbiqqcdtk.html

[E08] 数组按分隔符合并
来源：http://hz.guannengcc.top/gtkoffuwiy.html

Py:   ",".join(items)
来源：http://hz.tianlin.xyz/gtovlogbkp.html

PHP:  implode(",", $items);
来源：http://hz.xuetiantiany.cn/gtexpnquzy.html

JS:   items.join(",")
来源：http://hz.ppjwa.cn/gtfyjppeob.html

TS:   items.join(",")
来源：http://hz.sysykeji.top/gtrrvydhkz.html

Java: String.join(",", items)
来源：http://hz.ehwqpu.com/gtfrwcnrhw.html

Go:   strings.Join(items, ",")
来源：http://hz.xylfe.cn/gtvjkgnuqa.html

Ruby: items.join(",")
来源：http://hz.ivvv.top/gtejkgikxs.html

C#:   string.Join(",", items)
来源：http://hz.andypj.xyz/gthnzovcql.html

[E09] 去除所有空白字符
来源：http://hz.52xcode.cn/gtowqtmvxv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.nwbrower.top/gtcpulebop.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.andypj.xyz/gtdvjthqff.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.haohaochexian.top/gtuezjscai.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.cheryme.top/gtuldetbgt.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.redwolf501.top/gtmfwidyje.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hfpthk.cn/gtgbsrbhhe.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jinqigfzy.top/gtfsybyexq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jinqigufen.top/gtmdzywivj.html

[E10] 左侧补零 / 定长填充
来源：http://hz.0kj1m.cn/gtwezrxxjn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.gaohongyu789.top/gtmgrnlvac.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jiagoushi.top/gtlitpmsyt.html

JS:   "7".padStart(3, "0")
来源：http://hz.jinqigufen.top/gtkiybykmh.html

TS:   "7".padStart(3, "0")
来源：http://hz.bjfxy.top/gtojvrjrzt.html

Java: String.format("%03d", 7)
来源：http://hz.shanyushiyangtech.top/gtyagdpjgc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.tian-w.cn/gtbezcwvqu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gogol.net.cn/gtzqcbmzzi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.pengpengdd.cyou/gtegmznusg.html

[E11] 反转字符串
来源：http://hz.dashuyun.cn/gtcjteynkh.html

Py:   s[::-1]
来源：http://hz.yueranfly.top/gteoouckyw.html

PHP:  strrev($s);
来源：http://hz.xuanzx.com/gtfbqoneht.html

JS:   [...s].reverse().join("")
来源：http://hz.sxryk.cn/gtskourqwa.html

TS:   [...s].reverse().join("")
来源：http://hz.wangshuangyany.cn/gtcythqaci.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.aizwys.cn/gtjrqiddxb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xziqi.cn/gtxhwxxgng.html

Ruby: s.reverse
来源：http://hz.vqdsnc.cn/gtuywsdreo.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.gogol.net.cn/gtlkhknkyk.html

[E12] 统计某字符出现次数
来源：http://hz.dianchejie.cn/gtbexqargt.html

Py:   s.count("a")
来源：http://hz.shanyushiyangtech.top/gtbnxpgosu.html

PHP:  substr_count($s, "a");
来源：http://hz.bjfxy.top/gtgidxmtvl.html

JS:   s.split("a").length - 1
来源：http://hz.chenzaomai.com/gtulqybkme.html

TS:   s.split("a").length - 1
来源：http://hz.havefunace.top/gtyjymyqqc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hywenlv.cn/gtnbwkjczz.html

Go:   strings.Count(s, "a")
来源：http://hz.hnxiangtu.top/gtqlxtxgew.html

Ruby: s.count("a")
来源：http://hz.shangyingyoupin.top/gttuhcypvg.html

C#:   s.Count(c => c == 'a')
来源：http://hz.cheryme.top/gtwelddpil.html

[E13] 逐字符遍历
来源：http://hz.sufxvd.cn/gtyvoglabb.html

Py:   for ch in s: print(ch)
来源：http://hz.tian-w.cn/gteokimvqu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.chenzaomai.com/gttkiwrcwh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xinyue.icu/gtoekwgodx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zycfv.cn/gtswjbpsra.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zycfv.cn/gtesxrcfjp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ivvv.top/gtbetrnepy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.xuanzx.com/gtjffwiicb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yj20258.top/gtemqqrgpw.html

[E14] URL 编码与 Base64
来源：http://hz.jqgfzy.top/gtqqlwjtul.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ivvv.top/gtwqtkplqe.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.shanyushiyangtech.top/gtgnbovrbd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.aibaodan.cn/gtvmnoruta.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.aizwys.cn/gtjeitfzeg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.gotoacloud.top/gtxdxwjakf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jinqigufen.top/gtwpasulnx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.tianlin.xyz/gtrlyklfio.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhiwuduotai.top/gtpgcluavd.html

[E15] HTML 转义 / 反转义
来源：http://hz.svipenyu.cn/gtwkqwmyus.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.daria6918.cn/gtmxerstwq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.vqdsnc.cn/gtnbcqrhqs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zdqjudy.top/gtetymhzun.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.shuidangran.top/gtysyckxxs.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zycfv.cn/gtmtfkjdvd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yj20258.top/gtlytazhyu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.xingfuxueyuan.xyz/gtwhuiaynr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.snrcjt.cn/gtwvgtmwxl.html

[E16] 数字千分位
来源：http://hz.jiagoushi.top/gtjbpbywsw.html

Py:   f"{1234567:,}"
来源：http://hz.aibaodan.cn/gtufpacizj.html

PHP:  number_format(1234567);
来源：http://hz.kuanghao11.cn/gtmvolcjwt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.daria6918.cn/gttpxleopn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.meibo888.top/gtkrpbgtkm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.shanyushiyangtech.top/gtklbwxqir.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.cdnleiting.top/gtyyjtubir.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yangfankeji.com/gtmlfziisb.html

C#:   1234567.ToString("N0")
来源：http://hz.hnqzz.top/gtcwbqlyrc.html

[E17] 首字母大写
来源：http://hz.hnxiangtu.top/gtlkvojrsc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yuxming.cn/gtkypdrsxk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.ivvv.top/gtkotqxmwz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tanke756.top/gtczfgwvvf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhongyouzk.top/gtwkkxfowt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ydzc1.top/gtayyzxxit.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jiagoushi.top/gtdqzmfbcv.html

Ruby: s.capitalize
来源：http://hz.cqqwz.cn/gtpgxqplnz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xinyue.icu/gtqmzstlua.html

[E18] 模板占位符替换
来源：http://hz.jqgfzy.top/gtobiyghqu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ppjwa.cn/gthckwubto.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xinyue.icu/gtqifmrvfj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.vqdsnc.cn/gtidyfaxgw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.tanke756.top/gtywdmexvz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinyuanbaomall.cn/gtjhlpvftb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.gaohongyu789.top/gtpndbegtr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.nanxuanxn.top/gttuxytwpu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.bjfxy.top/gtngxvwekm.html

[E19] 多行文本按行拆分
来源：http://hz.ehwqpu.com/gtucwhajds.html

Py:   s.splitlines()
来源：http://hz.sweek.top/gtnedogear.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.tanke756.top/gthbferwri.html

JS:   s.split(/\r?\n/)
来源：http://hz.nanxuanxn.top/gtdtxdwuqh.html

TS:   s.split(/\r?\n/)
来源：http://hz.dashuyun.cn/gtvzfzdxgc.html

Java: s.lines().toList()
来源：http://hz.shzxlz.cn/gtokshgfgl.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhijiandao.cn/gtrbjgfarv.html

Ruby: s.lines
来源：http://hz.iojbl.cn/gtfqagwkjb.html

C#:   s.Split('\n')
来源：http://hz.zhiwuduotai.top/gttjscarwp.html

[E20] 判断字符串是否为空
来源：http://hz.xinyue.icu/gtgrbuxlfs.html

Py:   if not s:
来源：http://hz.smart0.xyz/gtqgvyztih.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jianghu66.top/gtlfomnedw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.chenzaomai.com/gtjllkckjb.html

TS:   if (s === "") {}
来源：http://hz.gaohongyu789.top/gtkrxxkwno.html

Java: if (s.isEmpty()) {}
来源：http://hz.quarkkingdee.top/gtsiyhckwo.html

Go:   if s == "" {}
来源：http://hz.hongshengwenyu.top/gtbwhsuiri.html

Ruby: if s.empty?
来源：http://hz.gotoacloud.top/gtthbwdcnh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.bjfxy.top/gtntjpqdcl.html

[E21] 超长截断加省略号
来源：http://hz.yj20258.top/gttjwurgtf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jianghu66.top/gtcvuldsfp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.snrcjt.cn/gtpwyutyrw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sysykeji.top/gtssuhczwl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinqigfzy.top/gttxkzvqhw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jinqigufen.top/gtbzlovhpk.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yvedp.cn/gtjvvvoboo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.havefunace.top/gtrrxeqmzu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ywan-chungtsiang.top/gtfhyelklb.html

[E22] 字节长度与字符长度
来源：http://hz.tianlin.xyz/gthbrdtxno.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zycfv.cn/gtffgoqitx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.smart0.xyz/gtjxyhbtde.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.wangdashe.top/gtxoxoqrfg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhengqikj.top/gtfphcldpl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.shuidangran.top/gtwvkoaixo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.nanxuanxn.top/gtjsnawznt.html

Ruby: s.bytesize;  s.length
来源：http://hz.jiagoushi.top/gtskwbcffw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jlsjyb.cn/gtrhpztihb.html

================================================================================
来源：http://hz.yangfankeji.com/gtczutgzow.html

F. 文件与目录
来源：http://hz.xinyue.icu/gtzxigpwyg.html

================================================================================
来源：http://hz.zhongyouzk.top/gtyxgsvksy.html

[F01] 读取整个文件
来源：http://hz.kuanghao11.cn/gtmfyzgrwg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.daxiang520.top/gtjxxudlyg.html

PHP:  file_get_contents("a.txt");
来源：http://hz.meibo888.top/gtmjusmxcj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.iojbl.cn/gtwjxxemvi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yuxming.cn/gtjglfdphl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhaomingkeji.xyz/gtwgegdqdv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.chenlongwang.top/gtckyirrwn.html

Ruby: File.read("a.txt")
来源：http://hz.jqgufenzy.top/gtvdovvnej.html


<!-- 参考信息 -->