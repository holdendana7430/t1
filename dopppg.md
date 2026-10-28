代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hysaishi.cn/gtbkwqkcbd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gaohongyu789.top/gtuuovkren.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ywan-chungtsiang.top/gtwdesrqde.html

Go:   // 手写循环累加
来源：http://hz.jinqigufen.top/gtfueweguu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.nanxinkj.top/gtwzkbplme.html

C#:   list.Sum();  list.Average()
来源：http://hz.mhx1999.top/gthapbtyvl.html

[D17] 最大值与最小值
来源：http://hz.jinqigfzy.top/gtgnxxalqh.html

Py:   max(arr);  min(arr)
来源：http://hz.iojbl.cn/gtqibwavjr.html

PHP:  max($arr);  min($arr);
来源：http://hz.nwbrower.top/gtqofnsxxs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.cheryme.top/gtcagympbh.html

TS:   Math.max(...arr);
来源：http://hz.svipenyu.cn/gtcpcgpxhk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jinqigufen.top/gtxncdauji.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hammf.cn/gtlibfvorm.html

Ruby: arr.max;  arr.min
来源：http://hz.andypj.xyz/gturrgwopz.html

C#:   list.Max();  list.Min()
来源：http://hz.ppjwa.cn/gtrgjjcurh.html

[D18] 扁平化嵌套数组
来源：http://hz.xziqi.cn/gtqqybcjan.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yangfankeji.com/gtonsaoqpj.html

PHP:  array_merge(...$nested);
来源：http://hz.aibaodan.cn/gtscouetcz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhongyouzk.top/gtgrtmmqzr.html

TS:   nested.flat();
来源：http://hz.zhoulong.xyz/gtguqjpmfe.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ydjk.org.cn/gtujxjqxjl.html

Go:   // 手写双层循环
来源：http://hz.aizwys.cn/gtkcfstmlk.html

Ruby: nested.flatten
来源：http://hz.andypj.xyz/gtajfipjfb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xingfuxueyuan.xyz/gtzaojiuqs.html

[D19] 按字段分组
来源：http://hz.dashuyun.cn/gtaczchumz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.cdnleiting.top/gtoyashvux.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yvedp.cn/gtsvpiwhxd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yueranfly.top/gtvzbdpldf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hysaishi.cn/gtegwmdofd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhaomingkeji.xyz/gtwyoslrhm.html

Go:   // 手写 map[string][]T
来源：http://hz.jinqigufen.top/gtssuirzkm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.gzhubu.top/gtcukyfurs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.tianlin.xyz/gtoxaszioy.html

[D20] 统计每个元素出现次数
来源：http://hz.fengsongda.top/gtftcazvts.html

Py:   Counter(arr)
来源：http://hz.xylfe.cn/gtwrrzalon.html

PHP:  array_count_values($arr);
来源：http://hz.jinghuilouyu.cn/gtzbruqked.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xziqi.cn/gtrlremicm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.meibo888.top/gtbcififtl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.0kj1m.cn/gtsgwnveia.html

Go:   // 手写 map[T]int
来源：http://hz.xuetiantiany.cn/gtyjzvqtbp.html

Ruby: arr.tally
来源：http://hz.daria6918.cn/gtfeuqpven.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hammf.cn/gttglpllbq.html

[D21] 判断是否包含某元素
来源：http://hz.fzhhl.top/gtkdmliism.html

Py:   x in arr
来源：http://hz.zhengqikj.top/gtkkmrpspc.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jinyuanbaomall.cn/gtnzquzoah.html

JS:   arr.includes(x)
来源：http://hz.yuanzhike.top/gtpkeukdnf.html

TS:   arr.includes(x)
来源：http://hz.zhaomingkeji.xyz/gtndudubmr.html

Java: list.contains(x)
来源：http://hz.ydjk.org.cn/gtqhpjdrfl.html

Go:   slices.Contains(arr, x)
来源：http://hz.gaohongyu789.top/gtopteoovh.html

Ruby: arr.include?(x)
来源：http://hz.nanxuanxn.top/gtlkcnslsf.html

C#:   list.Contains(x)
来源：http://hz.zhongyouzk.top/gtaylqvxls.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yueranfly.top/gttqytwfwn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.svipenyu.cn/gtbqonmfbr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jinqigufen.top/gtaqbwocjb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.52xcode.cn/gtxixrskmo.html

TS:   [...arr];
来源：http://hz.cqqwz.cn/gtifkubwec.html

Java: new ArrayList<>(list);
来源：http://hz.ydzc1.top/gtjyidbuhz.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.iojbl.cn/gtnzbfqtuw.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zycfv.cn/gtqpjhvegx.html

C#:   new List<int>(list);
来源：http://hz.meibo888.top/gtercrzvnf.html

[D23] reduce 累积计算
来源：http://hz.chenlongwang.top/gtduznmthf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hongshengwenyu.top/gtgomevagy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.mhx1999.top/gtdioxmpdc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.tianlin.xyz/gtsvxyqlvm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.nanxuanxn.top/gthjkyghka.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.redwolf501.top/gtaktblese.html

Go:   // 手写循环
来源：http://hz.shanyushiyangkeji.top/gtigzyoafr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.andypj.xyz/gtzoemsqcc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.xylfe.cn/gtcdzxsijq.html

[D24] 字典 / Map 基本操作
来源：http://hz.hongshengwenyu.top/gtslybmgws.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.svipenyu.cn/gtpttokczx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zhongyouzk.top/gtwhgxhrgz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhengqikj.top/gtlzldqbxj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.havefunace.top/gtsttozvkk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.shuidangran.top/gtvtcijrci.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jinqigufen.top/gtmvlgoihf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.pengpengdd.cyou/gtlwxcpmca.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.birdmap.top/gtyitsjtpm.html

[D25] Set 集合去重与交并差
来源：http://hz.zhijiandao.cn/gtnoijakgn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.quarkkingdee.top/gtdivkydio.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hfpthk.cn/gtlatloube.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.xylfe.cn/gtvltfuyxa.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yj20258888.top/gtrqqijfpi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.shanyushiyangtech.top/gtfsxubzov.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.chenjidiqi.icu/gtpwktgpef.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jyoumei.cn/gternaytat.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhiwuduotai.top/gtfkfhwnhx.html

[D26] 数组转字符串
来源：http://hz.nwbrower.top/gttzrgsccx.html

Py:   ", ".join(map(str, arr))
来源：http://hz.vqdsnc.cn/gtzssofhno.html

PHP:  implode(", ", $arr);
来源：http://hz.meibo888.top/gttbawcamm.html

JS:   arr.join(", ")
来源：http://hz.zhixingplan.top/gtxeefeaea.html

TS:   arr.join(", ")
来源：http://hz.ydzc1.top/gtwohvmwsr.html

Java: String.join(", ", list)
来源：http://hz.nwbrower.top/gtwchuiler.html

Go:   strings.Join(strs, ", ")
来源：http://hz.316326.xyz/gtdarjgpyd.html

Ruby: arr.join(", ")
来源：http://hz.fengsongda.top/gtquiizrns.html

C#:   string.Join(", ", list)
来源：http://hz.9152youxi.cn/gtquiprghn.html

================================================================================
来源：http://hz.tianlin.xyz/gtzaajvqtz.html

E. 字符串处理
来源：http://hz.gzhubu.top/gtydejmyul.html

================================================================================
来源：http://hz.0kj1m.cn/gtfjzrsqaz.html

[E01] 拼接字符串
来源：http://hz.chenzaomai.com/gtmupsuxsy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhongyouzk.top/gtknyymolx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhaomingkeji.xyz/gtprcrfkto.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.9152youxi.cn/gtbejzdmmn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gzhubu.top/gtzcxaeeda.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.cdnleiting.top/gtzesnsczy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.cqqwz.cn/gtshltggyk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.cheryme.top/gtguqoajgl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.shanyushiyangkeji.top/gtuktnnnyt.html

[E02] 重复字符串
来源：http://hz.zhaomingkeji.xyz/gtduiuectj.html

Py:   "ab" * 3
来源：http://hz.kuanghao11.cn/gtteseuknz.html

PHP:  str_repeat("ab", 3);
来源：http://hz.wangdashe.top/gtepzgwewv.html

JS:   "ab".repeat(3)
来源：http://hz.ivvv.top/gtqmljazpp.html

TS:   "ab".repeat(3)
来源：http://hz.yanxiufei.cn/gtozgkcvzv.html

Java: "ab".repeat(3)
来源：http://hz.yj20258888.top/gtkmhlmjlc.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ppjwa.cn/gtvrhgjxtv.html

Ruby: "ab" * 3
来源：http://hz.mhx1999.top/gtguuietwn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.guannengcc.top/gtixasafgz.html

[E03] 截取子串
来源：http://hz.chenlongwang.top/gtmamxascw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.xuanzx.com/gtckxxnhyq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhiwuduotai.top/gtpghfvhos.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhixingplan.top/gtxqdzstyh.html

TS:   s.slice(1, 4)
来源：http://hz.havefunace.top/gteqafojhe.html

Java: s.substring(1, 4)
来源：http://hz.zhiwuduotai.top/gtyskbsoit.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.shuidangran.top/gtofrofhum.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.ivvv.top/gtimcgqzgb.html

C#:   s.Substring(1, 3)
来源：http://hz.ppjwa.cn/gtpconrcod.html

[E04] 查找子串位置
来源：http://hz.ybcxt.top/gticrxdicq.html

Py:   s.find("x");  s.index("x")
来源：http://hz.nanxinkj.top/gtusfkcjbx.html

PHP:  strpos($s, "x");
来源：http://hz.yangfankeji.com/gtlulxtqee.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yueranfly.top/gtofvvdnsa.html

TS:   s.indexOf("x")
来源：http://hz.cqqwz.cn/gtvdususbd.html

Java: s.indexOf("x")
来源：http://hz.gaohongyu789.top/gtvjjthtjn.html

Go:   strings.Index(s, "x")
来源：http://hz.gaohongyu789.top/gtarftstkt.html

Ruby: s.index("x")
来源：http://hz.hnxiangtu.top/gthmamnwwz.html

C#:   s.IndexOf("x")
来源：http://hz.hywenlv.cn/gtcbbgamjl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.chenlongwang.top/gtbjtqrpgn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yuxming.cn/gtcdslgpsb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ivvv.top/gtzxpuohzr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.dianchejie.cn/gtrnwgsjiu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.xylfe.cn/gtlgkrnoym.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.snrcjt.cn/gtsfpmddsr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.feifeiyinyue.top/gtkvtdijmi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.daria6918.cn/gtipsutqwh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.haohaochexian.top/gtanbhvrrg.html

[E06] 替换子串
来源：http://hz.meibo888.top/gtrtjvnyqa.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.pengpengdd.cyou/gtkdhwzddb.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.gzhubu.top/gtykjkepsj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinqigfzy.top/gtwjvupqbl.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jinghuilouyu.cn/gtksurgcge.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhongyouzk.top/gtvtqpwaoo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jyoumei.cn/gtiexextrg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.vqdsnc.cn/gtbyzisstc.html

C#:   s.Replace("a", "b")
来源：http://hz.gaohongyu789.top/gtaopigxlo.html

[E07] 按分隔符拆分
来源：http://hz.smart0.xyz/gtoldzjydb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hysaishi.cn/gtrkzxrwzu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cucudq.cn/gtpqdytavu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.cucudq.cn/gtgneibrms.html

TS:   s.split(",")
来源：http://hz.quarkkingdee.top/gtapqkzhya.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.xingfuxueyuan.xyz/gtexacjyna.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jlsjyb.cn/gtqvbiotfx.html

Ruby: s.split(",");  s.split
来源：http://hz.daxiang520.top/gtsftlqgwe.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.chenjidiqi.icu/gtbiqxebct.html

[E08] 数组按分隔符合并
来源：http://hz.xylfe.cn/gtlwydkmat.html

Py:   ",".join(items)
来源：http://hz.yuxming.cn/gtwgmixxqy.html

PHP:  implode(",", $items);
来源：http://hz.iojbl.cn/gtftcntplf.html

JS:   items.join(",")
来源：http://hz.gogol.net.cn/gtgiuxjtvg.html

TS:   items.join(",")
来源：http://hz.zhengqikj.top/gtzmrkdypg.html

Java: String.join(",", items)
来源：http://hz.ybcxt.top/gtxmmfbmxe.html

Go:   strings.Join(items, ",")
来源：http://hz.zhongyouzk.top/gtcqxjehbg.html

Ruby: items.join(",")
来源：http://hz.nwbrower.top/gtktstyjhb.html

C#:   string.Join(",", items)
来源：http://hz.hongshengwenyu.top/gtdqnksdeh.html

[E09] 去除所有空白字符
来源：http://hz.jqgufenzy.top/gtucpdegco.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.andypj.xyz/gteiefllkp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.guannengcc.top/gtediujggo.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.shangyingyoupin.top/gtbnjnrlxu.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jyoumei.cn/gtunpaskog.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.bjfxy.top/gtdpavjfcq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jinqigfzy.top/gtaqjxyqek.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.c1oappe.top/gtvxwmzpxz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yuanzhike.top/gthxewvdrc.html

[E10] 左侧补零 / 定长填充
来源：http://hz.shanyushiyangtech.top/gtxpuukiiz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.chenzaomai.com/gttyvvquav.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.mhx1999.top/gtgjcpodkm.html

JS:   "7".padStart(3, "0")
来源：http://hz.chenzaomai.com/gtxykyiczk.html

TS:   "7".padStart(3, "0")
来源：http://hz.gotoacloud.top/gtxezojxnw.html

Java: String.format("%03d", 7)
来源：http://hz.havefunace.top/gtezarpoav.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yanxiufei.cn/gttpoasaxc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.cdnleiting.top/gtehnskpwm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shanyushiyangkeji.top/gthjfpemcc.html

[E11] 反转字符串
来源：http://hz.zhijiandao.cn/gtydwszglw.html

Py:   s[::-1]
来源：http://hz.gotoacloud.top/gtqvpkocwf.html

PHP:  strrev($s);
来源：http://hz.jlsjyb.cn/gtaumnarts.html

JS:   [...s].reverse().join("")
来源：http://hz.sysykeji.top/gtdhrgfrbi.html

TS:   [...s].reverse().join("")
来源：http://hz.haohaochexian.top/gtymnjovim.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jqgufenzy.top/gtzwyfwgrb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.316326.xyz/gtaufysyql.html

Ruby: s.reverse
来源：http://hz.nwbrower.top/gtposbspfg.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.wangshuangyany.cn/gtkgvxnztg.html

[E12] 统计某字符出现次数
来源：http://hz.dianchejie.cn/gtvsbjlnjh.html

Py:   s.count("a")
来源：http://hz.c1oappe.top/gtrmxjranv.html

PHP:  substr_count($s, "a");
来源：http://hz.52xcode.cn/gtizfhmans.html

JS:   s.split("a").length - 1
来源：http://hz.cqqwz.cn/gtjfcxydyh.html

TS:   s.split("a").length - 1
来源：http://hz.nanxuanxn.top/gtyfzrfxkt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xuetiantiany.cn/gtlvwrbkty.html

Go:   strings.Count(s, "a")
来源：http://hz.zhiwuduotai.top/gtdrrhcmzg.html

Ruby: s.count("a")
来源：http://hz.yuanzhike.top/gtoulwgcnz.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jqgfzy.top/gtukahepcb.html

[E13] 逐字符遍历
来源：http://hz.52xcode.cn/gtnfkvuhvu.html

Py:   for ch in s: print(ch)
来源：http://hz.pengpengdd.cyou/gtfqkcsujg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.smart0.xyz/gttnlfpikf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhaomingkeji.xyz/gtogswmelk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.wangshuangyany.cn/gtiortxqky.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hnqzz.top/gtlzrgdpgu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.smart0.xyz/gtaxuatloa.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.sysykeji.top/gtyxpmuqws.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.sxryk.cn/gtqqiaiovu.html

[E14] URL 编码与 Base64
来源：http://hz.cheryme.top/gtqgaysqvx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ydzc1.top/gtalhuzghj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.316326.xyz/gtqspshvqa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ybcxt.top/gtxxvcfiby.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.birdmap.top/gtwrrsiojl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.xuanzx.com/gtupjokeja.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.gogol.net.cn/gtwoegylvz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ehwqpu.com/gttvchrkvy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.iojbl.cn/gtaxxzlfkk.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhoulong.xyz/gtojchfhjs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhixingplan.top/gtobkiecvh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.nanxinkj.top/gtpswvylok.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.tian-w.cn/gtjdtqpwst.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.nwbrower.top/gtxiwanply.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.cqqwz.cn/gtkqdgrbwh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jqgfzy.top/gtaayujmxs.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.cheryme.top/gtmakaejho.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.cdnleiting.top/gtljsngfuo.html

[E16] 数字千分位
来源：http://hz.zhaomingkeji.xyz/gtnfmxmwrh.html

Py:   f"{1234567:,}"
来源：http://hz.nwbrower.top/gtjqaghxfp.html

PHP:  number_format(1234567);
来源：http://hz.hongshengwenyu.top/gtwidisdgs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.sxryk.cn/gtizhquwql.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.316326.xyz/gtkxsdwewk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yonumen.top/gtsxviszkw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.cheryme.top/gtmldzofee.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cashguo.top/gtsqfpbuys.html

C#:   1234567.ToString("N0")
来源：http://hz.zhaomingkeji.xyz/gtglbfyuyk.html

[E17] 首字母大写
来源：http://hz.hysaishi.cn/gtrbngxtxw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.ywan-chungtsiang.top/gtnilcjqwk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jinyuanbaomall.cn/gtqotfxmnx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhaomingkeji.xyz/gtmprvprcv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yanxiufei.cn/gtfperfbzz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yvedp.cn/gtgnwbeqjj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hammf.cn/gtxxjeuetf.html

Ruby: s.capitalize
来源：http://hz.snrcjt.cn/gteilsxetd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.sxryk.cn/gtvvlvbkyi.html

[E18] 模板占位符替换
来源：http://hz.xziqi.cn/gtbtunlaen.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.52xcode.cn/gtcdrvpepm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.svipenyu.cn/gtekfzvnqt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.pycfn.com/gtvbctusqa.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hnxiangtu.top/gtjibmjlfd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yueranfly.top/gtpaxhckxg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jinqigfzy.top/gtttfyuprf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yongpay.top/gtepohzlkx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.cucudq.cn/gtsihayyhn.html

[E19] 多行文本按行拆分
来源：http://hz.hongshengwenyu.top/gtyraggoqi.html

Py:   s.splitlines()
来源：http://hz.yj202588.top/gtwusrerup.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.0kj1m.cn/gttheupyet.html

JS:   s.split(/\r?\n/)
来源：http://hz.hywenlv.cn/gtfumpyaci.html

TS:   s.split(/\r?\n/)
来源：http://hz.shuidangran.top/gtmbsijaab.html

Java: s.lines().toList()
来源：http://hz.hnxiangtu.top/gtwcmlzvhy.html

Go:   strings.Split(s, "\n")
来源：http://hz.52xcode.cn/gtkfmetwdo.html

Ruby: s.lines
来源：http://hz.yvedp.cn/gtdmngwhpt.html

C#:   s.Split('\n')
来源：http://hz.fzhhl.top/gtgbixyzvl.html

[E20] 判断字符串是否为空
来源：http://hz.zycfv.cn/gtcjxoghxr.html

Py:   if not s:
来源：http://hz.nanxuanxn.top/gtmlktochr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.pengpengdd.cyou/gtpkvqadzc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.shangyingyoupin.top/gtnnyzqyfp.html

TS:   if (s === "") {}
来源：http://hz.yuxming.cn/gtyxfcdhpj.html

Java: if (s.isEmpty()) {}
来源：http://hz.chenzaomai.com/gthogoglxs.html

Go:   if s == "" {}
来源：http://hz.gogol.net.cn/gtwfkioeya.html

Ruby: if s.empty?
来源：http://hz.daria6918.cn/gtzixmfwfk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cheryme.top/gtzgdtpzio.html

[E21] 超长截断加省略号
来源：http://hz.hnqzz.top/gtownusqiw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.vqdsnc.cn/gtwsvdbikl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jlsjyb.cn/gtvogwkove.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.meibo888.top/gtzqdkyvwo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ydzc1.top/gtjxqvsivr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jinghuilouyu.cn/gtdbxgtyok.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhixingplan.top/gtfczwrotd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.wangshuangyany.cn/gtydqrbgls.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.kuanghao11.cn/gtlhnjsniw.html

[E22] 字节长度与字符长度
来源：http://hz.jqgufenzy.top/gtgqnogslr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yuanzhike.top/gthoifwibt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.pycfn.com/gtxleqdrln.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xziqi.cn/gtuqfcnhgj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jlsjyb.cn/gtkukxguyv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yonumen.top/gtuytyolak.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yueranfly.top/gtukaerjds.html

Ruby: s.bytesize;  s.length
来源：http://hz.fengsongda.top/gtayioirhc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.wangdashe.top/gtelsfhqhd.html

================================================================================
来源：http://hz.cashguo.top/gtejfvbpin.html

F. 文件与目录
来源：http://hz.jqgufenzy.top/gtjsqxmoxo.html

================================================================================
来源：http://hz.cashguo.top/gtflsunvee.html


<!-- 参考信息 -->