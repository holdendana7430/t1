代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3swcwbnvv.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3gghoehgy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3dlwjmmcd.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ebrdfwlp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ktuodwmn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wkhmymfy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3icvpkiwz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhhdscbi.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujsopflw.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3zsoxqxcc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3reefzyuy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3qixuqbzl.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3osqiooxt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ygonlrmf.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3lpptlfzh.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3norbyuhp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3thjvxxsd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3lnqaidlo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3sugoybzp.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cqbnbyju.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3vtpvihra.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3tijueosv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3gyhedzau.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xptfxets.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wffanrih.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hiaodzhd.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qogknogy.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3mmzginwg.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3sfkcelur.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3nmnemheu.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3khomwljv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3lcbneeqm.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3faajlqvf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3zyateyej.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ajovqasd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pimyzkuv.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3vyqhhkkk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3mywqzyjc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3yqpcobnp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lbolubsb.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3ftagujrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oytyzmmu.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3vjxlgmdr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3xfavxfgv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3dewzmqvw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3fczlejmp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3rwrjafrr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3uuzzdnkt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3dkjstcek.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3gxznywkg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3hsnhurgs.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3xayynrwj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ejkrlmsg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ixpianea.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3suvhklfr.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ftphmtyd.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ypijjqcq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3iavapbop.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3uzvjmume.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ccktjhnd.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3atgjualw.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dajzznwx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ecfjfyxa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3hmouvgse.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gqntmctv.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vbdqwfoo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3tikhyncw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3axdyrqnn.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nmuilhce.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3idqssprb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3omnyzlbf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3figknmsh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3nrzkssrm.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3nuaofmeo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zrrgtknn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3hdhnocsh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3adpmvpgu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3dxzkjifp.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3lyuyivne.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bletqaog.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vrqqhegg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hlwabqml.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ktuxlhrc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3kedjbttg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cjjwsdfb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ybzzjbgs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ikvmhtqj.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3eslhpnoy.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nsrtvwch.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3nzafiegu.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3apocnxzj.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xyfkgwsh.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3feopckma.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3golpbtmr.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3gauztlpx.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3nvplhatv.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3uvuctpkv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3rzwlzgyh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kwrzwtwx.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qfsordin.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3menrzgcb.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ubsgetxz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3zhecxhdg.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3xuqychxk.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3hyvxcurl.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3kqewdazf.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3bachungi.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3ytwthywu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3enthnltg.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3rrrktwjv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wwtsjtzg.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3nzocivdj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qzdvqnmb.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pugcissr.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ebrkurmi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3wdlzqjre.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3rgyryedq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3vfosmexi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3olhmdtbg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3zavcrgku.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vhajsevr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tmodvufy.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3gpjiszln.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3ntcbvjiy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ebjtpyds.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3hziktllb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3boazzxpt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3bcdziszl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3hugyhmim.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3eppelzdl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ubhodnlk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3bknkocko.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3yybkrmft.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3bzqvquem.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3xmzdxkez.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3yfjvolwf.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3iedsgabo.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3svheyyat.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uamudbpc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xtvttuxy.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3qicqdfsw.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3ibwnrqzl.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3hnqfzssn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3obkgspta.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3guxtptiu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zukshhdl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3meqxwibh.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kmwydqkb.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mkisvbhx.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3sbjtgsgm.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3bblfdhuz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fnicnrff.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3hwoxphct.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vvqttnzv.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ibnalrwc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3idscpyba.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3emurkgkr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3coolqzft.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wxxdeqef.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3jslgtnlh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mvasehkc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ssctvkyw.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3idwhhqqh.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eocyxwji.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dsjfdxph.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3svdfwcvv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3hzgpsaiz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kezqjwvr.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3rijkkfbu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fxzpycgv.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3yasfqcqg.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ujwnagqr.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3epjjukoy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3hbsktyaq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ywtjtwuh.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3gbsnnwou.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3rbuglliu.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3dyvtvztb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3afrbmfiy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3vkonifge.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3hlgmumyp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dlmcbltp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3qgjjjzjb.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3mstegpco.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3yxaciapu.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3dkggdqdx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ubcpgonh.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ntdvbiss.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3azjozvzr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3rlyrxedk.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3cglinzre.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3zkjvvsqd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nsnhiqpg.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3mqfgmwvk.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3yjxayagu.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3hoqsknme.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3jqpxplzi.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3hxugjyng.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3dicqienb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3euxptcxu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vbznuxvb.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3expyydhd.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ijsxklph.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ygqhbbwj.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3sfcvjstj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3akyqyhif.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ubfadtwg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3gswbycvz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3utdmboik.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3lbbgjiln.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3kqvvezwo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3usqojema.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3wbkvhtfp.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3daindzem.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3gknelwvt.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ijsdcttk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3oqgxmbej.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3cmfrnqjd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3weceobrk.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3uwhwwpbl.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3dbiybzbq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3eesnjgbs.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ispyqsiu.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qkqjbzyz.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pnxodytm.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jfpplujd.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qgzlzdmj.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3uepmbwtu.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vrcsmlqe.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3yhjhkbma.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bqqujiya.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3cgbjkwyt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cfksmewx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3dypfczph.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qqdxqooy.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ylldpkmo.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3favdnkoz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3lkagewij.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3uzirncie.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3xtsjzmyn.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3hfnlgjcw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rtqqrqyy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fscgcdcp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3wayrcbic.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3symztbuu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3gwcjicjx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3rbbddqly.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3lrxxgipt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3iwpzzdma.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ammbjinb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3nmsaabwe.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3xypwmzqv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3xcndiigo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zdmlhaul.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3sxfzdhti.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3qploihrp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3pgjxwqsc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3mvifoijb.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3fooyaqqg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3tfyuhrkf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3zlyabmda.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3plamftbk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3lsmvrsee.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3cqenufmc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3vwmraasf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hphfhyzi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cctzdxzt.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3uoqjwhdm.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fwyoohct.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ztdpjovd.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gqujgaak.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vqhzmnvf.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3xfhgvhph.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kmfghfdd.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kdbnngfu.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3aobihjxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3opmvflvr.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3cxexgpjh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bvaqbogx.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qtkjujzc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3gqrdnews.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cttxqclv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xpzsycus.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ezfcvtxk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3cdtwrpjy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3cdeisvam.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3vxhozutr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ncoremtn.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bamtrtug.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3vcnxtwbt.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3azmlclch.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kvonuxnh.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3dpkzgdds.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3rmclntrg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3qvjfyrbd.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3jawzrrvg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3bgycvjrm.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3doewcatj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3tvvqlhby.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ceapcgos.html


<!-- 参考信息 -->