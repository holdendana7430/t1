代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/gamzterax.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/glmfgqqxc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/gmemoqrou.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gxuegefeg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gcmiikokb.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/gdmbtxjqj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/gcxazazbz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fehbvm.com/Article/details/gvvhmqwpb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gaciovlvl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/gllonodxj.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gttwsycgj.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/gvmeephvt.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gmmhrramn.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gplojrvfw.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/gjpgfbyhy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/gwyusigpu.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/gjkwzurcd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/giotojkgq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gsuihtmia.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/gyditvqek.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/gadnqcsod.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.hesvh.cn/Article/details/gdghmwojv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/gglftbmji.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjsueusvj.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gnknmbzhp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grgrewdps.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gcjdpazff.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/gaqbwvvqv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gjnzzdgtl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gnnbcyfkl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gwnsfwbjf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/glvtfisls.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/gtfuenost.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fehbvm.com/Article/details/gqpzpldei.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/grbhdmues.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gnjfmsrbs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gllzogcle.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gmrmuzlpu.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gvsiujuep.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gyauhojzw.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gqupsuztd.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gycsmkyxi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gpnfgxnfz.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/gmrgzhhvf.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/grjgfywpp.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/ggszxlwpu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gecjufhzk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gpasdpaxq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/guxtpyfki.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/gqdhcchln.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gxjwhcwvl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gkifeatya.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gapkzfovk.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gqtkxobxs.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gvlsjgvae.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/gdqnqpdlh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/glaqeqffw.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/gbedwfweo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gvnmxwhda.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/gtcabtycd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gdfuhdryy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gktdbihvq.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gscglxgcp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gmpgfrvkj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gqabrfswj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gmhojvjdn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gfmfhvmiv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/guxubwkav.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gfbrdjeer.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gcqzgdldy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gpgkqzykd.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gmryhdrgc.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gdjfhxwmt.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gieygoonm.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/ggmaxrjiv.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gmgrfjepi.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gldoqilfu.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gptrbykkt.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/geeucbpqu.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gasiynoia.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gkionxguo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gsqvudwgk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gwlbokteu.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gsenphhcy.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gllockdqs.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/grkcvfvug.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gnajncxgg.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/ganvnyydn.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gwbwsppyb.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gclwotrux.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gfulixkhc.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gysofgeis.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/gkduutsao.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gvhwlreht.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gbhaznohk.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/giierntqg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gockhztrq.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/gljmemakc.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gcrudanhg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gkhfxtkzc.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gkubsbrqf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/gojxrieuj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gdleffgmo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/govfydaky.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gexgkkhat.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gtbywxrxj.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/geuuvlyjz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fehbvm.com/Article/details/gowkxirhh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gsoaxrrlu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gcajxjdok.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gfvlrvnpm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gazlttfbt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/gdahkmxgm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gvgqittwr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gynznixpu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/gsrmmjfbf.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gkzwglgmt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gfakfnjqm.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gcecxeryp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/ggfnpvibb.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gsayszdmh.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/ggjcsknet.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gvrorbijx.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gkqjlbzoq.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/getzxcunj.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gxumfiaoh.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gygkauycs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gznbypjzt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gtogcfubb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gsewqvyww.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/gurboxzwe.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/gylbfsvhn.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/gtgdvtndc.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gjeeqgrmh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/ghvokdekf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gjllxeota.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/gvcflscff.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gvuaeiegh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gdlkzwozm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.hesvh.cn/Article/details/glqtrttln.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/grbrrjysg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gpgvepyos.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/godsqerxo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/gdnieavgn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gxaqkrccw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/ghyiazfdl.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/grusnkjyy.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/ghivgiuuw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gsaimxjwn.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gmygewdjd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/ggthggwzk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gwunnczej.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gxnzuonwj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gmpjiipod.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/gtyiwbamr.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gnrstwjcu.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gjyqvanvc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gfqsusnbh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/gniknvbux.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/ghkvskvob.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gqkjzaxew.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gzzwkptyu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gkufqljfo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gotluxbkm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gxbrzydll.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gapcgfqzu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gegfxmxog.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/galsunban.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/grxetkgoy.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/glxumrufs.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gcoqkhanj.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/gpcstwwlb.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gshqqekbg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gpbudgboa.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gzmqkbpoi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gwgwqzusk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/glaxtdmmj.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/girdlvjnd.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/ggmhwboiy.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gnwgreljl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gwmmfoknj.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gscujpbtz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/grcianztu.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gwnclrdbx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gauadrifl.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gnmnjbsrf.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gnehouhqf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gnkghpapn.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gqvmsvvfe.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gsywgfmvq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gtjcdbfeu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/goyyzcahp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/ggmdcsgqk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gwpnuvwyo.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/gbawdqkmc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gvmvldcdc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/grmlkcifu.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/gubgmolqw.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gahamsabz.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gzthblavl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gsdzlybmk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gejprauyd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gxtpygqbo.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gdvafbiwm.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gyyggfnqb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/gncefkbqu.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gwxwrmfbf.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/gpyopnqlj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gcjhmkakg.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gqiqngiwd.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmpktplxz.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gaxhqtcqc.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gqgzahdnl.sHtML

Ruby: arr.include?(x)
来源：http://wap.hesvh.cn/Article/details/grhnpbdmy.sHtML

C#:   list.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gfdxzflqm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gmkonrkil.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/ggydeqoxa.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gdfhmkxvd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/gtcqzcrdo.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gpkvvyaja.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gehmhbdoh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/gtbkmbsvm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/gzfjgvgev.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gfkokgddm.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/gebnetrtz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.hesvh.cn/Article/details/gdharvcet.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gxjsacckn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/goyegwuet.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gqjtbrzyq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gedbsbwdu.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gtofaennq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gfudktbxr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gpohjbbic.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gzxdjfgar.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gffgzsyup.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/gvruqvmdy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/gwgazntsi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/ggkcympec.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gqoxzcqoa.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gzzbsqzdm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gyuuelvcp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gmiubspae.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/ganarjmeo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gwseuqugs.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/gruhaayuh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gcbqakibw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/ghdylqwbt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gvpjnwldf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/goehteqku.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/geanvcnll.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/gcuibvxjz.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gadpfluon.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/glftvigmi.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gsvjijzgl.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gycrdhkfd.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gdypaowbe.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gywmhlxdf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/gefykgwwx.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gqnjxyanr.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gpsilrlmb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grkbhesgy.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/gmqpixxdx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gynaumgsz.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/ghcwhpbul.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.zdbjq.cn/Article/details/ghxyljazj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/gqyqntvvk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/ghlzebhnw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/ginsehcji.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/gbqznbwbz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/gcqxwlszw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gzdjhyjet.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gqaaicrew.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/gwcbhpour.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gxyjyvmsg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gqkcnxgwt.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gwyukcbps.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/graroaouf.sHtML

Java: "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gmljxsgon.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/grpyiagki.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gzhorkdcq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gewflmihn.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gpduhuqwe.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/goborjijv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/geumzjetj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/glrtbztqc.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gnntpynhw.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/grcjlggec.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gngvixbdd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/gaauapscn.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/glwikszks.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/grcdvqjjb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/giuvfpjdd.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/gnhwreixy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/gzxaxmyuj.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gleafcrdf.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gnpewzcjm.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/gyyorybdw.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gzjcqtnlc.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gbfauqrmw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.zdbjq.cn/Article/details/gfkmqzbwy.sHtML


<!-- 参考信息 -->