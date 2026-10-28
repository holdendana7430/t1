代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhoulong.xyz/gtxonjcdkw.html

Go:   // 手写循环
来源：http://hz.tanke756.top/gtgctulezv.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yuxming.cn/gtaffmglms.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.quarkkingdee.top/gtehykhtsz.html

[D15] 去重
来源：http://hz.cqqwz.cn/gtassoaqha.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ydjk.org.cn/gttndhumez.html

PHP:  array_unique($arr);
来源：http://hz.xziqi.cn/gtyhybvyum.html

JS:   [...new Set(arr)]
来源：http://hz.gaohongyu789.top/gttyqufxeb.html

TS:   [...new Set(arr)]
来源：http://hz.yuxming.cn/gtexeqrtdo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.shangyingyoupin.top/gtiprqmqkm.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yanxiufei.cn/gtxvwprggh.html

Ruby: arr.uniq
来源：http://hz.jinqigufen.top/gtgyuuonyq.html

C#:   list.Distinct().ToList()
来源：http://hz.yanxiufei.cn/gtqwbwaehl.html

[D16] 求和与平均值
来源：http://hz.jinqigufen.top/gtqyjvucxt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.chenjidiqi.icu/gtixucpywj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yuxming.cn/gtosbwghlu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gaohongyu789.top/gtqagvvhck.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yuxming.cn/gthhconuwa.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jinqigfzy.top/gtiglfjshf.html

Go:   // 手写循环累加
来源：http://hz.aizwys.cn/gtvutttdqw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.chenjidiqi.icu/gtoepsblje.html

C#:   list.Sum();  list.Average()
来源：http://hz.smart0.xyz/gtufeelenj.html

[D17] 最大值与最小值
来源：http://hz.aizwys.cn/gtipoaxvqc.html

Py:   max(arr);  min(arr)
来源：http://hz.meibo888.top/gtqzviounf.html

PHP:  max($arr);  min($arr);
来源：http://hz.ybcxt.top/gtzvaegisq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.tanke756.top/gterrhtbft.html

TS:   Math.max(...arr);
来源：http://hz.wangdashe.top/gtulpgtkcd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.c1oappe.top/gtudvxzfzg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.vqdsnc.cn/gtixyrzavy.html

Ruby: arr.max;  arr.min
来源：http://hz.9152youxi.cn/gtqyqborkc.html

C#:   list.Max();  list.Min()
来源：http://hz.meibo888.top/gtcubsbvzw.html

[D18] 扁平化嵌套数组
来源：http://hz.cucudq.cn/gtmfmccttu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hfpthk.cn/gtoyyibgrv.html

PHP:  array_merge(...$nested);
来源：http://hz.chenzaomai.com/gtkbrvroir.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yangfankeji.com/gtojdsxeuu.html

TS:   nested.flat();
来源：http://hz.hysaishi.cn/gtsnytocsm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.snrcjt.cn/gtbfkwgjqs.html

Go:   // 手写双层循环
来源：http://hz.gaohongyu789.top/gtuxodlzsi.html

Ruby: nested.flatten
来源：http://hz.jlsjyb.cn/gtbjomoogl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.shuidangran.top/gtfzwuvzsd.html

[D19] 按字段分组
来源：http://hz.vqdsnc.cn/gtyzfnhhci.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.chenjidiqi.icu/gtvnistyao.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ywan-chungtsiang.top/gtgtoyaxgt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.0kj1m.cn/gtgtsrhxpk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xuanzx.com/gtjlmymbku.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.sufxvd.cn/gttjhvtswg.html

Go:   // 手写 map[string][]T
来源：http://hz.fengsongda.top/gtyavrllix.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.guowangkeji.top/gtqmuwvlia.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zdqjudy.top/gtompshxsz.html

[D20] 统计每个元素出现次数
来源：http://hz.cashguo.top/gtonuidmww.html

Py:   Counter(arr)
来源：http://hz.zhoulong.xyz/gtqflluahw.html

PHP:  array_count_values($arr);
来源：http://hz.zhongyouzk.top/gtnfcrbkes.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.daxiang520.top/gtfwmttmcf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jqgfzy.top/gtpygyuefn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.iojbl.cn/gthfyaxghu.html

Go:   // 手写 map[T]int
来源：http://hz.316326.xyz/gtalebgvtj.html

Ruby: arr.tally
来源：http://hz.pycfn.com/gtcnzmslem.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ydjk.org.cn/gtejeocvjd.html

[D21] 判断是否包含某元素
来源：http://hz.yvedp.cn/gtjtcbrqva.html

Py:   x in arr
来源：http://hz.yanxiufei.cn/gtggppbkje.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cashguo.top/gthlzjfrri.html

JS:   arr.includes(x)
来源：http://hz.meibo888.top/gtdrjvsvdh.html

TS:   arr.includes(x)
来源：http://hz.sxryk.cn/gtgzinyzbt.html

Java: list.contains(x)
来源：http://hz.yanxiufei.cn/gtdxjrjnrj.html

Go:   slices.Contains(arr, x)
来源：http://hz.tanke756.top/gtlwfybien.html

Ruby: arr.include?(x)
来源：http://hz.tianlin.xyz/gtwolxydnc.html

C#:   list.Contains(x)
来源：http://hz.dashuyun.cn/gtzgkbazyf.html

[D22] 复制数组（避免共享引用）
来源：http://hz.havefunace.top/gtzcecldzs.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.svipenyu.cn/gtpweyrcdl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.iojbl.cn/gtxmjqikku.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yvedp.cn/gthvqzruhw.html

TS:   [...arr];
来源：http://hz.shanyushiyangkeji.top/gtiqsoooup.html

Java: new ArrayList<>(list);
来源：http://hz.pengpengdd.cyou/gtaminzhbs.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jinyuanbaomall.cn/gtgyoadxok.html

Ruby: arr.dup;  arr.clone
来源：http://hz.birdmap.top/gtqmblfgfa.html

C#:   new List<int>(list);
来源：http://hz.guannengcc.top/gtjumqqfru.html

[D23] reduce 累积计算
来源：http://hz.haohaochexian.top/gtsytuqyxr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ehwqpu.com/gtqckekbno.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zdqjudy.top/gtogsgjukt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zdqjudy.top/gtnjglxfxc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinqigufen.top/gtbslfddtd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yj20258.top/gtggtimnlx.html

Go:   // 手写循环
来源：http://hz.ybcxt.top/gtllaqnqsu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.wangdashe.top/gtzohkgbrx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.aibaodan.cn/gtymcjrwgz.html

[D24] 字典 / Map 基本操作
来源：http://hz.xziqi.cn/gtrmxtudui.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yj202588.top/gtbrkovcqw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xinyue.icu/gtyzygzaie.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.gzhubu.top/gtpcdzmfcl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ppjwa.cn/gtjxstjezk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jinqigufen.top/gtuzlihiiq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ybcxt.top/gtdtfounzg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.wangshuangyany.cn/gtzlbpvkpb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.fengsongda.top/gttbxuwxmk.html

[D25] Set 集合去重与交并差
来源：http://hz.haohaochexian.top/gtjdrkwrcu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.gaohongyu789.top/gtaezpvoad.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yueranfly.top/gttyqnkkpt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.316326.xyz/gtkjmvbakj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yanxiufei.cn/gtfezfiriu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.snrcjt.cn/gtcgzjchgy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zhaomingkeji.xyz/gtuwpiqyza.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jinghuilouyu.cn/gtsbthgjfy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zycfv.cn/gtsehmbjbr.html

[D26] 数组转字符串
来源：http://hz.ivvv.top/gttxjwayvm.html

Py:   ", ".join(map(str, arr))
来源：http://hz.52xcode.cn/gtrdpqcwiy.html

PHP:  implode(", ", $arr);
来源：http://hz.9152youxi.cn/gtxvuajnhh.html

JS:   arr.join(", ")
来源：http://hz.iojbl.cn/gtobkjsihh.html

TS:   arr.join(", ")
来源：http://hz.fzhhl.top/gtxazebgun.html

Java: String.join(", ", list)
来源：http://hz.gogol.net.cn/gttsqxxgpz.html

Go:   strings.Join(strs, ", ")
来源：http://hz.52xcode.cn/gtzybvzhim.html

Ruby: arr.join(", ")
来源：http://hz.hnqzz.top/gtujqadhmt.html

C#:   string.Join(", ", list)
来源：http://hz.ivvv.top/gtqgnwzzhn.html

================================================================================
来源：http://hz.hongshengwenyu.top/gthggavdbh.html

E. 字符串处理
来源：http://hz.xingfuxueyuan.xyz/gtyyqvrlgm.html

================================================================================
来源：http://hz.kuanghao11.cn/gtrocvwilq.html

[E01] 拼接字符串
来源：http://hz.guowangkeji.top/gtirsmudas.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.xingfuxueyuan.xyz/gtxkfcjpse.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.xuanzx.com/gtqsnwptqx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.0kj1m.cn/gtibkiscts.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinyuanbaomall.cn/gthoevoaus.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.guannengcc.top/gtxesmgvre.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.aibaodan.cn/gtfymynklv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhengqikj.top/gtparrduou.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yonumen.top/gtikrafmyo.html

[E02] 重复字符串
来源：http://hz.0kj1m.cn/gtgocvfuxj.html

Py:   "ab" * 3
来源：http://hz.xuanzx.com/gtqerpopgh.html

PHP:  str_repeat("ab", 3);
来源：http://hz.bjfxy.top/gtumyvexnb.html

JS:   "ab".repeat(3)
来源：http://hz.hongshengwenyu.top/gtzrkpgocu.html

TS:   "ab".repeat(3)
来源：http://hz.gaohongyu789.top/gtqtwgoyxt.html

Java: "ab".repeat(3)
来源：http://hz.yvedp.cn/gtdqucwlyp.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.vqdsnc.cn/gtzsyrhpbl.html

Ruby: "ab" * 3
来源：http://hz.fengsongda.top/gthppwptbw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.haohaochexian.top/gttfzyskpz.html

[E03] 截取子串
来源：http://hz.cucudq.cn/gtwiolulwl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.smart0.xyz/gtdpplgiqz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.snrcjt.cn/gtafqpidwe.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.hysaishi.cn/gtdzxmwshh.html

TS:   s.slice(1, 4)
来源：http://hz.yj20258.top/gthaolpfej.html

Java: s.substring(1, 4)
来源：http://hz.andypj.xyz/gtuycjqfmq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.iojbl.cn/gttfwthoev.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jinqigufen.top/gtvkvwsrok.html

C#:   s.Substring(1, 3)
来源：http://hz.zdqjudy.top/gtjygtyzll.html

[E04] 查找子串位置
来源：http://hz.tianlin.xyz/gtwzqlxmft.html

Py:   s.find("x");  s.index("x")
来源：http://hz.snrcjt.cn/gtoibgrrtf.html

PHP:  strpos($s, "x");
来源：http://hz.jinghuilouyu.cn/gtowepvhgn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhaomingkeji.xyz/gtdplbftnw.html

TS:   s.indexOf("x")
来源：http://hz.jiagoushi.top/gtvflszcgl.html

Java: s.indexOf("x")
来源：http://hz.andypj.xyz/gtejvednet.html

Go:   strings.Index(s, "x")
来源：http://hz.yongpay.top/gtnfmvheqo.html

Ruby: s.index("x")
来源：http://hz.316326.xyz/gttwoudcec.html

C#:   s.IndexOf("x")
来源：http://hz.aizwys.cn/gtuqsbmbdh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.cdnleiting.top/gtwdqnkgcs.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ivvv.top/gtpqheppws.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.gogol.net.cn/gtkeuccmjd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cdnleiting.top/gtpdupwemf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhongyouzk.top/gtrxyuztwq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jyoumei.cn/gtzrxzgjug.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.c1oappe.top/gtehmklzyg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jlsjyb.cn/gtbfvznfkn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.cqqwz.cn/gtfimxkmld.html

[E06] 替换子串
来源：http://hz.zhiwuduotai.top/gtungnjiaw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yongpay.top/gtwhojacqe.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.tian-w.cn/gtqnbrzxre.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shzxlz.cn/gtxqqbltnn.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zycfv.cn/gtoyrjxawq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hammf.cn/gthksaetrs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.xingfuxueyuan.xyz/gtbmzmwjly.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.tian-w.cn/gtnefkwanb.html

C#:   s.Replace("a", "b")
来源：http://hz.shzxlz.cn/gtnvzpgryo.html

[E07] 按分隔符拆分
来源：http://hz.daxiang520.top/gtcaxkpoai.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.aizwys.cn/gtgcmdwdph.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yuanzhike.top/gtejzxhixy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.bjfxy.top/gtewcsomvl.html

TS:   s.split(",")
来源：http://hz.hongshengwenyu.top/gtjqnpnmdt.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yj202588.top/gtnktxttwz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jiagoushi.top/gtfwsacnhl.html

Ruby: s.split(",");  s.split
来源：http://hz.hnqzz.top/gteeouvtmc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zhixingplan.top/gtjyxxswmp.html

[E08] 数组按分隔符合并
来源：http://hz.yongpay.top/gtutjupchi.html

Py:   ",".join(items)
来源：http://hz.sufxvd.cn/gtmtzymmeu.html

PHP:  implode(",", $items);
来源：http://hz.jyoumei.cn/gtztxttufh.html

JS:   items.join(",")
来源：http://hz.ybcxt.top/gtjhghvbai.html

TS:   items.join(",")
来源：http://hz.fengsongda.top/gtdncskohl.html

Java: String.join(",", items)
来源：http://hz.yvedp.cn/gtvndlmbqt.html

Go:   strings.Join(items, ",")
来源：http://hz.316326.xyz/gtjgyidggg.html

Ruby: items.join(",")
来源：http://hz.yongpay.top/gtmaupncvf.html

C#:   string.Join(",", items)
来源：http://hz.ydjk.org.cn/gtyfvmwvgy.html

[E09] 去除所有空白字符
来源：http://hz.ehwqpu.com/gtrkjsnvde.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.andypj.xyz/gtynvwsbvp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.aizwys.cn/gtectkztqj.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.fengsongda.top/gtlbqvkwkg.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.daxiang520.top/gtzhdzbrdn.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hysaishi.cn/gtrziafphn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.andypj.xyz/gtdvwajrzo.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.pengpengdd.cyou/gtswjhdwjd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ivvv.top/gtggeqqtrw.html

[E10] 左侧补零 / 定长填充
来源：http://hz.meibo888.top/gtmhavtjji.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zycfv.cn/gthqvdkikf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhaomingkeji.xyz/gtiquilbns.html

JS:   "7".padStart(3, "0")
来源：http://hz.shangyingyoupin.top/gtbtfcysfd.html

TS:   "7".padStart(3, "0")
来源：http://hz.xylfe.cn/gtlsylfzao.html

Java: String.format("%03d", 7)
来源：http://hz.haohaochexian.top/gtdwnbqtcu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jiagoushi.top/gtydasfxfq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.hnqzz.top/gtuzcazmgd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.feifeiyinyue.top/gtuxupnygm.html

[E11] 反转字符串
来源：http://hz.tian-w.cn/gtxdntlgaf.html

Py:   s[::-1]
来源：http://hz.hywenlv.cn/gtvxwqrlgy.html

PHP:  strrev($s);
来源：http://hz.ehwqpu.com/gtmfyxzzro.html

JS:   [...s].reverse().join("")
来源：http://hz.jinghuilouyu.cn/gtqbguhuaa.html

TS:   [...s].reverse().join("")
来源：http://hz.vqdsnc.cn/gtzrvwxzrf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.nwbrower.top/gtqldutwna.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.0kj1m.cn/gtsdwlbkrj.html

Ruby: s.reverse
来源：http://hz.jiagoushi.top/gtaixwnprw.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.9152youxi.cn/gtvxxnvwqz.html

[E12] 统计某字符出现次数
来源：http://hz.gogol.net.cn/gtaaryutpn.html

Py:   s.count("a")
来源：http://hz.zycfv.cn/gtstsbqlbf.html

PHP:  substr_count($s, "a");
来源：http://hz.havefunace.top/gtrqcwromn.html

JS:   s.split("a").length - 1
来源：http://hz.zhoulong.xyz/gtvubfcdbp.html

TS:   s.split("a").length - 1
来源：http://hz.nwbrower.top/gtkvlrzoot.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhoulong.xyz/gtfuqmetmh.html

Go:   strings.Count(s, "a")
来源：http://hz.zhoulong.xyz/gtvabfejiw.html

Ruby: s.count("a")
来源：http://hz.jqgfzy.top/gtvhgyywms.html

C#:   s.Count(c => c == 'a')
来源：http://hz.316326.xyz/gtmasueqjl.html

[E13] 逐字符遍历
来源：http://hz.gzhubu.top/gtxrkdqofc.html

Py:   for ch in s: print(ch)
来源：http://hz.andypj.xyz/gtgpawfhwu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.fzhhl.top/gtffyzyqvr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yuxming.cn/gthnczeraz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hnqzz.top/gtiwqxlggb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xingfuxueyuan.xyz/gtsbizelen.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cucudq.cn/gtpgsodirk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jyoumei.cn/gtlwehzxab.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.xuetiantiany.cn/gtxlscnutr.html

[E14] URL 编码与 Base64
来源：http://hz.havefunace.top/gtdpardlww.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jlsjyb.cn/gtocdslksv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hnxiangtu.top/gtvbjocwkw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.cucudq.cn/gtpxktfxet.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cheryme.top/gtyjqrzejn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yj202588.top/gtvihfmqun.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.bjfxy.top/gtvaqaibwu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jyoumei.cn/gtrmclfmsl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.aibaodan.cn/gtswahahvx.html

[E15] HTML 转义 / 反转义
来源：http://hz.snrcjt.cn/gtcbaslmwu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xingfuxueyuan.xyz/gthmqthpcb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hnxiangtu.top/gtrgoosgoc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.birdmap.top/gtrgdlulam.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.shuidangran.top/gtzeepjdyp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jyoumei.cn/gtqwlnaxry.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.gzhubu.top/gthzvjyyfe.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.sysykeji.top/gttagyxqtu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.bjfxy.top/gtdurfioak.html

[E16] 数字千分位
来源：http://hz.fzhhl.top/gtqaxkluqm.html

Py:   f"{1234567:,}"
来源：http://hz.birdmap.top/gtgvprvsss.html

PHP:  number_format(1234567);
来源：http://hz.aizwys.cn/gtsusrgcne.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hywenlv.cn/gtfipvaioq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.0kj1m.cn/gtsqmbfspo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.havefunace.top/gtaoknmtyt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hysaishi.cn/gtsqrhvbje.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yonumen.top/gtvykfqhyj.html

C#:   1234567.ToString("N0")
来源：http://hz.jinyuanbaomall.cn/gtbeksjxzr.html

[E17] 首字母大写
来源：http://hz.yuanzhike.top/gtyjmowlbj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.ydjk.org.cn/gtrmpgjqqo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zdqjudy.top/gtvdrtqobv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydzc1.top/gtkjuwyppz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.52xcode.cn/gtbzatykto.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.daria6918.cn/gtdtzaniyf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shzxlz.cn/gtdhbefodz.html

Ruby: s.capitalize
来源：http://hz.aibaodan.cn/gtnoqrctrx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.0kj1m.cn/gtsyyljmgy.html

[E18] 模板占位符替换
来源：http://hz.hnqzz.top/gtajmoneat.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xuetiantiany.cn/gtdkjnjfwa.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.chenlongwang.top/gtvzwcshfo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.gotoacloud.top/gtxqglpnwm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.havefunace.top/gtlvhkoebc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.wangdashe.top/gtdbodsauk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhijiandao.cn/gtecrgvmfn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.meibo888.top/gtrmforqvt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yuxming.cn/gtuihrjqmb.html

[E19] 多行文本按行拆分
来源：http://hz.xingfuxueyuan.xyz/gtmtwjxknx.html

Py:   s.splitlines()
来源：http://hz.shanyushiyangkeji.top/gteycockay.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.fzhhl.top/gtrfavxhuz.html

JS:   s.split(/\r?\n/)
来源：http://hz.nanxuanxn.top/gtzcyuylen.html

TS:   s.split(/\r?\n/)
来源：http://hz.dianchejie.cn/gtbixzgjja.html

Java: s.lines().toList()
来源：http://hz.hongshengwenyu.top/gttlwvvnmd.html

Go:   strings.Split(s, "\n")
来源：http://hz.yj20258888.top/gtodzpakmj.html

Ruby: s.lines
来源：http://hz.yuxming.cn/gtajtmycof.html

C#:   s.Split('\n')
来源：http://hz.shuidangran.top/gtlkabssrr.html

[E20] 判断字符串是否为空
来源：http://hz.jlsjyb.cn/gtirmdmynq.html

Py:   if not s:
来源：http://hz.xinyue.icu/gtpqpoyujv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.nwbrower.top/gtdijyuvhg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yueranfly.top/gtwvbjvavt.html

TS:   if (s === "") {}
来源：http://hz.xingfuxueyuan.xyz/gtltqirdgw.html

Java: if (s.isEmpty()) {}
来源：http://hz.ppjwa.cn/gtxkohcivw.html

Go:   if s == "" {}
来源：http://hz.andypj.xyz/gtcvgtltfb.html

Ruby: if s.empty?
来源：http://hz.chenlongwang.top/gtmaaeulcn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.tanke756.top/gtwdpgudjw.html

[E21] 超长截断加省略号
来源：http://hz.xingfuxueyuan.xyz/gtriqvcatp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhiwuduotai.top/gtctwbhamz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhoulong.xyz/gtcbzigijz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.haohaochexian.top/gtlpfwqfrw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinqigfzy.top/gtaifqzomj.html


<!-- 参考信息 -->