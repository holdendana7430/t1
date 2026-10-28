代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jlsjyb.cn/gtgninnqrg.html

Go:   // 手写循环
来源：http://hz.sxryk.cn/gtehpbsbeh.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.9152youxi.cn/gtggbrlvhw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.daria6918.cn/gtzigklbol.html

[D15] 去重
来源：http://hz.mhx1999.top/gtelzwuvzj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.birdmap.top/gtxjmiflnj.html

PHP:  array_unique($arr);
来源：http://hz.cashguo.top/gtxcpuwadh.html

JS:   [...new Set(arr)]
来源：http://hz.jiagoushi.top/gtcismnvdn.html

TS:   [...new Set(arr)]
来源：http://hz.9152youxi.cn/gtxruukmww.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.mhx1999.top/gthzbcvvcr.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yanxiufei.cn/gteozlkdqb.html

Ruby: arr.uniq
来源：http://hz.cdnleiting.top/gtyyucoiow.html

C#:   list.Distinct().ToList()
来源：http://hz.jqgfzy.top/gtspazpltc.html

[D16] 求和与平均值
来源：http://hz.shzxlz.cn/gturvxnubs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.sweek.top/gtydlxjvjx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.quarkkingdee.top/gtgvucxxvs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shanyushiyangkeji.top/gtjxtbrnrr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xuetiantiany.cn/gtwiccnmmx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jinghuilouyu.cn/gtmcktsvam.html

Go:   // 手写循环累加
来源：http://hz.shanyushiyangtech.top/gtixhklyin.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yuxming.cn/gtsykwyegj.html

C#:   list.Sum();  list.Average()
来源：http://hz.nanxinkj.top/gtflwctsmb.html

[D17] 最大值与最小值
来源：http://hz.guannengcc.top/gtszptudie.html

Py:   max(arr);  min(arr)
来源：http://hz.chenjidiqi.icu/gtyqdvzlnl.html

PHP:  max($arr);  min($arr);
来源：http://hz.nanxinkj.top/gtjesvukll.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.birdmap.top/gtfqlatybf.html

TS:   Math.max(...arr);
来源：http://hz.zhijiandao.cn/gtxzaeejpl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jinqigfzy.top/gtxndrlark.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.shanyushiyangkeji.top/gtgutwsfmu.html

Ruby: arr.max;  arr.min
来源：http://hz.gogol.net.cn/gtmyzpgmbf.html

C#:   list.Max();  list.Min()
来源：http://hz.kuanghao11.cn/gtgdwkgihb.html

[D18] 扁平化嵌套数组
来源：http://hz.havefunace.top/gtbzctural.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.aibaodan.cn/gtfwxwltra.html

PHP:  array_merge(...$nested);
来源：http://hz.guowangkeji.top/gtsqvpviqe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.cdnleiting.top/gtloriokoc.html

TS:   nested.flat();
来源：http://hz.chenjidiqi.icu/gtkbsuymmb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.andypj.xyz/gtpqynlfxh.html

Go:   // 手写双层循环
来源：http://hz.jinqigufen.top/gthqbmnueb.html

Ruby: nested.flatten
来源：http://hz.c1oappe.top/gtrtjyaurd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.shangyingyoupin.top/gtioqiuobf.html

[D19] 按字段分组
来源：http://hz.gogol.net.cn/gtdrstbqqg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.9152youxi.cn/gtfbuxtljh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhoulong.xyz/gtizagsddg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jqgfzy.top/gtgyzttcld.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.nwbrower.top/gtzbzfxmpo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ywan-chungtsiang.top/gtlozdbevc.html

Go:   // 手写 map[string][]T
来源：http://hz.aizwys.cn/gtfkbkkkhj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ivvv.top/gtilqftkhz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.feifeiyinyue.top/gtjcquylhk.html

[D20] 统计每个元素出现次数
来源：http://hz.quarkkingdee.top/gtlebwxafc.html

Py:   Counter(arr)
来源：http://hz.jianghu66.top/gthdixkioo.html

PHP:  array_count_values($arr);
来源：http://hz.jyoumei.cn/gttinhzpcv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xinyue.icu/gtszrzrzry.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yueranfly.top/gtsfkctsak.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.chenzaomai.com/gtrrxztavn.html

Go:   // 手写 map[T]int
来源：http://hz.chenjidiqi.icu/gtcnhwopmu.html

Ruby: arr.tally
来源：http://hz.shzxlz.cn/gtyotqkjnx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.tianlin.xyz/gtdoqiayuo.html

[D21] 判断是否包含某元素
来源：http://hz.jinqigufen.top/gtotcwhevt.html

Py:   x in arr
来源：http://hz.gogol.net.cn/gtyxnxjmwa.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jinghuilouyu.cn/gtoeupcukc.html

JS:   arr.includes(x)
来源：http://hz.fengsongda.top/gtaqqgtwth.html

TS:   arr.includes(x)
来源：http://hz.yj20258.top/gtbpasqxja.html

Java: list.contains(x)
来源：http://hz.tanke756.top/gtioojuwpl.html

Go:   slices.Contains(arr, x)
来源：http://hz.ppjwa.cn/gtryzxabwd.html

Ruby: arr.include?(x)
来源：http://hz.wangdashe.top/gtygxsdibv.html

C#:   list.Contains(x)
来源：http://hz.hywenlv.cn/gtbifttahe.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jiagoushi.top/gtkzbevobw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.guannengcc.top/gtdjokkoly.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.cqqwz.cn/gtulrqzyis.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.shuidangran.top/gtepnajsgm.html

TS:   [...arr];
来源：http://hz.jinyuanbaomall.cn/gtrzfylwrb.html

Java: new ArrayList<>(list);
来源：http://hz.ywan-chungtsiang.top/gtnarphdlg.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.redwolf501.top/gtakueivqb.html

Ruby: arr.dup;  arr.clone
来源：http://hz.fengsongda.top/gtzcludttr.html

C#:   new List<int>(list);
来源：http://hz.mhx1999.top/gtjztlbkrb.html

[D23] reduce 累积计算
来源：http://hz.fengsongda.top/gtlegvasjw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.xuetiantiany.cn/gtsrycfpmj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yj20258.top/gtwzcnospm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.guowangkeji.top/gtkmfilqxv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.kuanghao11.cn/gtynqmbnhb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.xinyue.icu/gttwnojgyf.html

Go:   // 手写循环
来源：http://hz.daria6918.cn/gtwdpmmeor.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhijiandao.cn/gtkkgqfhtj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.wangshuangyany.cn/gturjblgts.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhijiandao.cn/gtbpdixxup.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ywan-chungtsiang.top/gthlgylgro.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.c1oappe.top/gtqmduhnlz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ybcxt.top/gtjbbhwfkh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.tanke756.top/gtwgmjepnm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.fengsongda.top/gtmafjzdtv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhixingplan.top/gtiqceuarl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.redwolf501.top/gttjjzxyke.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.feifeiyinyue.top/gtmumodjln.html

[D25] Set 集合去重与交并差
来源：http://hz.gotoacloud.top/gtgdqfpfbg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.316326.xyz/gtivjcwscw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.shanyushiyangkeji.top/gtyubmfaew.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.cucudq.cn/gtxlafwwtu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.c1oappe.top/gtcrplkgii.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yangfankeji.com/gtdipidsvw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.sysykeji.top/gtpoqfvyib.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.nanxuanxn.top/gtrxckhxtj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.ydzc1.top/gtjyngiasj.html

[D26] 数组转字符串
来源：http://hz.yj202588.top/gtyvpdshzx.html

Py:   ", ".join(map(str, arr))
来源：http://hz.wangshuangyany.cn/gtnzxgnrez.html

PHP:  implode(", ", $arr);
来源：http://hz.vqdsnc.cn/gtfonztdli.html

JS:   arr.join(", ")
来源：http://hz.jiagoushi.top/gtiqipofja.html

TS:   arr.join(", ")
来源：http://hz.cdnleiting.top/gtnykszjky.html

Java: String.join(", ", list)
来源：http://hz.andypj.xyz/gtbtaxqigm.html

Go:   strings.Join(strs, ", ")
来源：http://hz.bjfxy.top/gtzpdmfzke.html

Ruby: arr.join(", ")
来源：http://hz.vqdsnc.cn/gtezvhhzij.html

C#:   string.Join(", ", list)
来源：http://hz.havefunace.top/gtlxrnpcwf.html

================================================================================
来源：http://hz.nanxuanxn.top/gtrpinslfg.html

E. 字符串处理
来源：http://hz.gogol.net.cn/gthpgdzxxa.html

================================================================================
来源：http://hz.jinqigfzy.top/gtgxuwpjnr.html

[E01] 拼接字符串
来源：http://hz.sufxvd.cn/gthaxsqysj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.aibaodan.cn/gtcdctwyba.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.xylfe.cn/gtcvqmjlnn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yonumen.top/gtlcdzuwfx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xingfuxueyuan.xyz/gtpetypmia.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yonumen.top/gtdebxfumo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.quarkkingdee.top/gtqxmdbwan.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jinghuilouyu.cn/gteedsgpsv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhengqikj.top/gthnavrgoe.html

[E02] 重复字符串
来源：http://hz.zhiwuduotai.top/gtokzbawqn.html

Py:   "ab" * 3
来源：http://hz.cashguo.top/gtdyhwlqua.html

PHP:  str_repeat("ab", 3);
来源：http://hz.tianlin.xyz/gtoiwrafio.html

JS:   "ab".repeat(3)
来源：http://hz.tian-w.cn/gtsiddifuo.html

TS:   "ab".repeat(3)
来源：http://hz.gogol.net.cn/gtjlxzmcan.html

Java: "ab".repeat(3)
来源：http://hz.zhaomingkeji.xyz/gtottlkibw.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhengqikj.top/gtynoczuze.html

Ruby: "ab" * 3
来源：http://hz.havefunace.top/gteokknajh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yueranfly.top/gtaqegsyep.html

[E03] 截取子串
来源：http://hz.xinyue.icu/gteunjtbko.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jinqigufen.top/gtvbcwncdd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.shuidangran.top/gtmkbrypap.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.ywan-chungtsiang.top/gtiewhtalq.html

TS:   s.slice(1, 4)
来源：http://hz.xziqi.cn/gtpucqrpkz.html

Java: s.substring(1, 4)
来源：http://hz.sufxvd.cn/gtbnydrsde.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hnqzz.top/gtakiesxdn.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jiagoushi.top/gthltymban.html

C#:   s.Substring(1, 3)
来源：http://hz.zhaomingkeji.xyz/gtbgqhluvg.html

[E04] 查找子串位置
来源：http://hz.cashguo.top/gtjaoxknbc.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yanxiufei.cn/gtgeodbpxu.html

PHP:  strpos($s, "x");
来源：http://hz.daria6918.cn/gtjrqllxpr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ywan-chungtsiang.top/gtquirvdrs.html

TS:   s.indexOf("x")
来源：http://hz.haohaochexian.top/gtdijgjrew.html

Java: s.indexOf("x")
来源：http://hz.xziqi.cn/gtfmkvrnqc.html

Go:   strings.Index(s, "x")
来源：http://hz.gaohongyu789.top/gtpitxtnse.html

Ruby: s.index("x")
来源：http://hz.haohaochexian.top/gtmrcsnfwd.html

C#:   s.IndexOf("x")
来源：http://hz.jinghuilouyu.cn/gtnjztvzts.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.gogol.net.cn/gtzldcdwlz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hnxiangtu.top/gttsjcaewj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jinqigfzy.top/gtltrpfcgg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.c1oappe.top/gtatcljevi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.feifeiyinyue.top/gtnrghxtft.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hongshengwenyu.top/gtfsdxjlbw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.meibo888.top/gthsexsejh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.meibo888.top/gtjlbzrhzx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.feifeiyinyue.top/gtpkpmwmgs.html

[E06] 替换子串
来源：http://hz.meibo888.top/gtcnsojjxo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.mhx1999.top/gtymioippr.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yvedp.cn/gtrwxckxog.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jqgufenzy.top/gtzatuigkr.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhengqikj.top/gtjdxedxyz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cashguo.top/gtlruszinz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.redwolf501.top/gtdnickjwv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.hongshengwenyu.top/gtmnpoedij.html

C#:   s.Replace("a", "b")
来源：http://hz.fzhhl.top/gtjpcusrbx.html

[E07] 按分隔符拆分
来源：http://hz.hammf.cn/gtpngzzzsx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hammf.cn/gtacfwahgf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.snrcjt.cn/gtxsrrnupx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.daxiang520.top/gtorvsokbg.html

TS:   s.split(",")
来源：http://hz.jiagoushi.top/gtsvlpronn.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.guannengcc.top/gtogzkerzb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.hysaishi.cn/gtetlmnuxh.html

Ruby: s.split(",");  s.split
来源：http://hz.jinqigufen.top/gtkwvadrtn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yj202588.top/gtpsgvxvat.html

[E08] 数组按分隔符合并
来源：http://hz.guowangkeji.top/gtrfmkwgeu.html

Py:   ",".join(items)
来源：http://hz.ydzc1.top/gtveazumut.html

PHP:  implode(",", $items);
来源：http://hz.xylfe.cn/gtuowlpygl.html

JS:   items.join(",")
来源：http://hz.vqdsnc.cn/gtvkfxrxun.html

TS:   items.join(",")
来源：http://hz.zdqjudy.top/gtozklqwly.html

Java: String.join(",", items)
来源：http://hz.daria6918.cn/gttjthntsv.html

Go:   strings.Join(items, ",")
来源：http://hz.gzhubu.top/gtkhjncpks.html

Ruby: items.join(",")
来源：http://hz.9152youxi.cn/gtmssrlswl.html

C#:   string.Join(",", items)
来源：http://hz.pengpengdd.cyou/gtcxoyhtor.html

[E09] 去除所有空白字符
来源：http://hz.yvedp.cn/gtgyoajyir.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.guannengcc.top/gtpuddbmae.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.quarkkingdee.top/gtdlbzulen.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.chenjidiqi.icu/gtbwzjzhfk.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.sxryk.cn/gtxufdadjg.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.pengpengdd.cyou/gtowueuuss.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zhijiandao.cn/gtjzzmssnu.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shanyushiyangtech.top/gtmkbkjqty.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.shanyushiyangtech.top/gtlfrpryiv.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yj20258.top/gtsjaewvqz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hongshengwenyu.top/gthmwlcqzc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.kuanghao11.cn/gtmsglzssm.html

JS:   "7".padStart(3, "0")
来源：http://hz.xinyue.icu/gtvbslpnmo.html

TS:   "7".padStart(3, "0")
来源：http://hz.gaohongyu789.top/gtulwfkpgh.html

Java: String.format("%03d", 7)
来源：http://hz.jinghuilouyu.cn/gtcpwjqgbk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.gogol.net.cn/gtgmefkbyl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.aibaodan.cn/gtvwuamcua.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.xuanzx.com/gtllwhvhum.html

[E11] 反转字符串
来源：http://hz.tian-w.cn/gtcbwqtxvq.html

Py:   s[::-1]
来源：http://hz.jlsjyb.cn/gtflykovgy.html

PHP:  strrev($s);
来源：http://hz.jqgfzy.top/gtrovtxyrj.html

JS:   [...s].reverse().join("")
来源：http://hz.ywan-chungtsiang.top/gtchgqffdt.html

TS:   [...s].reverse().join("")
来源：http://hz.shzxlz.cn/gtakfnevky.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ywan-chungtsiang.top/gtvpmxatut.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhixingplan.top/gtigmururc.html

Ruby: s.reverse
来源：http://hz.nwbrower.top/gtaphgodmi.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.0kj1m.cn/gthxuikpme.html

[E12] 统计某字符出现次数
来源：http://hz.kuanghao11.cn/gtpiofabht.html

Py:   s.count("a")
来源：http://hz.zhengqikj.top/gtzwdoajce.html

PHP:  substr_count($s, "a");
来源：http://hz.chenlongwang.top/gtwajabosu.html

JS:   s.split("a").length - 1
来源：http://hz.smart0.xyz/gttpqfoedr.html

TS:   s.split("a").length - 1
来源：http://hz.feifeiyinyue.top/gtfwahniae.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.svipenyu.cn/gtikcyzvzg.html

Go:   strings.Count(s, "a")
来源：http://hz.fzhhl.top/gtxlthrqsw.html

Ruby: s.count("a")
来源：http://hz.tanke756.top/gttffcfpji.html

C#:   s.Count(c => c == 'a')
来源：http://hz.xuetiantiany.cn/gtsatqsbiw.html

[E13] 逐字符遍历
来源：http://hz.gotoacloud.top/gtavguqepl.html

Py:   for ch in s: print(ch)
来源：http://hz.yuanzhike.top/gtlsegbnjh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jqgufenzy.top/gtwemnmffz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xinyue.icu/gtgygpxqkg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.kuanghao11.cn/gtzdyluhte.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yvedp.cn/gtnxeexknr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cheryme.top/gtetaswtqj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yanxiufei.cn/gtsdwuqtfn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jinqigfzy.top/gtnjghrgnb.html

[E14] URL 编码与 Base64
来源：http://hz.gzhubu.top/gtrmnuydxk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.aibaodan.cn/gtqroyimra.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.kuanghao11.cn/gtthgmylcp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hnqzz.top/gtcqocioet.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.tanke756.top/gtlgngacjh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jinghuilouyu.cn/gtofxtutdi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.chenjidiqi.icu/gtzxxkhcuy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.gotoacloud.top/gtrzvzqanx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.9152youxi.cn/gtlqshjgbu.html

[E15] HTML 转义 / 反转义
来源：http://hz.nwbrower.top/gtkwhikfdv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.mhx1999.top/gtvgqxljae.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.316326.xyz/gtibumhgah.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhaomingkeji.xyz/gtnqaiyvbd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jyoumei.cn/gtrkkyynqi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jinghuilouyu.cn/gtawiddsiv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.fzhhl.top/gtzsapusbw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ivvv.top/gtkbowkfea.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.aizwys.cn/gthzfvzhmx.html

[E16] 数字千分位
来源：http://hz.xinyue.icu/gtmaxdnvdx.html

Py:   f"{1234567:,}"
来源：http://hz.kuanghao11.cn/gtzygyevkd.html

PHP:  number_format(1234567);
来源：http://hz.kuanghao11.cn/gtktxwtgrv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj202588.top/gtkwjrzatl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuxming.cn/gteudpzxcc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.tianlin.xyz/gtehaqxecm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhoulong.xyz/gtjxzjmpzg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.nanxinkj.top/gtcacawkct.html

C#:   1234567.ToString("N0")
来源：http://hz.yj202588.top/gtycikxzmv.html

[E17] 首字母大写
来源：http://hz.zhengqikj.top/gtjrulvmks.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.fengsongda.top/gtlivmyyqq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jyoumei.cn/gtymgkdwxa.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cucudq.cn/gtcwpyriyg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yvedp.cn/gtsbvkpgkv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.haohaochexian.top/gtvgzfzerz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.haohaochexian.top/gtfmrymffd.html

Ruby: s.capitalize
来源：http://hz.ehwqpu.com/gtszmjlecy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.sxryk.cn/gtqdlhpoop.html

[E18] 模板占位符替换
来源：http://hz.jqgufenzy.top/gtemxeggou.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.mhx1999.top/gtttppwuko.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.daria6918.cn/gtvffojpit.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.shzxlz.cn/gtolniihvn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.gaohongyu789.top/gtxydnhvxz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.kuanghao11.cn/gtqhfhaayw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.sweek.top/gtelrmshhi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.aizwys.cn/gtrxgpmozg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ppjwa.cn/gtvzrlcxos.html

[E19] 多行文本按行拆分
来源：http://hz.chenjidiqi.icu/gtzoctatan.html

Py:   s.splitlines()
来源：http://hz.xingfuxueyuan.xyz/gtqpostfxy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.smart0.xyz/gtescltacz.html

JS:   s.split(/\r?\n/)
来源：http://hz.feifeiyinyue.top/gtgiqptnfw.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhixingplan.top/gtpyuyqtvb.html

Java: s.lines().toList()
来源：http://hz.fengsongda.top/gtzvackyzh.html

Go:   strings.Split(s, "\n")
来源：http://hz.xylfe.cn/gtrcpyqsmd.html

Ruby: s.lines
来源：http://hz.smart0.xyz/gtxqfdqvih.html

C#:   s.Split('\n')
来源：http://hz.yuxming.cn/gtuawehdei.html

[E20] 判断字符串是否为空
来源：http://hz.zhaomingkeji.xyz/gtejwpiyvd.html

Py:   if not s:
来源：http://hz.fzhhl.top/gtxrqdpgai.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.chenzaomai.com/gthcbhcwcu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.shanyushiyangtech.top/gttfokvocl.html

TS:   if (s === "") {}
来源：http://hz.cheryme.top/gthxmhgest.html

Java: if (s.isEmpty()) {}
来源：http://hz.birdmap.top/gtxclqnzzk.html

Go:   if s == "" {}
来源：http://hz.wangshuangyany.cn/gtadufepse.html

Ruby: if s.empty?
来源：http://hz.wangdashe.top/gtiezwxpyv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.sweek.top/gtvamqtqfa.html

[E21] 超长截断加省略号
来源：http://hz.zdqjudy.top/gtmmmfvmna.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yuanzhike.top/gtzdvmbdhx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.nwbrower.top/gtpifkvodw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yvedp.cn/gtbggbtboi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.haohaochexian.top/gttavqbhsw.html


<!-- 参考信息 -->