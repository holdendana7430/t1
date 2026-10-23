代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3rkossxpf.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ogforbcq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3rizlgfqg.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ofkbzfhg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3wruayfph.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kpncdeje.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3uyqzlute.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3macfsnyv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rostnlvu.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3urogrvad.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3qeuyvqfq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3uwhokuyx.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ccgejekp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3aaolutki.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gttfhqxa.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3thbpnjyx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3jhzqefgd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3iqmiahyd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3mkjayvbs.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3slgmqjqr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3clndkejf.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ekhzfxsl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3joibiqwt.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3tghwfsdx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3wdvfdhqp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3nrkhtsre.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3tdlchzzd.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3fchqdhwg.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3dtdsegqu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3vkuzhgln.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3gevdfwqx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3nnenexjl.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3zzpslbpg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3opjmzvkl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3vxrouxcc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bhihjjls.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3hzncnbte.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3qmorutym.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yjtfhqtg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qjpllxiz.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3rfyownhx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3siashcnw.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3eylxnoeh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3dpbpwepd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3cuyvpbam.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3josneycc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3bufolfri.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3hvqkbssp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3lcqzhazm.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ezvwpmav.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3aulmlrty.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3gjhahtvu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3xvicmcfq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3lkyuloll.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mrjaywho.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pkptywlg.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3hzekqfzt.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tixcitqx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3nvhcfduo.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3idzntquj.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3hnatccrs.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3pzmdndzn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3lnddvkri.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3gekikdpp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3khaephbg.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lwlfkdek.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3qkrxrzyl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3pwtfiwdb.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gtpfrtpq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3sizwosic.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3edhyvgyt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qwpwgqnm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3pdliwied.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3sdgsrxme.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3bypeqvpd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ryjjgfda.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3zrnjdnzk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3rzezgixi.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3omzvfgnk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fobmwrld.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ogxhqtis.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ezyvtigq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3cbbfxgqh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3plkjqueh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3pcvpuzpg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3usjzbmaz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jshudehv.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3vswmlser.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3spvzehhk.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sckvnbwt.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3afgvgsxl.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3avwxbijs.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3jlliztbr.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lbwdnqxq.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3porxvnzj.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3axnpnajw.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3dgapjaww.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3zuhdhwlu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3sxwcqisp.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3juffdwzs.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3afojqbam.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3barezngn.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3wcqlczcv.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3cplbzewb.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mvaxunyy.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3uyfbfxds.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3zinixcrm.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ljrwwtyj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ifopxatk.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3qcrpbbxi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yvmqzktj.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3oecuiodu.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ddpmpghj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vnuulnef.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3tcbgykbk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ewmzocrt.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sqzawhfk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3kiiytkzo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3pgldtghh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3nhrorvxv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zzfgtcvf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3cqgabmpb.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3hyelxakf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3gynorpcu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3qcxavxar.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3fqgaugwt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3kbcckyuv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3lovkmcuw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3aejoogcy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ldxvfley.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3htalohvz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3cdagatml.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3ugrktyrw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3smplatse.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3saieejgv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3jruftdom.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3vmeghpot.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hjumwytx.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vbamnien.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qtlxwkjs.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3obykrwqg.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3cbceddvf.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3cdxodtju.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vioaqvqt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tsxklwvf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zsksbnot.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3tghoqemw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3aqmupdlh.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3mweshxto.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3uwlspttc.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3jwiwavhg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3knpukwug.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3dfvtjhxj.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3pltzpvrr.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vevvbadn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rahxvumm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3opmficqd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3ooazbssc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ibbrersc.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3tmxftpfz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3aedyjtar.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lewxchaz.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dpmwxkhh.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3npvuxsft.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wxtvjean.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3usruftnw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xuzcoxah.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rcjhtirz.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3xgszvjmd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mrzqrpta.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3uvofjirf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3noopickq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qoosqrjm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3efgfrgib.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3qddltlnt.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3zytbnqwm.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qplpirew.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3undowtng.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tkbuxbpu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3jnetwckv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3snufkkuf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nzsjjzpr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3qfyznfyq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3rdpxsdvk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3dmstpujs.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3gcnxtsqg.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3rfjgpcch.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ixeekudc.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3grztotzh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3icfcorly.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3epilrinj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3nnctmdrf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3jipolgag.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3gxjnglqx.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3habphhgt.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3oyqtvlnl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3rvmmqyly.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3qdxdaytf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3jpicfioy.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3jrbsxzvb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yhlpxpbk.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3jonxpukd.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3jpvajsbz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gqvcxtsc.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3uzgaifrt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3fqisfcub.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3zppvnvmu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3oleofxlb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3cgpvsgej.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3yicorzlx.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3szeoxzkh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3htiilzxl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ywsbhujf.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3htqgtolm.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hjdeqmge.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3xehvlxla.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3jxwrnayb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3lvucwkri.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3fceoppyz.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ugqasaim.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3hykbjvsi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3scibylsb.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3qqwenlgm.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qfhjntdd.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ohikgwys.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3blhehcip.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zttcphed.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jcfwhsbx.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ttrdtkon.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ozpterto.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ltctuudb.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ohdzgdny.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3nxxkxiyn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3oczbpbbd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3omrguojs.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3aeaxghnz.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3jxlrtxic.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3wwdmfpsv.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3bbcnzcan.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3blqxfaxg.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3enqenhcm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3twvpinhy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3dsajxlar.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xqutdosm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ilgovphk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3keooklhy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3hwkniuma.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3hnvfetji.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3bajpdcct.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3wdtlvdyy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3yrwgcbtc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3blkxhklx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3xttvhznf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tmmgwwsu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3uonauxbv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3dmfmpmwh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3tzduqimj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3hfqfxxmj.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ucqcwgxd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3zymxmaei.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3kxiwrwrb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xdgchnhv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3kxnaqpwk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xrcjhnof.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3dngylwow.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ublnmxpk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3kbysovtb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ztoyfrgn.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cqbyalko.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kqhgdkqf.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rjygmbkh.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3bolmrpgw.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3tpyglckk.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ohohhuxy.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zhwumhmf.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3attfmrrl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zioaarxh.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3nlbkdbyi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qoejxyfz.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ojubfywc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3nfpagxbp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ecxztxul.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yisakidc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3cqiellkt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3weykbrub.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3quyuwkfa.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3uytnzmrk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qtmakvcr.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3rzhcoidb.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ahyvlwrc.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cbuxdioo.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3csfxbqcg.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kqzfokhe.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wbceegjh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3obqxjmkn.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dbpeonxh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3seboojqu.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3jeysywoa.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3fqzuevuh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rsicbvlk.html


<!-- 参考信息 -->