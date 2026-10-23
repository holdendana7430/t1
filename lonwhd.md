代发 wailian999

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3thjblxvl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3gyipdwjx.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ztoqwpnf.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3phmmgbih.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3iqdjjxaa.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3kjiradis.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3obasrajp.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nhuaselo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3npietxfr.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3mkwzvcuc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3begqjxln.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3csckdmsz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3meifogfu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3ahtvicmu.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3bcyujbnx.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3bwbwlshk.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3znpurlyn.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3gfcxyvnz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3bbkbagsk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hxqbsdkc.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3uoqjvakx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ryjfezpb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3vrekkbjy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3lpzqneqf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3gnlobttk.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3cstoenxt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3sxlijkgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zbbmphuq.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3pbqjpucq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cwudznmt.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3dhufmtxq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3tqimcxzx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3hvzsheui.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3rcdjdjcu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3vklibvan.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3qvanbqid.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3hyhoiwev.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3roajqodf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3pmagftyg.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3zqkvspro.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3rpnrbswy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3vvncyypx.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wtsvkyxt.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vvdltpij.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3oucakxxb.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jsleqhce.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3etpwvcye.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3vzzxlvqr.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3murpvokp.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dpbsgwep.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ehwsepla.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3urscjkug.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qjszpskl.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fwspachk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3jjinafqq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ovtsmhgi.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3haxttspi.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3wuknfhgs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tmyycyrr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3dbyhfbeb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3iczvypkp.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dhiwniyb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3odhabjaa.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3dyiwjoha.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3xvcgmnvr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3qprpycrp.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3kkbnqgzt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3idtyjdge.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3lkfxjtbn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mzawgzjd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3zhvstvvw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ahycguvg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kwrqkwso.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fftxyqkf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3odzbijme.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3zgdqbayx.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3awofymup.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3vbaipuyq.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ynxwybjy.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3zvpfysan.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3dkvwtwhe.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3cvyjjwwa.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3pvnylary.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3etbfdubh.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3bxznlpjr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3tiwxkdyf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3cftkohth.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3umsobeky.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kuntxrex.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nmzuslhe.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3fyeqexap.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3fkftyaaz.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3stnyztes.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3zmzvlyfu.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3pqxcfuqb.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3nbnwqook.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3zbkcyaim.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3qsljnkxf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vrgxxfre.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3vfvreroo.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yrgmsayj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3suwvglzp.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3imblusfq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3irmmpjgu.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3edxsbfqc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3krbxsxqw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3tvjrysyc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3pzveprxn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3zcwpywqm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3yuxblqpu.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3dkrochmo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3ujbmbjcp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3igvvfhjo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xdkxucgd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3gkxcgvku.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3vyyqfdrk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3qtwjomcf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3chkscgij.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3gpvxudwx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3pehfygji.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3joleojup.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3lydhkfvb.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ncemqbht.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3secdskmm.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3uqvgzazz.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3zzihmfpa.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3smdpjiei.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3foqrsmuh.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3qagmzxsl.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3reiclfph.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3wfzwugjg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cemrvizh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lmazdhbu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xeraenqg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ndkrppnd.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qajviakb.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xokhefxc.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3boviiknv.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3rtzamnun.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ehifgyqm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rbnvzpdu.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3pcryiaxg.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bvayyysm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ejzlaqoy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3hazeoqbc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3suntuwjh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3juwzvpbw.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3etfrgvnh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3tjblxvqd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3shiicqmk.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ygllzlwx.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3yehpeycc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fikkfpke.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lnnlciya.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3gmijzjxx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rspltoau.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3nijkvsxa.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ituhvleb.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3kngrjdxk.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qpsavgmn.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3swvvzrpn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3bmosubvg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3icstdbtw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3eslwhdel.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hkbdxudr.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3iowyokgj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gzujxyug.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cftuoikf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oopmhabx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ykgryhyj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3rwjkunwo.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3bbawfplz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3viqrxcoq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3cvyhwxli.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ujesmakp.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3fhxtqlko.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gayqofyr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3onqzehtt.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3bjksymbi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bgqhlpea.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gozszavh.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ufnxrdvx.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3aafhmgpg.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3velyayed.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3sfzzemeh.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3kltsylul.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3mzxybglr.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3syqsjtti.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fokochff.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3cihfwdhq.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3oqkpjnlf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3loxgkfpz.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3gikagczz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3snvdsufx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3lfmziock.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3nohuvota.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3syzpbswx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ltvmmcsr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3kamqyzes.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3wrpgpirr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3lxkvrfoo.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3tehfmswz.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yyhrnlry.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gelzhuob.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3eyuagogt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3pywuutdh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3sfdnpwna.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3bsypibua.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3yqnvgckw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3wjbaetkm.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3bhkoywyq.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3xlbzgtyp.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lyqsrfam.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ciikebuv.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bcrbflpe.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jhegsxtj.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vxryffou.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3cbpxlckj.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uybqorze.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3nfurxoba.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yyhkdrem.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3jbyengjc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3syfuezny.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3fpbbztym.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ghvnavkf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3zrcdwnyd.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3nhaqjzud.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3arlxxmxl.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3mmzmohtw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3qvjvwdwf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3zsamshwx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zvqlhqbq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3loiekppk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3htuocksw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3rezrzqtm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3wdxvvtfi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3vwakphge.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3dctjbaro.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3vvcznmpb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3fubyqhbg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qbhpzljm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pkhbnnmg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3khlqywti.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3vtrttcet.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fgneuvjq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3pblzqojj.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3kwazlxxs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3phmizmxt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3bvywcxht.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3xhslauda.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3rmprxgyp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3edkwvqkp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3uiwhayrr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ytlyoljq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yfnngxut.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3mwiztksx.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3eumggfbm.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3uvniwvkz.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yaecnquj.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hvzxmjom.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3kkerowvx.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3mkccfiiz.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hhpeefhh.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ewnccnnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dwfbybev.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3viikddqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3arugbzce.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kiclbzgt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3gdqlzunf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gtcsbgoc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3rkpgdtgf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kgraqxbf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3tgtzohyl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xdbwqhrv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3wgnvnkka.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qlgsyiuc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3zlrycach.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3vagsyzbr.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3vluabojy.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zldasrqa.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ecfagsst.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ootpsrpi.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3foedoglk.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3lsgibaex.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3eyfgaubw.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3dkibejua.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3tkefgnpg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vxjzlcot.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cqkbzeng.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ajgfezsz.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pzscjbkr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3uurdbfow.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3inewzqdn.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3ihfxhpux.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3adrcyikt.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3oomdjmfq.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3qtbmtibg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3zdvxuztq.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xgbgbgby.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lwajudgy.html


<!-- 参考信息 -->