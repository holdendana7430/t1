代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2pnmnpyhb.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2rhjptqes.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2mdeawfyr.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2yzxtyrjw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2sawoczvr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2djcjwcwp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ncbsludy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2udmtfghy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yoqscwsy.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2fgdjweal.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2zcyffmxf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2ryjpxwyh.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2gujvhcgl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2lmjqywms.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xppxsmtl.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2aryqxleu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2giffgacf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2bllkangi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ofuujyez.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2eqmxtvoo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2wbzhwkdx.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ycvsyqkt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2njfgznma.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2eeofiuqs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jtsywqjv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dinajrbb.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2catmtoky.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2tfjqtxrz.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2cvwhietq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2zsmrxpnp.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2vfiezucs.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2tyealcyg.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2pwmfmpzr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2zdeqwbus.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2hjkbshyq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2pxqvtvop.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2mbqwzdun.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2druoqcdw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2pumslxqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2togzuwmv.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2gnqhxdcp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oyoxsvzm.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qdgklppm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2gasfkudh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2twzdhqhn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2gvptkrdp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2xmmppfdf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ceclncuj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2zskosgmg.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2trjxehrn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2thzksjln.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2yukkxiex.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2sbquwfkd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2rchkbibp.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2apsjqois.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uukyhqzm.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2hxfgisuu.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2fpditulo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2jdwtondw.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pvwooqni.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2pwhowjcp.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ccvryose.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2edfbzvvq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2uoykjqfo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2uziujmcw.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rjlwztii.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2rjncpthe.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2wndwunjj.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eryhazsu.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2lmhafbvx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mcozoead.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2gimhbanj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2pkjahfox.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2wuivlbtl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2xdcyutnr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2mpjxgmmn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jghdkuwp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2tvtximdl.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2kqisvsew.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qqomrwxr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2sdwpixmn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rkhhlefs.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2mybedciw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2fxnpisat.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fopjqobi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2khxigmkr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wayvyzoe.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2scdxnjeb.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ndusgfoe.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iomkzacy.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2kqtlgldr.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2tqncqmtx.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2fdkppnxn.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2klruemqh.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jnfovntf.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2nlosimgd.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2rqhakirp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2amwbohih.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xtixzcxy.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2flpwlfnn.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zkpevcqj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2bnviwpev.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2wadykyhp.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2fynuvxww.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2wfvpxxzx.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2urbgmzyh.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2evscupvl.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2kwboneok.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2brcqokxh.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2uoqcqtds.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bepcvoow.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2jcgmiavr.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2habyakzd.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qzbraonl.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2zydvowys.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2gqrasago.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2fpamuxbt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2nzwsfmbk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2emxquklt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ahpdlrdo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2irbcprrg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2mbrsqnll.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2gruqnact.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2uhejshmq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2tjeditlr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rkcrxjka.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2mmckkwxe.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2boezdzlv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2rfgmgoud.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2rpfuyspe.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2xdyteycu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2xrneyizw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2zijdnxms.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2pxgrijyx.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2lzvtbbix.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2qfrjsrcg.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2sdgkdwoi.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2vjfbfhln.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vuctbqen.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2pcbklncw.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2vnacrehz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2giewcnkj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qzviiikm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2jlkcakaj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ryoogrif.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2zbnoifra.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2gillpavt.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jikjswdj.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ifslrkbv.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2cfwlkvys.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2fflyweio.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2msxjqdge.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nuhpvtds.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qnynipxp.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cejjqwdw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jeioselr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2oxarurrf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2thbfgbil.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zbhnvmfu.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2gejyvovw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2duepucmo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tomfgcis.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cnqxfcrb.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kbfbdcgl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2pknvydpu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ucswwpub.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pgqhsgap.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2imsrdbqe.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2snnskpkc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2xxyfhhkl.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2njittirc.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ybjeszft.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2upzxjimw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2owwcoltd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2pquwbdpg.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ggnmxthp.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tpexombk.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2kheikaac.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2yjgtswvz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mtlgotvl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2pmstswaz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hiicrems.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2gfddibxf.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2agxbbbuy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2rzhmwnec.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2rveqipbt.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2uryvxnee.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2opgugida.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2vojanpru.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tpkwnxla.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kdxoesyj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yaarduid.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2qhvxaaya.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2chupzmil.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2hubuojfi.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2vjuxszcw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2lqhjuszc.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2vciwkiwp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2xrwymfcw.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2tarjueuq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qzgtmqqa.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2aukzdpio.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2exffufgc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pggongwx.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2dutpycvy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2gyieqvgl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2odhpqufm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2otcqzpbn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2chfpagay.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2uiraebjm.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2crreblpd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2vmsiqaoh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2oyuxnlmv.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2obssunrx.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wxvoxhlw.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gtftserm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wcdtfcxl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ysoqdpyf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2lflyxekf.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2zfmttbot.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2leboxray.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2janwjbah.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2fktcrctw.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2pmuammxj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ktjznftr.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rbpxeydn.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hhaeaudy.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lsdcezhk.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ndmrlgmc.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2exzsiamd.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xqtcsqdy.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2cwxrfybz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2tpyixpne.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2aymhxbdf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2mnhiikga.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2yrmetyjz.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2xmmvbkbg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2putchvsi.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2kyctztwd.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2rfaitobg.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2zdcibrpu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2rodbedbd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2bdxlknjv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2xwcqtabc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jzzlfumq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2doxyvwhj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2oiutwnnx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2jtnnsjwx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ucnhzizu.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2edeewnsk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2gkqcuegb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bolxgxwu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2muspizji.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hadcdzzo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2azjzjule.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2yowxjyzu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tmkgrjow.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2rylinsgl.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2hvckbbfk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2sjpodlby.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2fpnhtkms.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2yzcarvcm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2wtacvwqp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2tmttujkz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2hfwrtwkf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2gcbkvfxw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2vendiehu.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2beiiwnms.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lsjlcpgh.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dczwebzo.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2guxybsdc.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xeqmjhtl.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2cvagudhq.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2lwkmezem.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hkkhbfwv.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2dbdbgctg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yffblasv.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2grapyrtn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pqrflsoz.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tceazmzv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2kbymzkaz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ilvbskos.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2zkshuqyw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hxcdezrx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2uyduidsn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cohocsfe.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2xnjaadpo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gamhshbt.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2jprlqamx.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jcwgsqfw.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ijdvwbsv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2kyxfnioh.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2iyoghobz.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2etfrwpar.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2htpsvquy.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2grgrartu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ckzdwnyd.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2sjamaqix.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2mbcdcyld.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qclbkvno.html


<!-- 参考信息 -->