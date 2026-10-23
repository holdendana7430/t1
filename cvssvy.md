代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3vcsfxwnm.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3qkdqhwin.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3hudstufd.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3rdfoausu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ntcdtwgf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3xvqitfha.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3xkzdybgy.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ucrtkhlx.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ovbfxzot.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3tgyynyuo.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3tugjlasg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3pxpygmxa.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3jqxhzzbu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ondrhqbh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3riawratc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3hzokxitd.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3geyweicm.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ubcfrlbi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yarigiky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qgqmprtr.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3navtqjzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ofscsaro.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3bpjqyfza.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3iduilpdu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3lqaubjzy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ygkdollw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3rokbulzo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3wnkvxgyf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3veppyzla.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3vepoyhkg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3mgxfyyvz.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3wcapesgp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3xmlwlvfu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3palrqeal.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3zaucpuvf.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kvuzfqxr.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3eszwjizj.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3woxtfspy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3gzxuhyop.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kmmruukj.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ijaxcyqz.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pdugielp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ygaegvkc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3gtfavzzr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xmnfugls.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3aonwgszr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3efaitvsi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3pcllidzq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xnvlbrhw.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3pjfltrms.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ketdbyqk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3hpduqodh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ocrgypca.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cuiibtge.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zdubntaa.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3cpybyfxm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3iuudzrfo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3gzuactgd.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3rnnxkjph.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3yquaurad.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3npplqlzl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jxntgkzi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3atgoojyl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3yogbyavh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bfxihnrn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dzighgtx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3sxiottdr.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3blcrpgjy.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kmlzztkh.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3apncyxtn.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3rxxrqbvb.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3yjoqfvmc.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3gsgfmwwd.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3yshmhbvv.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3jggwmret.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3ieleefsl.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3msgrvusm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3pjoygqqd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3yvhmmjkf.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vroxuzoh.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ntlzuenv.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3loheqhgf.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3sbgtcdmz.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3jzuuplnw.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jxpoahcg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3jexority.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3goynjzqg.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3trbkhkjh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3eeknrjea.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3knrkiphw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3idqfefpw.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3jdbyywfh.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zyefwbvy.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3thuhytoc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3zdeahmfa.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ehwemdmb.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3tuzxcoqo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3tihwopuq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3vpyslame.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3msirzngi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lgusypps.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fslmymgm.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3qzwvhgmp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3povbiibo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bvowlrpj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3njsmxhkq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3mgutpeje.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3kjhemcmf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3zgeckxfx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3nzllmszn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3hesptxoz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3brsomapd.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3sfdudpbl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3rdfvatpt.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3udhmrzaa.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3tjqmnnoi.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3acbqmmgg.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3mvfbwgab.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gculywyv.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qhfcztmb.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3zlivqayz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3usjvojot.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3vmtmijmh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ftexyibk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lvwiqqfn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3rsecczkw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3rbeyyuhb.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nmdqlvrm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mhncdxry.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3msayigqe.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3xjqmzpli.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3krdzzqlf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vlblelkv.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3qvxcznlj.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3oabqmlep.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3rznusftk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3bjdulfmd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3dohdqnrc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bmuhakmb.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3wqxlwebu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mmunbuar.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3lzixnorq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xtqkcrbs.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3mlsszhsi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cyhavqyz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3wdunxkhk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3utldwhci.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fihstsxu.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ayxmzuma.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mejjqykw.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ivirtaok.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3sztbvfjv.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dvnwpslv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3zxpalbeh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3wuqbprkb.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ibyixgsj.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3myxdbihj.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3uechyccw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qbrbxdjs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3jpylvnkv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tgfqzhkx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ptbqlkfd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3xeuoyrob.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3dasxdddp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3llkvwztb.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3lhvdwcax.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3pjogzmka.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nupzkdwv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ooulnkiu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3ljtnedkx.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zpejkmxr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3tmwmajdm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ahvclbiu.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ksbgdqrt.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3iexigybd.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3yxgmvlcz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3eoymvqbw.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3afsfbdsj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3skpfdzsv.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3agfcgeus.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tulibdce.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3egxubbfg.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3pbujzkfr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bewhlejw.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3kozktfae.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ihtodkdb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3knprjtem.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3lpdmesmk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3vytltmwd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3fbyubsoy.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3jjnftpbh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3fznghlrv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3fidwdcfm.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3nkunhcow.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pxdufkud.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bjecbegm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3miutatzo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3liypklbv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3enmebypf.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3glrzcncs.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3lpyalvyy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3watxcacm.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3cyuibtot.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3omwweqne.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jokdjpfc.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zzqpoyso.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hjdylaql.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gflwkbnz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hiopclbv.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3qwkdieoe.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lmihyfcl.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3nsfnndau.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3yyxouoon.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3wrxredwb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3fmcuiadv.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3onfltjqq.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zfzkmswy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3mnykwqof.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3jdlxmelg.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3sbgzhpey.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3qybusvqv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3cbchutyk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mxzjimnj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3qgwuurzb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ygcsdszp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3kcqzhgfs.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3murfkwej.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3qajxaxmq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3zjmldyed.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3tdvrjmgw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jkzxopyt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3vwxtcgji.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3xtijfacf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kcehpmcw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3wznhlvrp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3lhffnwdm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3swkndkpu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3asgsvbdy.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3zrlgszmr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ztjmnvrf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3dmwsbudi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ernuejou.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3bpriersz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3vnogveep.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3qtmubrlt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3fhcrmnft.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kxgsykss.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rvweppem.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ukzqeern.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xbyrtzal.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3spqeyksy.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yigcgiho.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3yjvzwwdj.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dlitvexe.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3pnlyaldl.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3lwfpvcpb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pcensoff.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3ckwojujj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hqpmrdyd.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fagzbzsq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3nuiblxvw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rdpfftjn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qeigzjvp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tzzjbhla.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3jvafrtqr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hwvodhnb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3sakhqpqf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kxionjlo.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jzsiifhl.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3nigxfasq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3blkldzil.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vastvyle.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ywsgwski.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vjxjkhiq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ofakgzni.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3qfvxypxd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ljrntaub.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3eevxglvs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3vkunfkxq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ifxctdit.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gmmrxxii.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qseiikeg.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3cmidfxpg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3sznumuce.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3jcxyxiut.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3ofxdkjjg.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3pnziqfjx.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3kcwgqgbh.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3jpkonotu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3yzxlzfqc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3liysynhn.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jqdhiyej.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3pdnyaddp.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pwlydckg.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3aodyimka.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3uxnxozef.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3dyfthrdg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3igtwdvpg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rbxjgwpg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3sbrfcfrc.html


<!-- 参考信息 -->