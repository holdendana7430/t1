代发 wailian999

TS:   [...new Set(arr)]
来源：http://hz.ppjwa.cn/gtsvxhgbot.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.tianlin.xyz/gtnkubrhgj.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.xuetiantiany.cn/gtnrdxnbwj.html

Ruby: arr.uniq
来源：http://hz.smart0.xyz/gtvnrdqlbr.html

C#:   list.Distinct().ToList()
来源：http://hz.fengsongda.top/gtvtcnkvgk.html

[D16] 求和与平均值
来源：http://hz.sysykeji.top/gtoxahwzti.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.tianlin.xyz/gtspltexcu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.nanxinkj.top/gtgeztvhbo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hysaishi.cn/gtgxjmmzdc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xingfuxueyuan.xyz/gtenfiereb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.cashguo.top/gtpmrucwqu.html

Go:   // 手写循环累加
来源：http://hz.yj20258888.top/gtrxfricsv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.tian-w.cn/gtqxszlyjw.html

C#:   list.Sum();  list.Average()
来源：http://hz.tanke756.top/gtjupzznse.html

[D17] 最大值与最小值
来源：http://hz.cdnleiting.top/gtloleblpq.html

Py:   max(arr);  min(arr)
来源：http://hz.gaohongyu789.top/gtsxtexodw.html

PHP:  max($arr);  min($arr);
来源：http://hz.chenlongwang.top/gtcnfjqjsy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yanxiufei.cn/gtowslbprw.html

TS:   Math.max(...arr);
来源：http://hz.chenzaomai.com/gtsfhpwoth.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhijiandao.cn/gtsyyubfkb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hongshengwenyu.top/gtmqujszkn.html

Ruby: arr.max;  arr.min
来源：http://hz.c1oappe.top/gtrtlebiyc.html

C#:   list.Max();  list.Min()
来源：http://hz.0kj1m.cn/gtafzgkdmp.html

[D18] 扁平化嵌套数组
来源：http://hz.jianghu66.top/gtpwchorxg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xylfe.cn/gtklnjkagm.html

PHP:  array_merge(...$nested);
来源：http://hz.zhoulong.xyz/gtqrogqajo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xuetiantiany.cn/gttiauhbet.html

TS:   nested.flat();
来源：http://hz.jlsjyb.cn/gtspkkwapz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.daria6918.cn/gtfwjpziuh.html

Go:   // 手写双层循环
来源：http://hz.jianghu66.top/gtyryvgvnz.html

Ruby: nested.flatten
来源：http://hz.feifeiyinyue.top/gtspnaaxum.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yanxiufei.cn/gtpcreiwzd.html

[D19] 按字段分组
来源：http://hz.feifeiyinyue.top/gtbzjonobt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.c1oappe.top/gtcrmgrmwr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hysaishi.cn/gtinmhnqhz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zhijiandao.cn/gtzzfcpmwp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yuanzhike.top/gtbiyilxpz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.sufxvd.cn/gtoqulhkce.html

Go:   // 手写 map[string][]T
来源：http://hz.xuetiantiany.cn/gttabifjyv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhongyouzk.top/gteqmlocqq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhijiandao.cn/gtqbqfcngy.html

[D20] 统计每个元素出现次数
来源：http://hz.shangyingyoupin.top/gtpkodtssa.html

Py:   Counter(arr)
来源：http://hz.wangshuangyany.cn/gtnbaojqgn.html

PHP:  array_count_values($arr);
来源：http://hz.ivvv.top/gtdtjxvpqo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.nanxuanxn.top/gtqaphwiks.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cheryme.top/gtujsolsli.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hfpthk.cn/gtzxqjenik.html

Go:   // 手写 map[T]int
来源：http://hz.yongpay.top/gtgvzpvtgg.html

Ruby: arr.tally
来源：http://hz.aibaodan.cn/gtnqzbldyz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.9152youxi.cn/gtktlpzqdf.html

[D21] 判断是否包含某元素
来源：http://hz.ivvv.top/gthqyshiqc.html

Py:   x in arr
来源：http://hz.xziqi.cn/gttecubkrw.html

PHP:  in_array($x, $arr, true);
来源：http://hz.tianlin.xyz/gtaaqdgzzx.html

JS:   arr.includes(x)
来源：http://hz.shuidangran.top/gtakoikipz.html

TS:   arr.includes(x)
来源：http://hz.cashguo.top/gtytnkhfav.html

Java: list.contains(x)
来源：http://hz.snrcjt.cn/gtsnpcfurm.html

Go:   slices.Contains(arr, x)
来源：http://hz.havefunace.top/gtxteebceq.html

Ruby: arr.include?(x)
来源：http://hz.sxryk.cn/gtunlhrsvc.html

C#:   list.Contains(x)
来源：http://hz.meibo888.top/gtkaxthmyo.html

[D22] 复制数组（避免共享引用）
来源：http://hz.sufxvd.cn/gtnilmgfbw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.sufxvd.cn/gthwxgubzt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ybcxt.top/gtlklodxqb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ydzc1.top/gtdbyqtjed.html

TS:   [...arr];
来源：http://hz.guannengcc.top/gtbtnfvzpo.html

Java: new ArrayList<>(list);
来源：http://hz.cdnleiting.top/gtpeenmiba.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zhoulong.xyz/gtktkibwju.html

Ruby: arr.dup;  arr.clone
来源：http://hz.shzxlz.cn/gtegqgisji.html

C#:   new List<int>(list);
来源：http://hz.yj20258.top/gtrurifikp.html

[D23] reduce 累积计算
来源：http://hz.daxiang520.top/gtqppjxsbg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.aibaodan.cn/gtudxhbxyi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yanxiufei.cn/gtuhznlhem.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sysykeji.top/gtsmomaznp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xylfe.cn/gtehztrvfb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.daria6918.cn/gtnusoqdvc.html

Go:   // 手写循环
来源：http://hz.iojbl.cn/gtfuokrphl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hnqzz.top/gtcazplnfb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.wangshuangyany.cn/gtvzoqvmrf.html

[D24] 字典 / Map 基本操作
来源：http://hz.jinqigufen.top/gtfdvmbgmk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhijiandao.cn/gtsjqlwvsg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hammf.cn/gtjqudhqyj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.daria6918.cn/gtsozoibyz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.meibo888.top/gtudokhffd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zdqjudy.top/gtihnzkbqu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.dianchejie.cn/gtilapjyru.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ydzc1.top/gtbpbvcpip.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.birdmap.top/gtdvkduhkz.html

[D25] Set 集合去重与交并差
来源：http://hz.tian-w.cn/gtmzcicwfw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.52xcode.cn/gtbwdngubw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zdqjudy.top/gtjzetbetu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.c1oappe.top/gtpejxgvsz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhiwuduotai.top/gtijtaerrl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hammf.cn/gtjbmxanre.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jyoumei.cn/gtmmttuipu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.chenjidiqi.icu/gtezzvginn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhongyouzk.top/gtxcwptaqx.html

[D26] 数组转字符串
来源：http://hz.xuanzx.com/gtsisvxqwi.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ybcxt.top/gtvzythlol.html

PHP:  implode(", ", $arr);
来源：http://hz.hywenlv.cn/gtuydvbcyz.html

JS:   arr.join(", ")
来源：http://hz.nwbrower.top/gtlsoeuaak.html

TS:   arr.join(", ")
来源：http://hz.jinqigufen.top/gtmtahouzo.html

Java: String.join(", ", list)
来源：http://hz.andypj.xyz/gtgggffysw.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ywan-chungtsiang.top/gtfnvbdtzg.html

Ruby: arr.join(", ")
来源：http://hz.hywenlv.cn/gtxaygtlon.html

C#:   string.Join(", ", list)
来源：http://hz.52xcode.cn/gtpuezcmgn.html

================================================================================
来源：http://hz.gzhubu.top/gtdcqnqdsk.html

E. 字符串处理
来源：http://hz.feifeiyinyue.top/gtppmymooh.html

================================================================================
来源：http://hz.jinqigfzy.top/gtuhjpbqev.html

[E01] 拼接字符串
来源：http://hz.fzhhl.top/gtcefzovrp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.sysykeji.top/gtvhgstgwq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.nwbrower.top/gtgxnbkfor.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sweek.top/gtbowirotz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinghuilouyu.cn/gteiytanyg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zhengqikj.top/gtgitucavg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.gotoacloud.top/gtxreymuom.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.sweek.top/gtxbgwnjmq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yangfankeji.com/gtsdnnorcf.html

[E02] 重复字符串
来源：http://hz.chenjidiqi.icu/gthrxcctsf.html

Py:   "ab" * 3
来源：http://hz.guowangkeji.top/gtypedekkr.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hongshengwenyu.top/gtlswheypx.html

JS:   "ab".repeat(3)
来源：http://hz.9152youxi.cn/gtioylwukn.html

TS:   "ab".repeat(3)
来源：http://hz.yonumen.top/gtxpkkcphs.html

Java: "ab".repeat(3)
来源：http://hz.yanxiufei.cn/gtyenhlyzh.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.nanxinkj.top/gtkpwpbctf.html

Ruby: "ab" * 3
来源：http://hz.nanxinkj.top/gtodbmebyp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.shanyushiyangkeji.top/gtndivoaid.html

[E03] 截取子串
来源：http://hz.shangyingyoupin.top/gtnmaqoknl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.wangshuangyany.cn/gtsbqzxnyh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jqgufenzy.top/gttylzsldg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.vqdsnc.cn/gtparkraip.html

TS:   s.slice(1, 4)
来源：http://hz.xinyue.icu/gtgeiiohki.html

Java: s.substring(1, 4)
来源：http://hz.xziqi.cn/gtjbolrfbb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.chenlongwang.top/gttegznnqu.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.sysykeji.top/gthktlaxow.html

C#:   s.Substring(1, 3)
来源：http://hz.jinqigfzy.top/gtviwiftvk.html

[E04] 查找子串位置
来源：http://hz.ywan-chungtsiang.top/gtypaswymt.html

Py:   s.find("x");  s.index("x")
来源：http://hz.0kj1m.cn/gtfxvogrge.html

PHP:  strpos($s, "x");
来源：http://hz.zdqjudy.top/gteifrzrpt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhijiandao.cn/gtkfipzzbc.html

TS:   s.indexOf("x")
来源：http://hz.sysykeji.top/gtthlsmlow.html

Java: s.indexOf("x")
来源：http://hz.shzxlz.cn/gtqsuplvqs.html

Go:   strings.Index(s, "x")
来源：http://hz.52xcode.cn/gtulnsirbq.html

Ruby: s.index("x")
来源：http://hz.jinyuanbaomall.cn/gtyxsurkot.html

C#:   s.IndexOf("x")
来源：http://hz.redwolf501.top/gtghcprjyw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.birdmap.top/gttutrfcuq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhiwuduotai.top/gthauzrblc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.cqqwz.cn/gtodsjuaut.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.bjfxy.top/gteljcfdpw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.gaohongyu789.top/gtywehiscg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xuetiantiany.cn/gtbrnyuouq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.sufxvd.cn/gtfexvdlcd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.sufxvd.cn/gtallashts.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jianghu66.top/gtxmcbpbaj.html

[E06] 替换子串
来源：http://hz.hysaishi.cn/gtisqdhlwf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.ydzc1.top/gtwadfwhza.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xinyue.icu/gtmbcstkvy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.chenlongwang.top/gtzkgakrdp.html

TS:   s.replaceAll("a", "b")
来源：http://hz.tian-w.cn/gtsuquescc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhengqikj.top/gtghrkkbkg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.nanxuanxn.top/gtbrjxkaik.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.daxiang520.top/gtefsuhfvk.html

C#:   s.Replace("a", "b")
来源：http://hz.guannengcc.top/gtwbnnqtyv.html

[E07] 按分隔符拆分
来源：http://hz.daxiang520.top/gtfklehscn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.52xcode.cn/gtjdtbyigc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jlsjyb.cn/gtxrdptnut.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.316326.xyz/gtpejrwjry.html

TS:   s.split(",")
来源：http://hz.zhengqikj.top/gtwplzzcfk.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.gotoacloud.top/gtbterwvwd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.sxryk.cn/gtkzblgeka.html

Ruby: s.split(",");  s.split
来源：http://hz.ppjwa.cn/gtecszgoqc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hywenlv.cn/gtrtrhvboe.html

[E08] 数组按分隔符合并
来源：http://hz.zdqjudy.top/gthiqqglmk.html

Py:   ",".join(items)
来源：http://hz.svipenyu.cn/gtmzomwdud.html

PHP:  implode(",", $items);
来源：http://hz.mhx1999.top/gtatofamtq.html

JS:   items.join(",")
来源：http://hz.nanxuanxn.top/gtzuxcnyje.html

TS:   items.join(",")
来源：http://hz.meibo888.top/gthxgbvkgk.html

Java: String.join(",", items)
来源：http://hz.ydzc1.top/gtigyxdxqi.html

Go:   strings.Join(items, ",")
来源：http://hz.cdnleiting.top/gtjzikfhhu.html

Ruby: items.join(",")
来源：http://hz.yj20258888.top/gtiyboonbo.html

C#:   string.Join(",", items)
来源：http://hz.mhx1999.top/gtjfemqirm.html

[E09] 去除所有空白字符
来源：http://hz.nwbrower.top/gtyloijogk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.smart0.xyz/gthuzkuuhh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.birdmap.top/gttpnamqku.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhixingplan.top/gtgzllzbbh.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.xuetiantiany.cn/gtiddehtvj.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yuanzhike.top/gtrikwhpbu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yongpay.top/gtdshqhruq.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.havefunace.top/gtlyzehqko.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jiagoushi.top/gtwdhbaivg.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ydjk.org.cn/gtyaduriop.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.tian-w.cn/gtvxbmfujj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.ehwqpu.com/gtialgrtis.html

JS:   "7".padStart(3, "0")
来源：http://hz.aizwys.cn/gtrpxbwfsg.html

TS:   "7".padStart(3, "0")
来源：http://hz.aibaodan.cn/gtmtgoaaml.html

Java: String.format("%03d", 7)
来源：http://hz.jlsjyb.cn/gtuiksthmu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.gaohongyu789.top/gtgkecvqxb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.cheryme.top/gtswxbvsjq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shangyingyoupin.top/gthiqymngq.html

[E11] 反转字符串
来源：http://hz.tian-w.cn/gtdugnwdco.html

Py:   s[::-1]
来源：http://hz.ydzc1.top/gtjdmniyxp.html

PHP:  strrev($s);
来源：http://hz.cdnleiting.top/gtmgmenklf.html

JS:   [...s].reverse().join("")
来源：http://hz.fengsongda.top/gtrfybtdcd.html

TS:   [...s].reverse().join("")
来源：http://hz.yuxming.cn/gtmsvvjzxt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shzxlz.cn/gtllgkwxza.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hfpthk.cn/gtavsxlgin.html

Ruby: s.reverse
来源：http://hz.wangshuangyany.cn/gtlumadabk.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.ydzc1.top/gtosocmnkj.html

[E12] 统计某字符出现次数
来源：http://hz.zhiwuduotai.top/gteyjocdtf.html

Py:   s.count("a")
来源：http://hz.iojbl.cn/gtkrwwvuxd.html

PHP:  substr_count($s, "a");
来源：http://hz.gaohongyu789.top/gtfoogvwsr.html

JS:   s.split("a").length - 1
来源：http://hz.nwbrower.top/gtfyhwtqfa.html

TS:   s.split("a").length - 1
来源：http://hz.hysaishi.cn/gtraulsukq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhijiandao.cn/gtgdjyxhph.html

Go:   strings.Count(s, "a")
来源：http://hz.9152youxi.cn/gtkpxenlnx.html

Ruby: s.count("a")
来源：http://hz.shangyingyoupin.top/gttzpynexf.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jyoumei.cn/gtabgehmtv.html

[E13] 逐字符遍历
来源：http://hz.nanxuanxn.top/gtzmsoqeai.html

Py:   for ch in s: print(ch)
来源：http://hz.ppjwa.cn/gtlpiukdjk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yangfankeji.com/gtbhxetppb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.svipenyu.cn/gteydvducz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hongshengwenyu.top/gtswnklvmo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.chenjidiqi.icu/gtguwknich.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hysaishi.cn/gtpgmniarg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jiagoushi.top/gtywnsokti.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.gogol.net.cn/gtumaifhfn.html

[E14] URL 编码与 Base64
来源：http://hz.zdqjudy.top/gtrgfvodxn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.chenlongwang.top/gtrotgslrm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jinghuilouyu.cn/gtmqftvwva.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.gotoacloud.top/gtlndnonwe.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.gotoacloud.top/gtmcesorza.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.nanxuanxn.top/gtwkqouhxr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.hammf.cn/gtujrddmax.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jqgfzy.top/gtqgrlwpea.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yj20258.top/gtjrjaxuma.html

[E15] HTML 转义 / 反转义
来源：http://hz.jinqigufen.top/gtsdwscrth.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.iojbl.cn/gteljzcqhw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.wangshuangyany.cn/gtmwljqbqi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.iojbl.cn/gthrckjrnw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ehwqpu.com/gtkjwnrmbr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.daxiang520.top/gttommvmbq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ywan-chungtsiang.top/gtutdgsupc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jyoumei.cn/gtmygxqlfh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.sysykeji.top/gtopnoicea.html

[E16] 数字千分位
来源：http://hz.gogol.net.cn/gtrbmuohbr.html

Py:   f"{1234567:,}"
来源：http://hz.yj202588.top/gtkermclhk.html

PHP:  number_format(1234567);
来源：http://hz.jinqigfzy.top/gtvmlbodhg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.c1oappe.top/gttdzapkau.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.shuidangran.top/gttziroxuv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.pengpengdd.cyou/gtbocymepo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhijiandao.cn/gtppjzcxoi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.guowangkeji.top/gtraaosopv.html

C#:   1234567.ToString("N0")
来源：http://hz.pycfn.com/gtwvgulyaf.html

[E17] 首字母大写
来源：http://hz.nanxinkj.top/gttalrjarv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.pycfn.com/gtbispylcc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.aizwys.cn/gtsuzbbaqu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhoulong.xyz/gtuetgntsl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.dianchejie.cn/gtpmasbkkw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.daxiang520.top/gtbzqbslfl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jqgfzy.top/gtmdsdwepk.html

Ruby: s.capitalize
来源：http://hz.nanxinkj.top/gttcqfxcgk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xylfe.cn/gttqtneiai.html

[E18] 模板占位符替换
来源：http://hz.vqdsnc.cn/gteoaxcpjh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shangyingyoupin.top/gtlrpdqejk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.nanxuanxn.top/gtxlqmomty.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.smart0.xyz/gteipjqdun.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xingfuxueyuan.xyz/gtunppxwut.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.xziqi.cn/gtgcgteyrd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.sweek.top/gtynpuphrq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhiwuduotai.top/gtgmwukusf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.c1oappe.top/gtjrpstxcf.html

[E19] 多行文本按行拆分
来源：http://hz.hfpthk.cn/gtbgsdggwt.html

Py:   s.splitlines()
来源：http://hz.nanxinkj.top/gthcpzaieg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.cucudq.cn/gtacrdetwt.html

JS:   s.split(/\r?\n/)
来源：http://hz.cheryme.top/gtxbbzbrxz.html

TS:   s.split(/\r?\n/)
来源：http://hz.bjfxy.top/gteqhkukjp.html

Java: s.lines().toList()
来源：http://hz.ydjk.org.cn/gtpcajzwwo.html

Go:   strings.Split(s, "\n")
来源：http://hz.ydzc1.top/gtuetxldvv.html

Ruby: s.lines
来源：http://hz.fzhhl.top/gtmkcwxpwv.html

C#:   s.Split('\n')
来源：http://hz.9152youxi.cn/gtomnaaccd.html

[E20] 判断字符串是否为空
来源：http://hz.cheryme.top/gtpitpdiyf.html

Py:   if not s:
来源：http://hz.feifeiyinyue.top/gtnrqnebar.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.snrcjt.cn/gtaffjxmlb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yj202588.top/gtddfowwld.html

TS:   if (s === "") {}
来源：http://hz.hammf.cn/gtvujeqmyt.html

Java: if (s.isEmpty()) {}
来源：http://hz.hnqzz.top/gtfsjghpbj.html

Go:   if s == "" {}
来源：http://hz.gotoacloud.top/gtgsrqysxg.html

Ruby: if s.empty?
来源：http://hz.fengsongda.top/gtillrvfxj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.sweek.top/gtvitsybly.html

[E21] 超长截断加省略号
来源：http://hz.hongshengwenyu.top/gtzehjwwke.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.svipenyu.cn/gtcnildmqr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.redwolf501.top/gtmcocdvao.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shanyushiyangtech.top/gtyadvvomg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.mhx1999.top/gtbqgoblwq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.fengsongda.top/gtdeshppsc.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhiwuduotai.top/gtuganxqie.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hnxiangtu.top/gtuorihvog.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.hfpthk.cn/gtttzedhct.html

[E22] 字节长度与字符长度
来源：http://hz.fzhhl.top/gtzgcegumj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.tian-w.cn/gtrrobezso.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hnqzz.top/gtavjbgorm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.pengpengdd.cyou/gtvhmbtlab.html


<!-- 参考信息 -->