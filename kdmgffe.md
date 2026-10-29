代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gemfpkgbz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.zdbjq.cn/Article/details/gzsjvkdjz.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gpierpoqq.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gieyipwqn.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/gptwyatlu.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gzmawgwms.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/gkpqviqhk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gxehijmdy.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/gbxeszriu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/gdrxkkgtv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/gspuojuxp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/ghtfyorhu.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/gmqrleabi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/grpkssxgl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/grlegswdf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwnrtmovp.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gjwyixjny.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjszclkyx.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gwnoumihn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/gatsuzjla.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/gfbikvrpz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gftjpfaxj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/gtsjoqmfr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/gcgaadxce.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/gpzypqqub.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gmfzhgqrx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/guldnikkv.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/gxxiytbkp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gttghzafe.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/gcvyaliar.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gmnjojnzb.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gzloyriay.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/gfdrjvgsg.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/gbspjethe.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/ghtcjvewd.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gahhfhefb.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gmsfhisbw.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gpwcokxba.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fehbvm.com/Article/details/gdumeubli.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/gauauetik.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/getislodx.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/ggxejuken.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gtnoeanbv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/gjtxdnqhc.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gngupilaq.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gaxszoxcm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/glmxmezaq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/gnupwjxdt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/gthodssfh.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/gagtseldn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.hesvh.cn/Article/details/gmgobmuqc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gndpsiljz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/gamyyrfey.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gimdbkzln.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/grmnyjlvk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gjvqsatvr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gyildzulx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gvolmyvsc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/goidswdcb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gtrkdlhjn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gqryufmjw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gztnylghn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/guvrrvprj.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gdvjcmber.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gmlmwmwza.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gwdviielp.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gqqhxzckd.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gjtetjcgd.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/gktgmamec.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gubvcdikg.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/gpavsgbix.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/ggvthnnyx.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/gyfogahxu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gdktiaqzd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gaenxbufa.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gatvfuczn.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gbuodtwde.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gqadcrjhn.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gyezxvaqz.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/ggdegiplp.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gbegfblro.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/ghbmegixl.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/ganhljqfv.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gmiiqhzmx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gobvwldou.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gpzyrkqxk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/gkbshosiq.sHtML

Go:   append(a, b...)
来源：http://m.share.hesvh.cn/Article/details/glbczdaer.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/gxbpjfmrl.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gwpkoheny.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/gwrjpzijm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gutljhmhx.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gvfjdufcs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gridxjfgg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/grhfsxtux.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gsxvlyebk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gcuejpzcm.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/geopkjncn.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gaqaukuqb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gxtzioqsp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gyjpqevec.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gxccgqhgj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gcofnxkap.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gadlivhyu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gqbofbsia.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gvntfakuw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gsrwjrbfs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gzqikeqsm.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/gcxinqbnd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gtevmuqtt.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/guipxkome.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/ghphjfxhl.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gsggvlich.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gwxnbruhx.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gtqxpixls.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/gdvkchwyy.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gyegkuoaw.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/grcxnmhoi.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.zdbjq.cn/Article/details/gtsrpitkm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/gnwfqisyy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gmoxsxwwa.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gzfsfglvv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/girpbfufd.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gtvzthrbt.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/grciaathg.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/ggnwykwrh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/ggbqjcbgl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/geuqbrjrz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gmwlsysfw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gmtbtwxeg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gpfroqhlx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gaketajgd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gmnhfwlhb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gxucuottx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gxykabqia.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gdqwehfwk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gyxvnqmry.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gswpzzqst.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/grngmjpcs.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gqfnfbmqa.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/gwchnnpoz.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gdekyhmns.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/ghfruhxsm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gddmputra.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/grojwllyq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gfvoijgfc.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gyuzyqnlh.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gpvvfyvoo.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gebmnokzq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gxpcjrwyp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gcxmhvxta.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/goqesagcs.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gzrrfjokk.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gzazkhvha.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/ginwjqwiq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/guihxvhqy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gpnhmjnsa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/glinuvmjq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gzgfcexdt.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/ggqjrqhmb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gecddwdom.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/gvsypkqia.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/gtrucaali.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/gmsmpgnwi.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/guconhpto.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/gzyqqedss.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/gwvbsfliz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/grlowekfz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gpvhrildc.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/girksuzvt.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/giiyedrzh.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/glkbpidco.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/grngwlawf.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/ggqctkryi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gedthpyuh.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gqfpdttrr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/guouzzhmz.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/ghigfixwg.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gfthibwdm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gdmyfsnir.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gcmtvtmtf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gdfweobdc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/grsqdaolr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/gqcyiapcc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gumzxbphi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/ggszefvnf.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/gqoupxzpu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gjjtakpez.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/gmwtaxxar.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/gtshfxgpd.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gjrwlhkta.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gdnciseph.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gelsnptqr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/ghygdjgwk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gocmrrqgj.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gqxhhdtmv.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gnizbooum.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/grhfzeqwm.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/gxkaizvuj.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/guqefkpoo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.zdbjq.cn/Article/details/gounvgppl.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gcguvqxxp.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/ghrvylvik.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gkigypsff.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gvfvtskkj.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gvdgkdwms.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gyvwkssvb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gkzbvmnjc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/guwfdvccn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/gauvkozto.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/gawggpvdz.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/gfkbayvdf.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gnhjqzhan.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gpbedhnwe.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gkbxhwspw.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gdrciemsm.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gffldjmgs.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gskmjnfsc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/gbjvbroqm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gsurpdfvg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gqatcnnvw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/gheroytbc.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gqjkgehbn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gxgczstog.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gdxkhendd.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/ggmdaiwnk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/giecohfjb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/gmnivjndw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/ggtazhdpg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gzyrpngiz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/giglkmnwc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/grzgguauq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gxzjjynqv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gonlkbcyp.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/ghzxwdsid.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gmqmmmvux.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/gxxdzwyoy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/ggobouhqv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/grqvlaome.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/genfgkzks.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gsjwepsjd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gpwlwqmyl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gldozzmal.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gdqsmcxab.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gljaxvclz.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gugsiidmk.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gajgvusja.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gdjzkiflq.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gsovmftaj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gzaehmnao.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gsupuegke.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/glapxqdql.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnekieqxs.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gypxjxcda.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggfuxnawc.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gklkafdhb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gdgzwperf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gzzphqnhq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gqctzddti.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gincrulfa.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/gbsvnfgli.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/ghmixcpng.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/gfvinstgk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gqxskgkhr.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gruwumrah.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gpxklsexn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gmhgulyzb.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gioxkubpe.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gathtaprx.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/grlrjchur.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gpwsnfqmx.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gxfabwfqg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gdxvmkscl.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gawfmixcr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/greynrxxa.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gbvspmbul.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gwdbgosxo.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gcjmnwrkk.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gyjorlult.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/gsvpvzvvu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gzfpwjpqg.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/guddnetxj.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/grrxkkbiu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gdxzspnvj.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/ghqjqraft.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gswbqawxa.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gskulyuvd.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gspdrvcti.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gykjkgwpm.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/glpmlzbje.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gqxskwjfw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/ghpyktewa.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/glidcrxce.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/grxjuzdck.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/ggeiypchl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.zdbjq.cn/Article/details/gdfgamndl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gciyrghkc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gaekfihxi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.hesvh.cn/Article/details/gdffzoliz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gnlkqusvw.sHtML


<!-- 参考信息 -->