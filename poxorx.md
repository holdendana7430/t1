代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2bgoewwku.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2cgjlgpkv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2vtxmlkqy.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ykqbffgs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2jriuikdr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2jkystwrs.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2udgtrhcy.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2okozigeo.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2xuomjqxd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ecihdzas.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2rncwsawx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2bebqcisv.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2lvqerqiw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2yjfomhje.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2sfukxlzw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vdrfqgjh.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2mbymbzaj.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2qvesktdc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2oqmyzase.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2emuhxtxn.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ezfmksnb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ypcrgame.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2aqrbcnlh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2nejuwyzu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ofkyittt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2zbanqcsa.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2cdhoieji.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2mflzcrra.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2fdsobmyo.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2qxlydizx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2urqmogkm.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2nrlaqtpb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2pdhitagx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2chycuibb.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gqlhhceq.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ltbbhslv.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2wwchfuci.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bfzynass.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2dyounwzr.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2epenbxag.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2mlngqfir.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2jcipbnvi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2bpsigisz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2xqqxisxg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gaistywi.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yocclhea.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2iisgjhzx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2iwruwvvm.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2asxkceyi.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2fwehyfhw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2qmkhyzfa.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2dcauiqhu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2xuukvpwa.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2lzyrzsrb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2obxxomam.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2tqadjddc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sgknmkti.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2yygbeimi.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2wuwsxnte.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2teweianl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2aadkflga.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kkryacac.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ndyttkmi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ncxyunov.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nyfdgsdr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wrgixohd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ecpdulie.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2morzxwtc.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2qanucrem.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2iijfaixd.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2zkrnxigo.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2frnqwzvx.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2cysawkve.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hcuexcmm.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2zsawkjtt.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2mzohuols.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2gddlihwc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2vaepmzvv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2rzoxshdf.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qshszgjd.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gbuuqokq.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2odlgshqf.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2qjqadjai.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2nogigrvs.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ifpzapoq.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2nolhtlib.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ggedvuwe.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2qtxpppfl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2imtajqfj.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2uwpukhph.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2wpvbbgcq.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2jspbgkhg.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wyyonfvs.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2osogjyiq.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2bnsqrcuw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2fgcizfzf.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vsjonepm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2hlnmzsgy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ywkmyxqc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2peiltcum.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ovyhvprh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2jauyvmzk.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2eytuaujs.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2vfrengpl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2rqqnhbkm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2viundqsk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2bmmbvpyj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2myovjtrb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2cgrjegzk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2vfeqeyzx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2eiojrcaj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2xgterute.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2iyycsfvm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2nilcbzvl.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mualtpaq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2nvzdbgit.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2yecpwxbt.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2orfouyqt.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jtibxewp.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2eawufsvg.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2vlgjoxgb.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2jxduiwsb.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2pximaegv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2gngyiqtc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wioccmmi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ktaplmvn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2uuesfsop.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sstiecgd.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yhaeazsz.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2dlgshnlw.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2bhvpwpgm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qlzmubrz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2fhtxnaog.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gmrohzhx.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2lfhsdmdp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2yuivvuqc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ztgngfdi.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2itohmofd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2epxhjzec.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2fktwnlsy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2kjebzrml.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2epthhtuj.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2slojxnhv.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2coyauvas.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sxxxsyxq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2uikcmqcw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rmspgqoa.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gvcyxnrn.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2udqenuup.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2zxmvlnrm.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2lmlifzgf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2uumwwqon.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2duteewqc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2uhlbrjnq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2yxgkzyau.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2suroxomu.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2izvrgvsg.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2wamqvuxk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pocuohzg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2bxndrvgr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2briwgmxn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2wzgtsilw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2typzcpcx.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2uirinjfg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2pxydszvp.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2zpzjgyre.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2jhtnjmqb.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2dqndfbml.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qfjjudnn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2obbvmccv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ymlpuuiu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qfxbqvgo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pxhobcoe.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2bydtkimv.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2rvdktvww.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2zlirwoqp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2kgigskzb.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2kebfoalt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2fogbaeba.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2hlegfwql.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2aqnsvcqc.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2orbzxnnv.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2leshvejv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rknnujnr.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2dutvfrst.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nglxovmv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2inpydbsu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2gycydbax.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2nvoiopnx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2eugktuec.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2vsmhcxid.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2nbkjocky.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ziwbqfyi.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2cemihmma.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jdxqgnak.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uejixhbw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2heamzggf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2lfllbwex.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2bouilokn.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2pxarctec.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2jozhdzva.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2lqofdvlk.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2yjotgyxw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2eetopwmt.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2nmgycvrp.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zsypsrfh.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ifwljjrd.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mlekxgdi.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lecoaaym.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2scxkyvyc.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wfbiscyz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2gsvmqhuu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ilwbfvlu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2flvsynjt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xdukgion.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2gouvkvwc.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2mxslgtpy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2epthcsot.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2hpcnalfr.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pfvlpxkz.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2mcxntnnx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2keqmxuhs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2pnykupmo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2wnidobuh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2wyfpedxi.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2utjjbubw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ahrliuoo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2mftfgjbz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2xoowaxps.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2upokiaat.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2uwbwsmkj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2wkrpswfk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2bgqwistf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2yeesyspm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2dnontqql.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2dibsctbz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2kcycjnzw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2jvdkiguc.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2hoiiaouj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2zqsgywad.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2iqicifji.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ymidktbk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2wcbdeidj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lzorgrto.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2jkgfryrx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kvetoyuk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cagshmht.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qkflwohg.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qywbyvwk.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2tvxbevsi.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2lokotghc.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ludcdjlu.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2bbygknxq.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2cnsqxzae.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2lorhplly.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2lrldxtnb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ndlftngo.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2tdmuhnrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cqtrolfw.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rxfswjkg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2lxxbzsav.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qxtakbwq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2btkwpzes.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zaozzmpa.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2fqtxrezv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vnrbdldm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2vaavjono.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pwqxwysm.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2bqyckkzb.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2imbhkkvk.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2zvxlfdfm.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uupkhfgf.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qhbsropr.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hqvdooqe.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2mtwacrrh.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2kcnnfvzd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2cbyqdypk.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2wcybmamd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ftfvnbli.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2aamngwmo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ybnyzhui.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gbrlquxm.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2morpewpc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2zpwnqffg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2yvnemicn.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2etywvpix.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2tvrvlvxl.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bjjskzyu.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2aovkiiid.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2jbejrmpy.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vkptaxsk.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zsdolknv.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2qfcnojpd.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rujticng.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lgjsaxwl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ryvsuisi.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vwvklzjd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2sculfdoy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wohcoqfj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nrkkzjsp.html


<!-- 参考信息 -->