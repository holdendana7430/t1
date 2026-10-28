代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jlsjyb.cn/gtthcilupj.html

C#:   list.Sum();  list.Average()
来源：http://hz.52xcode.cn/gtfbqlutzh.html

[D17] 最大值与最小值
来源：http://hz.pycfn.com/gtlelorzyf.html

Py:   max(arr);  min(arr)
来源：http://hz.aibaodan.cn/gtimaiiqjr.html

PHP:  max($arr);  min($arr);
来源：http://hz.redwolf501.top/gtvfykoepc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.cdnleiting.top/gtigyrkapa.html

TS:   Math.max(...arr);
来源：http://hz.pengpengdd.cyou/gtsxwbidyf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xuetiantiany.cn/gtboupwqlm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yj202588.top/gtumjvtwxs.html

Ruby: arr.max;  arr.min
来源：http://hz.jianghu66.top/gtynnfqkfd.html

C#:   list.Max();  list.Min()
来源：http://hz.aizwys.cn/gtvvhrurbl.html

[D18] 扁平化嵌套数组
来源：http://hz.jinqigufen.top/gtvmdfrwns.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.cheryme.top/gtqhoirwhb.html

PHP:  array_merge(...$nested);
来源：http://hz.snrcjt.cn/gtbbkforyk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hywenlv.cn/gtxhtggopr.html

TS:   nested.flat();
来源：http://hz.zhiwuduotai.top/gtwyvbnbai.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zhijiandao.cn/gtnpbnxxqt.html

Go:   // 手写双层循环
来源：http://hz.ywan-chungtsiang.top/gtqnlqkepr.html

Ruby: nested.flatten
来源：http://hz.ppjwa.cn/gtaqqexhky.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhijiandao.cn/gtisiqdfzt.html

[D19] 按字段分组
来源：http://hz.ppjwa.cn/gtjazitdoc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jlsjyb.cn/gtmxwrrmuo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.vqdsnc.cn/gtmvstjvgv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.316326.xyz/gteturoejx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.tian-w.cn/gttomkyjhi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.xziqi.cn/gtlsliqveu.html

Go:   // 手写 map[string][]T
来源：http://hz.cucudq.cn/gterzblork.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.xuanzx.com/gtkbfgdmmf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.gotoacloud.top/gtprmuksot.html

[D20] 统计每个元素出现次数
来源：http://hz.zdqjudy.top/gtokanuzsp.html

Py:   Counter(arr)
来源：http://hz.daxiang520.top/gthdtixnrr.html

PHP:  array_count_values($arr);
来源：http://hz.jinghuilouyu.cn/gtipagityg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.wangshuangyany.cn/gtvegpajlu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.kuanghao11.cn/gtrlpvkbyn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.guowangkeji.top/gtmabibjkg.html

Go:   // 手写 map[T]int
来源：http://hz.xziqi.cn/gthcaflcnq.html

Ruby: arr.tally
来源：http://hz.cheryme.top/gtsbqlyxue.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.haohaochexian.top/gtutshqrhk.html

[D21] 判断是否包含某元素
来源：http://hz.iojbl.cn/gtmuglomjx.html

Py:   x in arr
来源：http://hz.jinyuanbaomall.cn/gtquyiiyxd.html

PHP:  in_array($x, $arr, true);
来源：http://hz.redwolf501.top/gtsmclalsn.html

JS:   arr.includes(x)
来源：http://hz.jinyuanbaomall.cn/gthufoarap.html

TS:   arr.includes(x)
来源：http://hz.shuidangran.top/gtawtovjwm.html

Java: list.contains(x)
来源：http://hz.nwbrower.top/gtacimbsbj.html

Go:   slices.Contains(arr, x)
来源：http://hz.jinghuilouyu.cn/gtzjjhbdbk.html

Ruby: arr.include?(x)
来源：http://hz.xingfuxueyuan.xyz/gtyjobnfnq.html

C#:   list.Contains(x)
来源：http://hz.cqqwz.cn/gtqueysydw.html

[D22] 复制数组（避免共享引用）
来源：http://hz.fengsongda.top/gtvqqpvqdh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.feifeiyinyue.top/gtnxzejgqw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ybcxt.top/gtvfgllyyp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.gaohongyu789.top/gtyvszhcnd.html

TS:   [...arr];
来源：http://hz.zhijiandao.cn/gtoqqavzuz.html

Java: new ArrayList<>(list);
来源：http://hz.aizwys.cn/gtlhblbzrl.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.mhx1999.top/gtgfjnsjti.html

Ruby: arr.dup;  arr.clone
来源：http://hz.guannengcc.top/gtzhungnhr.html

C#:   new List<int>(list);
来源：http://hz.tianlin.xyz/gtaisuglzh.html

[D23] reduce 累积计算
来源：http://hz.yonumen.top/gtnmooxyoz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zycfv.cn/gtorjwhikn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.tianlin.xyz/gtjzxhazru.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.redwolf501.top/gtqpomgxwv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.aibaodan.cn/gtvubkkcyf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jinghuilouyu.cn/gthsrftoyg.html

Go:   // 手写循环
来源：http://hz.9152youxi.cn/gthmynjlyi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.havefunace.top/gtfbeghdfh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.cqqwz.cn/gtnrpsmkmy.html

[D24] 字典 / Map 基本操作
来源：http://hz.yangfankeji.com/gtghyzhsjf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.sxryk.cn/gtjssjlkgb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.cashguo.top/gtvxiddwtm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.gaohongyu789.top/gtxibqclgf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yongpay.top/gtyfswraru.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.meibo888.top/gtcyyfchza.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.birdmap.top/gtiorlvqwv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.birdmap.top/gtpntdjvwp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.gaohongyu789.top/gtofvnookx.html

[D25] Set 集合去重与交并差
来源：http://hz.bjfxy.top/gtrxrzpnqf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.shanyushiyangkeji.top/gtemdqxdhe.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jlsjyb.cn/gtrpuozevl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ppjwa.cn/gtecfiwlye.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhixingplan.top/gtcdustdrp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.shanyushiyangtech.top/gtvkwoxyin.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hnxiangtu.top/gtjoazwajj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xylfe.cn/gtwlrzlmkd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jinqigufen.top/gtxyojaxxc.html

[D26] 数组转字符串
来源：http://hz.chenzaomai.com/gtvamoiecc.html

Py:   ", ".join(map(str, arr))
来源：http://hz.cheryme.top/gtjdeyujwy.html

PHP:  implode(", ", $arr);
来源：http://hz.ywan-chungtsiang.top/gtmetiwonm.html

JS:   arr.join(", ")
来源：http://hz.iojbl.cn/gtwnchvzew.html

TS:   arr.join(", ")
来源：http://hz.yj20258.top/gtmphrbldh.html

Java: String.join(", ", list)
来源：http://hz.hywenlv.cn/gthgrffhio.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jinqigfzy.top/gtunwgmlyr.html

Ruby: arr.join(", ")
来源：http://hz.shzxlz.cn/gtpnrbluym.html

C#:   string.Join(", ", list)
来源：http://hz.daria6918.cn/gtlbgfwblr.html

================================================================================
来源：http://hz.sysykeji.top/gtwvsnjczj.html

E. 字符串处理
来源：http://hz.cucudq.cn/gteadqxump.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtqwfushqu.html

[E01] 拼接字符串
来源：http://hz.fengsongda.top/gtnumteofa.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jyoumei.cn/gtawmggfyz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.chenzaomai.com/gtnuafrfon.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinqigufen.top/gtemtchhvj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shanyushiyangkeji.top/gtejasqdlw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zhaomingkeji.xyz/gtvqvnqmeu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hnxiangtu.top/gtqxfvxvdu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yj20258.top/gtxvtnpchw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yuxming.cn/gtlsmixapq.html

[E02] 重复字符串
来源：http://hz.hfpthk.cn/gtatubvvzq.html

Py:   "ab" * 3
来源：http://hz.snrcjt.cn/gtcvtlmfyx.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jiagoushi.top/gtathanwbm.html

JS:   "ab".repeat(3)
来源：http://hz.zhaomingkeji.xyz/gtxvputpbs.html

TS:   "ab".repeat(3)
来源：http://hz.hnqzz.top/gtpcibwffe.html

Java: "ab".repeat(3)
来源：http://hz.zdqjudy.top/gtvwntvrxf.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.feifeiyinyue.top/gtedwxfdid.html

Ruby: "ab" * 3
来源：http://hz.chenzaomai.com/gthibfinwp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhaomingkeji.xyz/gtcphphlzo.html

[E03] 截取子串
来源：http://hz.gogol.net.cn/gtxmjxamkt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.chenlongwang.top/gtylfxpbbk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yangfankeji.com/gtgddtfbga.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.shzxlz.cn/gtwjccqdpz.html

TS:   s.slice(1, 4)
来源：http://hz.ybcxt.top/gtslhgoxaw.html

Java: s.substring(1, 4)
来源：http://hz.chenjidiqi.icu/gthqvaqaoj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yj20258888.top/gtszpdfcau.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xuetiantiany.cn/gttrunqpdm.html

C#:   s.Substring(1, 3)
来源：http://hz.yanxiufei.cn/gtfkvnvntk.html

[E04] 查找子串位置
来源：http://hz.yj20258.top/gtnueagoqv.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hfpthk.cn/gtdscxzyrl.html

PHP:  strpos($s, "x");
来源：http://hz.xziqi.cn/gtnukajxpi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yvedp.cn/gtoubraxpc.html

TS:   s.indexOf("x")
来源：http://hz.yonumen.top/gtxwlntccz.html

Java: s.indexOf("x")
来源：http://hz.guowangkeji.top/gtnonkesdp.html

Go:   strings.Index(s, "x")
来源：http://hz.sufxvd.cn/gtszhnqhzg.html

Ruby: s.index("x")
来源：http://hz.dianchejie.cn/gtxgkbeckt.html

C#:   s.IndexOf("x")
来源：http://hz.ybcxt.top/gtlslwpjci.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.haohaochexian.top/gtstddgxnv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hysaishi.cn/gtmlsjjmov.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hongshengwenyu.top/gtrcgceluo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yvedp.cn/gtuqcdcjnp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.chenzaomai.com/gteetoxein.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhongyouzk.top/gtfodqdzsb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.hongshengwenyu.top/gtixwvccxf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.pycfn.com/gtlqukrlrk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.316326.xyz/gtarpbrbtr.html

[E06] 替换子串
来源：http://hz.nanxuanxn.top/gtuoovinrn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yonumen.top/gtkuqbcdai.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xinyue.icu/gtvaixtokx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yueranfly.top/gtrvhtxuas.html

TS:   s.replaceAll("a", "b")
来源：http://hz.sweek.top/gttdzeosco.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hysaishi.cn/gtruxuoaqf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.cucudq.cn/gtqifwgvqt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jinyuanbaomall.cn/gtancpkseg.html

C#:   s.Replace("a", "b")
来源：http://hz.yonumen.top/gtbpzxivtb.html

[E07] 按分隔符拆分
来源：http://hz.pycfn.com/gtkdsbnocw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jlsjyb.cn/gtftkwajlm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.tian-w.cn/gtmggjhzbo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ivvv.top/gtthtyybpv.html

TS:   s.split(",")
来源：http://hz.mhx1999.top/gtnjphvtvs.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.nanxuanxn.top/gtrvwxsume.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.fzhhl.top/gtegatudtb.html

Ruby: s.split(",");  s.split
来源：http://hz.yonumen.top/gtkzuotuvq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.wangshuangyany.cn/gtehznpnia.html

[E08] 数组按分隔符合并
来源：http://hz.dashuyun.cn/gtqcbodxir.html

Py:   ",".join(items)
来源：http://hz.fengsongda.top/gtlzclkdbw.html

PHP:  implode(",", $items);
来源：http://hz.hongshengwenyu.top/gtfyamfseo.html

JS:   items.join(",")
来源：http://hz.ybcxt.top/gtmexmwwix.html

TS:   items.join(",")
来源：http://hz.zhijiandao.cn/gtcjaqyhoc.html

Java: String.join(",", items)
来源：http://hz.9152youxi.cn/gtytsiqzmu.html

Go:   strings.Join(items, ",")
来源：http://hz.ywan-chungtsiang.top/gtytxkvehc.html

Ruby: items.join(",")
来源：http://hz.hnxiangtu.top/gtqgoynvjy.html

C#:   string.Join(",", items)
来源：http://hz.wangdashe.top/gtlhjtrnac.html

[E09] 去除所有空白字符
来源：http://hz.316326.xyz/gtubjgcwnl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yuanzhike.top/gteynynjpv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shanyushiyangkeji.top/gteqtlyrrj.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.aibaodan.cn/gtysrnyelf.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jinghuilouyu.cn/gtssxnzlhj.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.0kj1m.cn/gtcqkhyblt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.shzxlz.cn/gtrjmqzmiv.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhaomingkeji.xyz/gtcelqywbz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hnqzz.top/gtwkeckwqx.html

[E10] 左侧补零 / 定长填充
来源：http://hz.cheryme.top/gtwxcocszb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.daria6918.cn/gtelhgdixv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yj20258.top/gtawcfejzz.html

JS:   "7".padStart(3, "0")
来源：http://hz.shanyushiyangtech.top/gtjtmvasqw.html

TS:   "7".padStart(3, "0")
来源：http://hz.nwbrower.top/gtliynpjwe.html

Java: String.format("%03d", 7)
来源：http://hz.dashuyun.cn/gtwdmymrzd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.sysykeji.top/gtzhxlsrgb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.aibaodan.cn/gtpgrlerun.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yangfankeji.com/gtbuqreewd.html

[E11] 反转字符串
来源：http://hz.nanxinkj.top/gtzuvabxmx.html

Py:   s[::-1]
来源：http://hz.gogol.net.cn/gtcnyoymts.html

PHP:  strrev($s);
来源：http://hz.hnqzz.top/gtzktyutws.html

JS:   [...s].reverse().join("")
来源：http://hz.xuanzx.com/gtzgipmelt.html

TS:   [...s].reverse().join("")
来源：http://hz.yueranfly.top/gtjjxodpep.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhijiandao.cn/gtxtbqsjzn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.wangdashe.top/gtlmjjcpyx.html

Ruby: s.reverse
来源：http://hz.chenzaomai.com/gtqxppeqob.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yj20258.top/gtrcpcazsq.html

[E12] 统计某字符出现次数
来源：http://hz.pycfn.com/gtixthdrsf.html

Py:   s.count("a")
来源：http://hz.birdmap.top/gtndbgteym.html

PHP:  substr_count($s, "a");
来源：http://hz.yuanzhike.top/gtftaikixp.html

JS:   s.split("a").length - 1
来源：http://hz.hongshengwenyu.top/gtsfukgmcg.html

TS:   s.split("a").length - 1
来源：http://hz.hammf.cn/gtytkqkvoc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ppjwa.cn/gticjszxsf.html

Go:   strings.Count(s, "a")
来源：http://hz.ybcxt.top/gtbrxithoc.html

Ruby: s.count("a")
来源：http://hz.jqgfzy.top/gtbgzvrnxx.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yueranfly.top/gtbtgyusgh.html

[E13] 逐字符遍历
来源：http://hz.gogol.net.cn/gtankjozgj.html

Py:   for ch in s: print(ch)
来源：http://hz.hysaishi.cn/gtvgeclxba.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ehwqpu.com/gtvwbfnjfy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhaomingkeji.xyz/gtdlofgbpp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.feifeiyinyue.top/gtmsvmwerw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.chenzaomai.com/gtyuvldfyu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.tanke756.top/gtnnydxwja.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.dashuyun.cn/gtlllfiryp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.iojbl.cn/gtuacdtyng.html

[E14] URL 编码与 Base64
来源：http://hz.cashguo.top/gtizzvpigf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.sysykeji.top/gtgmemttti.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ydzc1.top/gttlfktlam.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shanyushiyangtech.top/gtfejmuktu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yonumen.top/gtjugigirj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.chenjidiqi.icu/gtafktpeuf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jinqigufen.top/gtboedmtyg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hywenlv.cn/gtyzngxzqy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.shanyushiyangtech.top/gthsarbgjw.html

[E15] HTML 转义 / 反转义
来源：http://hz.hongshengwenyu.top/gtgxhdahft.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jqgfzy.top/gtipawerof.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.feifeiyinyue.top/gtazbtjmnn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.daria6918.cn/gtbojzpwmz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhongyouzk.top/gtacnrszvi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.chenlongwang.top/gtvadhqrhi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zhijiandao.cn/gtatmjypqe.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.tianlin.xyz/gtlgdzbkbx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.sysykeji.top/gtpqmcagmh.html

[E16] 数字千分位
来源：http://hz.ehwqpu.com/gtheljtteo.html

Py:   f"{1234567:,}"
来源：http://hz.meibo888.top/gtoumzhhgn.html

PHP:  number_format(1234567);
来源：http://hz.zycfv.cn/gtponjiszw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yongpay.top/gtvsydhsib.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yongpay.top/gteueuvnan.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.ydjk.org.cn/gtchujgenh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yanxiufei.cn/gtmovdgotr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.wangshuangyany.cn/gtblimbyxv.html

C#:   1234567.ToString("N0")
来源：http://hz.jinqigfzy.top/gtlqsvdtij.html

[E17] 首字母大写
来源：http://hz.haohaochexian.top/gtgrleedqc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.chenjidiqi.icu/gttcmcaenm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.sysykeji.top/gtvidjqkax.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hywenlv.cn/gtcexdunhx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.haohaochexian.top/gtfgkkxswm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.0kj1m.cn/gtehfgpxht.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hongshengwenyu.top/gthgbnbfmk.html

Ruby: s.capitalize
来源：http://hz.yj20258.top/gtmaylaoyo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yonumen.top/gtpedwogxc.html

[E18] 模板占位符替换
来源：http://hz.andypj.xyz/gtbotsrllk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhaomingkeji.xyz/gtisozdwxt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jqgfzy.top/gtuqqiwxgu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.shzxlz.cn/gtffkuxhpc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.aibaodan.cn/gtsvnrzbom.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.guannengcc.top/gtqrlhdlnw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jinqigfzy.top/gtwtsayjba.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.cdnleiting.top/gtafbocula.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.wangshuangyany.cn/gthtamcavl.html

[E19] 多行文本按行拆分
来源：http://hz.shanyushiyangkeji.top/gtyspghxtx.html

Py:   s.splitlines()
来源：http://hz.shzxlz.cn/gtlmupgnck.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yuanzhike.top/gtkddvvvpn.html

JS:   s.split(/\r?\n/)
来源：http://hz.feifeiyinyue.top/gtzvfebfrw.html

TS:   s.split(/\r?\n/)
来源：http://hz.smart0.xyz/gtpiyqpsgp.html

Java: s.lines().toList()
来源：http://hz.jqgfzy.top/gtnqtzhlle.html

Go:   strings.Split(s, "\n")
来源：http://hz.jyoumei.cn/gtyxrdzrbt.html

Ruby: s.lines
来源：http://hz.nanxinkj.top/gtotlduyfq.html

C#:   s.Split('\n')
来源：http://hz.tanke756.top/gtrrtmcclp.html

[E20] 判断字符串是否为空
来源：http://hz.tanke756.top/gtynizlbhw.html

Py:   if not s:
来源：http://hz.guowangkeji.top/gtxxuhbuve.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hammf.cn/gtgcgzwhfo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xziqi.cn/gtecmqgigz.html

TS:   if (s === "") {}
来源：http://hz.jqgfzy.top/gtgcfqrzni.html

Java: if (s.isEmpty()) {}
来源：http://hz.nanxinkj.top/gtbytokewi.html

Go:   if s == "" {}
来源：http://hz.xinyue.icu/gttesljjhl.html

Ruby: if s.empty?
来源：http://hz.gzhubu.top/gtvenvhtvs.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yj202588.top/gtjhlnxljj.html

[E21] 超长截断加省略号
来源：http://hz.xuetiantiany.cn/gteqamfdya.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ybcxt.top/gttemzqpyz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.snrcjt.cn/gtlbhezfeu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinyuanbaomall.cn/gtkqgyczzw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sufxvd.cn/gtozbslbji.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.nwbrower.top/gthnwwjlbo.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.52xcode.cn/gthwuwtkxy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.xziqi.cn/gtpazhsosd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.tanke756.top/gtgrjonoro.html

[E22] 字节长度与字符长度
来源：http://hz.shanyushiyangtech.top/gtzkyhghsr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ydjk.org.cn/gteebyuwzd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.wangdashe.top/gtckyaugiu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhaomingkeji.xyz/gtipxmypox.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hfpthk.cn/gtmbwsqwtk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.gaohongyu789.top/gtjzsukwmo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ywan-chungtsiang.top/gtvwkcgkvv.html

Ruby: s.bytesize;  s.length
来源：http://hz.ppjwa.cn/gttownwdfg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hammf.cn/gttipktihz.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtkcxgjlma.html

F. 文件与目录
来源：http://hz.yonumen.top/gtitwbbcjg.html

================================================================================
来源：http://hz.cashguo.top/gtcoagifkl.html

[F01] 读取整个文件
来源：http://hz.xingfuxueyuan.xyz/gtwufsixko.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.pengpengdd.cyou/gtsvwkvhgs.html

PHP:  file_get_contents("a.txt");
来源：http://hz.tian-w.cn/gtbsspqfsa.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.shangyingyoupin.top/gtiydworin.html


<!-- 参考信息 -->