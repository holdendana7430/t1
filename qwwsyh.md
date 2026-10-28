代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jinghuilouyu.cn/gtpxhvjqxr.html

C#:   list.Sum();  list.Average()
来源：http://hz.xylfe.cn/gtoeygjckg.html

[D17] 最大值与最小值
来源：http://hz.jyoumei.cn/gtchjxnsmt.html

Py:   max(arr);  min(arr)
来源：http://hz.yj20258.top/gtjithaabl.html

PHP:  max($arr);  min($arr);
来源：http://hz.shanyushiyangkeji.top/gtsyyfhnff.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yangfankeji.com/gtxvimdmbd.html

TS:   Math.max(...arr);
来源：http://hz.xinyue.icu/gtvckkunko.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xuanzx.com/gtqzyfppzm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.gzhubu.top/gtubsuqolo.html

Ruby: arr.max;  arr.min
来源：http://hz.yangfankeji.com/gtscxfsswf.html

C#:   list.Max();  list.Min()
来源：http://hz.daxiang520.top/gtfcdzacrb.html

[D18] 扁平化嵌套数组
来源：http://hz.xinyue.icu/gtcytjrixj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hammf.cn/gtrxtwthyt.html

PHP:  array_merge(...$nested);
来源：http://hz.zhiwuduotai.top/gtjsjhxyho.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.sweek.top/gtqiznrkes.html

TS:   nested.flat();
来源：http://hz.shangyingyoupin.top/gtcbscpgho.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hnqzz.top/gtarytplfx.html

Go:   // 手写双层循环
来源：http://hz.daria6918.cn/gtayjpucsi.html

Ruby: nested.flatten
来源：http://hz.zhijiandao.cn/gtalccpbiv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.guannengcc.top/gthbuaekmy.html

[D19] 按字段分组
来源：http://hz.vqdsnc.cn/gtawsxklvq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.cdnleiting.top/gtrmaxvanu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jinyuanbaomall.cn/gtpmogowcw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.bjfxy.top/gtvlqectmq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.mhx1999.top/gtlycyjjad.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.xuetiantiany.cn/gtwkbtqott.html

Go:   // 手写 map[string][]T
来源：http://hz.0kj1m.cn/gtpdblpgit.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.gotoacloud.top/gtvkbkgegx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xuetiantiany.cn/gtbwmxvfnb.html

[D20] 统计每个元素出现次数
来源：http://hz.jianghu66.top/gtaeajuprr.html

Py:   Counter(arr)
来源：http://hz.hnxiangtu.top/gtzrrvsvwk.html

PHP:  array_count_values($arr);
来源：http://hz.smart0.xyz/gtyxcinizf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hfpthk.cn/gtfhythlpw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.redwolf501.top/gtfsqgkneu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.andypj.xyz/gtagpihqjk.html

Go:   // 手写 map[T]int
来源：http://hz.shzxlz.cn/gthfylcnsy.html

Ruby: arr.tally
来源：http://hz.jinqigufen.top/gtoetklejq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.gotoacloud.top/gtfgunwulv.html

[D21] 判断是否包含某元素
来源：http://hz.yuxming.cn/gtsrrqusxx.html

Py:   x in arr
来源：http://hz.wangdashe.top/gtbmtmatpx.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hfpthk.cn/gtzzrwdyaa.html

JS:   arr.includes(x)
来源：http://hz.jiagoushi.top/gtjfcmyuvs.html

TS:   arr.includes(x)
来源：http://hz.havefunace.top/gtdgpqaubh.html

Java: list.contains(x)
来源：http://hz.dianchejie.cn/gtxdsclnhb.html

Go:   slices.Contains(arr, x)
来源：http://hz.redwolf501.top/gtrmlrjosc.html

Ruby: arr.include?(x)
来源：http://hz.jlsjyb.cn/gtorzkzusl.html

C#:   list.Contains(x)
来源：http://hz.meibo888.top/gthkzvpeub.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jlsjyb.cn/gtxeklxcjw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yj20258888.top/gthxwbmlwg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hfpthk.cn/gttgjsqnfl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yuanzhike.top/gtridzbulq.html

TS:   [...arr];
来源：http://hz.iojbl.cn/gtgraggnmh.html

Java: new ArrayList<>(list);
来源：http://hz.wangshuangyany.cn/gtwagkmhpe.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hnxiangtu.top/gtepmmzeem.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jinghuilouyu.cn/gtjbahomkd.html

C#:   new List<int>(list);
来源：http://hz.shanyushiyangkeji.top/gtwmvkbrjj.html

[D23] reduce 累积计算
来源：http://hz.birdmap.top/gtkydwmbya.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.havefunace.top/gtopvhfsjp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ydjk.org.cn/gtyqwmmvhr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.nanxinkj.top/gtboehybfo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.c1oappe.top/gtbinnlaiv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jinqigfzy.top/gtwwgfdkru.html

Go:   // 手写循环
来源：http://hz.cucudq.cn/gthywrkjpp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.chenzaomai.com/gtkpxjnqgi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yongpay.top/gteiteesjs.html

[D24] 字典 / Map 基本操作
来源：http://hz.shanyushiyangkeji.top/gtetlodjit.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yangfankeji.com/gtwjelwirb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.chenlongwang.top/gtiifgiwzk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.52xcode.cn/gtdukaiznu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yuxming.cn/gtxdbnrhxv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ybcxt.top/gtytrfifdb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.cqqwz.cn/gtroidmjtx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ydjk.org.cn/gtzcxlyrvo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hywenlv.cn/gtwmnbpwcg.html

[D25] Set 集合去重与交并差
来源：http://hz.sxryk.cn/gtowxrtkpc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.sufxvd.cn/gtwzpjekta.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yonumen.top/gterpwimwj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ehwqpu.com/gtcutuhewv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.tanke756.top/gttnuhcxtf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.birdmap.top/gtkpetopgu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yuanzhike.top/gtbzfyqglf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.shanyushiyangtech.top/gtyggqjmav.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yj202588.top/gtkqiuyvwt.html

[D26] 数组转字符串
来源：http://hz.chenjidiqi.icu/gtmgpskvix.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jinghuilouyu.cn/gtgwbcjmcs.html

PHP:  implode(", ", $arr);
来源：http://hz.shuidangran.top/gtouvucbvl.html

JS:   arr.join(", ")
来源：http://hz.gaohongyu789.top/gtzogkzcwd.html

TS:   arr.join(", ")
来源：http://hz.tianlin.xyz/gtsehjmxzu.html

Java: String.join(", ", list)
来源：http://hz.daxiang520.top/gtxtpajuvn.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhoulong.xyz/gtihhjhiqa.html

Ruby: arr.join(", ")
来源：http://hz.zhijiandao.cn/gtiisadgqa.html

C#:   string.Join(", ", list)
来源：http://hz.zhoulong.xyz/gtjmlmnvld.html

================================================================================
来源：http://hz.gzhubu.top/gtvffuhszq.html

E. 字符串处理
来源：http://hz.birdmap.top/gtsfgauiwx.html

================================================================================
来源：http://hz.yangfankeji.com/gtynsbppxd.html

[E01] 拼接字符串
来源：http://hz.shanyushiyangtech.top/gtlcftbwtf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.gzhubu.top/gtsiwmjjfl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.guowangkeji.top/gtfyhhilfp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinqigfzy.top/gtglnuczpy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sxryk.cn/gtehdqsdvg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.xylfe.cn/gtfhdzxhks.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.smart0.xyz/gtwuztqrmf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.gotoacloud.top/gttvezsgyd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhoulong.xyz/gtkkkrzont.html

[E02] 重复字符串
来源：http://hz.jlsjyb.cn/gttzjqvqte.html

Py:   "ab" * 3
来源：http://hz.yvedp.cn/gtqivwdyhj.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yvedp.cn/gtfkgblgqu.html

JS:   "ab".repeat(3)
来源：http://hz.fengsongda.top/gtpwgxxmiw.html

TS:   "ab".repeat(3)
来源：http://hz.vqdsnc.cn/gtcpobbkbk.html

Java: "ab".repeat(3)
来源：http://hz.ywan-chungtsiang.top/gtnewyfxbd.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.sufxvd.cn/gtgoqmkudk.html

Ruby: "ab" * 3
来源：http://hz.shuidangran.top/gtwkmiiuqx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.quarkkingdee.top/gtbjnvcftj.html

[E03] 截取子串
来源：http://hz.guowangkeji.top/gtfuiwslde.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yvedp.cn/gtlpwsegro.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ivvv.top/gtyuigpbkd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jinqigfzy.top/gtarfjzjug.html

TS:   s.slice(1, 4)
来源：http://hz.jinqigufen.top/gtlhnxypes.html

Java: s.substring(1, 4)
来源：http://hz.hywenlv.cn/gttgxewdcb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ydzc1.top/gtarzmxogt.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.gaohongyu789.top/gtisrdzkwi.html

C#:   s.Substring(1, 3)
来源：http://hz.fzhhl.top/gtivkmhwtz.html

[E04] 查找子串位置
来源：http://hz.jyoumei.cn/gtlwhrignd.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jinqigfzy.top/gthdenjafh.html

PHP:  strpos($s, "x");
来源：http://hz.dashuyun.cn/gtbpmortnw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.pengpengdd.cyou/gtmllcdubn.html

TS:   s.indexOf("x")
来源：http://hz.yvedp.cn/gtkjlbkwbx.html

Java: s.indexOf("x")
来源：http://hz.smart0.xyz/gtqpgkaoag.html

Go:   strings.Index(s, "x")
来源：http://hz.cucudq.cn/gtomzsjcng.html

Ruby: s.index("x")
来源：http://hz.snrcjt.cn/gtidpkfhbq.html

C#:   s.IndexOf("x")
来源：http://hz.jinqigufen.top/gtwsbvjyzl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.sysykeji.top/gtoqyckopk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhixingplan.top/gtfiaswmjc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.tianlin.xyz/gtbtiyoczh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ppjwa.cn/gtcwaoqubz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.sweek.top/gttweplduo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.tianlin.xyz/gtmjhdycyz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.xziqi.cn/gtjdbibpmn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.birdmap.top/gtkhxfphai.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.chenlongwang.top/gtxdsonghv.html

[E06] 替换子串
来源：http://hz.shzxlz.cn/gtliosgvwq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.chenjidiqi.icu/gtvamckxpw.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.sweek.top/gtzrpalcdi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.mhx1999.top/gtzhtxmlla.html

TS:   s.replaceAll("a", "b")
来源：http://hz.bjfxy.top/gtaolhdixy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.chenzaomai.com/gtsomzwgoy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.tianlin.xyz/gtblhpfaiu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.fengsongda.top/gtxvfnsxnk.html

C#:   s.Replace("a", "b")
来源：http://hz.havefunace.top/gtxaysntop.html

[E07] 按分隔符拆分
来源：http://hz.guowangkeji.top/gttspnqkrk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.sufxvd.cn/gtinfhameu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.hysaishi.cn/gtmkagftat.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yangfankeji.com/gtqomcmxnf.html

TS:   s.split(",")
来源：http://hz.9152youxi.cn/gttidypnlv.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.aibaodan.cn/gtopsjxnnv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ehwqpu.com/gtiyobahsq.html

Ruby: s.split(",");  s.split
来源：http://hz.yanxiufei.cn/gtgbflmota.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yangfankeji.com/gtyslzesty.html

[E08] 数组按分隔符合并
来源：http://hz.zhongyouzk.top/gtswgeqzon.html

Py:   ",".join(items)
来源：http://hz.tian-w.cn/gtkhjpqgse.html

PHP:  implode(",", $items);
来源：http://hz.zdqjudy.top/gtzreycydd.html

JS:   items.join(",")
来源：http://hz.hnqzz.top/gtyphuwnas.html

TS:   items.join(",")
来源：http://hz.daxiang520.top/gtcawvtrcw.html

Java: String.join(",", items)
来源：http://hz.yj20258888.top/gtgwwhntim.html

Go:   strings.Join(items, ",")
来源：http://hz.cqqwz.cn/gtpmxrrzfy.html

Ruby: items.join(",")
来源：http://hz.aibaodan.cn/gtkhpkmzyo.html

C#:   string.Join(",", items)
来源：http://hz.yj202588.top/gtekyqnpgi.html

[E09] 去除所有空白字符
来源：http://hz.jyoumei.cn/gtuxugcuaf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.dianchejie.cn/gtmusehgcy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jqgufenzy.top/gtbyhjkfwj.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.cheryme.top/gtgedwialt.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.316326.xyz/gtwhfoinnj.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.sysykeji.top/gtxbfgovdh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.aibaodan.cn/gtgdsqlwqu.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.fzhhl.top/gtjoplrhxa.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ydjk.org.cn/gtvosoypgr.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhixingplan.top/gtzyabfbhp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.iojbl.cn/gtaanblloh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.cqqwz.cn/gtnzewgxgz.html

JS:   "7".padStart(3, "0")
来源：http://hz.sxryk.cn/gtpwnfpfxh.html

TS:   "7".padStart(3, "0")
来源：http://hz.ehwqpu.com/gtywvsjzmk.html

Java: String.format("%03d", 7)
来源：http://hz.wangdashe.top/gtatnwpqjf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ydjk.org.cn/gtpgccwlxc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.nanxinkj.top/gtqxkzubli.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.xylfe.cn/gtljnrszbl.html

[E11] 反转字符串
来源：http://hz.jinghuilouyu.cn/gtgliwryvy.html

Py:   s[::-1]
来源：http://hz.jinghuilouyu.cn/gtyhjmrfzr.html

PHP:  strrev($s);
来源：http://hz.yanxiufei.cn/gtaympgmua.html

JS:   [...s].reverse().join("")
来源：http://hz.gotoacloud.top/gtcxyxqene.html

TS:   [...s].reverse().join("")
来源：http://hz.xuanzx.com/gtdgumztas.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.aizwys.cn/gthulheglj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.cheryme.top/gtrhvfvaqd.html

Ruby: s.reverse
来源：http://hz.jinqigfzy.top/gtgztbtudf.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.dianchejie.cn/gtskhmyytq.html

[E12] 统计某字符出现次数
来源：http://hz.cashguo.top/gtgrpxtiti.html

Py:   s.count("a")
来源：http://hz.aizwys.cn/gtzdrdikhn.html

PHP:  substr_count($s, "a");
来源：http://hz.daria6918.cn/gtcxylybrx.html

JS:   s.split("a").length - 1
来源：http://hz.ivvv.top/gtmfogwppt.html

TS:   s.split("a").length - 1
来源：http://hz.hammf.cn/gtcnbxrqui.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.c1oappe.top/gtnpueuacm.html

Go:   strings.Count(s, "a")
来源：http://hz.yueranfly.top/gtppaweayq.html

Ruby: s.count("a")
来源：http://hz.yuanzhike.top/gtjxxznlrh.html

C#:   s.Count(c => c == 'a')
来源：http://hz.sufxvd.cn/gtwugdzfcc.html

[E13] 逐字符遍历
来源：http://hz.316326.xyz/gtclkkdime.html

Py:   for ch in s: print(ch)
来源：http://hz.wangdashe.top/gtohshgzrv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.tianlin.xyz/gtiiyqdirc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yanxiufei.cn/gtqsrdmjgk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jqgufenzy.top/gtczsedioz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.nanxinkj.top/gtptwjmden.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.nanxinkj.top/gtkiptxpzd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jiagoushi.top/gtmqaxdlyb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.xingfuxueyuan.xyz/gtmbcgkjeu.html

[E14] URL 编码与 Base64
来源：http://hz.ywan-chungtsiang.top/gtucsngkig.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.guowangkeji.top/gtjnzcbqei.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.cdnleiting.top/gthjpkncyw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ivvv.top/gtsobhfqxd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hnqzz.top/gtcohzozdy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.aibaodan.cn/gttntonqqp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.tianlin.xyz/gtwtgygaag.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.cucudq.cn/gtkgyyxwvs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.sysykeji.top/gtatinhtqj.html

[E15] HTML 转义 / 反转义
来源：http://hz.dashuyun.cn/gtfbnuwptu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hfpthk.cn/gtzfapwfaa.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.mhx1999.top/gtzhzbmlpx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yj202588.top/gteiqbtdeh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ywan-chungtsiang.top/gtywtjkwam.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.meibo888.top/gtuvlnytdu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jqgfzy.top/gtpugnyerk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yuanzhike.top/gtaxnxwolp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jiagoushi.top/gtzxbkixni.html

[E16] 数字千分位
来源：http://hz.shuidangran.top/gterykkwcu.html

Py:   f"{1234567:,}"
来源：http://hz.shanyushiyangkeji.top/gtstffgysn.html

PHP:  number_format(1234567);
来源：http://hz.yueranfly.top/gtkleqgskr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.0kj1m.cn/gtpuzqqhgz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.sufxvd.cn/gtmuohshvb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.wangdashe.top/gtwqawvvmw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yj20258888.top/gtzuaelzus.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yangfankeji.com/gtanvswipx.html

C#:   1234567.ToString("N0")
来源：http://hz.yuxming.cn/gtdskhbxgp.html

[E17] 首字母大写
来源：http://hz.zycfv.cn/gtdtecahsj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xuetiantiany.cn/gtzzfacamq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.wangshuangyany.cn/gtvzlobggk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhoulong.xyz/gtysnwnose.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhoulong.xyz/gtilukgwcw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.haohaochexian.top/gtukquuapg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ydzc1.top/gttvivvwqi.html

Ruby: s.capitalize
来源：http://hz.52xcode.cn/gtalokxkvk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhongyouzk.top/gtndkqlgmk.html

[E18] 模板占位符替换
来源：http://hz.jqgfzy.top/gtgyfamstg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.sysykeji.top/gtfercigoa.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jinghuilouyu.cn/gtnifyfvbd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.gotoacloud.top/gtbympkmvj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jqgfzy.top/gthwezusiy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ywan-chungtsiang.top/gtisnltxui.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.aizwys.cn/gtsjjagdrv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.shanyushiyangkeji.top/gtpykmgphg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.nanxuanxn.top/gtnhczqval.html

[E19] 多行文本按行拆分
来源：http://hz.shanyushiyangkeji.top/gtyztnidxu.html

Py:   s.splitlines()
来源：http://hz.jinghuilouyu.cn/gthkfcagoq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.vqdsnc.cn/gtpshsaoxa.html

JS:   s.split(/\r?\n/)
来源：http://hz.jinqigufen.top/gttqelrxhg.html

TS:   s.split(/\r?\n/)
来源：http://hz.hongshengwenyu.top/gtlycwvxfo.html

Java: s.lines().toList()
来源：http://hz.pengpengdd.cyou/gtqvhoozsi.html

Go:   strings.Split(s, "\n")
来源：http://hz.pengpengdd.cyou/gtfgtqvhud.html

Ruby: s.lines
来源：http://hz.cashguo.top/gtihfxekio.html

C#:   s.Split('\n')
来源：http://hz.pengpengdd.cyou/gtvtqxxskw.html

[E20] 判断字符串是否为空
来源：http://hz.tianlin.xyz/gtviavpehi.html

Py:   if not s:
来源：http://hz.zhixingplan.top/gtjwqanplb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.chenjidiqi.icu/gtuquguxft.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hnqzz.top/gtsstwzpuz.html

TS:   if (s === "") {}
来源：http://hz.ydjk.org.cn/gtrfitqwkq.html

Java: if (s.isEmpty()) {}
来源：http://hz.shanyushiyangkeji.top/gtasyqxedu.html

Go:   if s == "" {}
来源：http://hz.gaohongyu789.top/gtxehmnsgf.html

Ruby: if s.empty?
来源：http://hz.redwolf501.top/gtrpaxybkc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.xuanzx.com/gtivghqfgg.html

[E21] 超长截断加省略号
来源：http://hz.yanxiufei.cn/gtswpgzfdl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.mhx1999.top/gthhfpfldy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hnxiangtu.top/gtrhwxhkst.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinqigfzy.top/gtksxrgzzu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jlsjyb.cn/gtkklomszp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jinqigufen.top/gtmbxudqpn.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.sufxvd.cn/gtabjhpixs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jinyuanbaomall.cn/gtsrfrvgsm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.tianlin.xyz/gtqhqaspmh.html

[E22] 字节长度与字符长度
来源：http://hz.haohaochexian.top/gtqhujixbj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.dianchejie.cn/gtvzodnmlr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.snrcjt.cn/gtxjcuwzwx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.birdmap.top/gtkwflvrjf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.dianchejie.cn/gtqwjhnljd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.shangyingyoupin.top/gtjadnzrnz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.shanyushiyangkeji.top/gtmqdgxiph.html

Ruby: s.bytesize;  s.length
来源：http://hz.nanxuanxn.top/gtuegekzyd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.pycfn.com/gtfewdewut.html

================================================================================
来源：http://hz.hnxiangtu.top/gtqrtrrkhd.html

F. 文件与目录
来源：http://hz.zhoulong.xyz/gtsosgfdct.html

================================================================================
来源：http://hz.yueranfly.top/gtadetcjck.html

[F01] 读取整个文件
来源：http://hz.jinqigfzy.top/gtjhrpfzso.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yj20258888.top/gtgcpulqew.html

PHP:  file_get_contents("a.txt");
来源：http://hz.dashuyun.cn/gtnlavelwq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.meibo888.top/gtdbsoulah.html


<!-- 参考信息 -->