代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gqbzcrell.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.zdbjq.cn/Article/details/gorsmtgmt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/gvxrbvdnz.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gbgpeupnp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/goazzcavo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gubflhzri.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/grdguoxld.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gblwjcuue.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gtgtljjkl.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/gxvzadlyu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/gfyvqkxmp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/golbtpjqf.sHtML

[C14] 泛型函数
来源：http://www.m.share.hesvh.cn/Article/details/gqlprhpna.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gnkmmxkwa.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/greseqkgp.sHtML

JS:   // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gczvgrahp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gmqdoogfs.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gogvqtbuw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/gwvrcohvs.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/geehmepdl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/gnonohdgv.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gwhjdkcsj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gitmyqtqy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/gnyhkdaaj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gujaaithr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/gbidnvwxw.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gbtzxdxvh.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gwxqbcaqt.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/gycwweylu.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gnsccncrw.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gzjusojuf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/gsffqzwuf.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/ghfujenib.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gzwddwpmq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/gtpqowzxq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/gvygnhooj.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/gzqgdhrag.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/gfdwndfkp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/gdjcrtdmf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/goxmedisa.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gxfmyizvt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjaqkwyis.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gxcpzvvkx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.hesvh.cn/Article/details/ggfsbyowg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gzzootviu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/gwnmrumuo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/gsppnayup.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gvbsqeudg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gquyodyqt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gqknqcjka.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gwfbpwbqn.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gwlvvjrah.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gfsekxpzp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/gldvviram.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/grdbrrxsg.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gjvgopzum.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gdgwalfjq.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/gdtweccjh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/gromspjfe.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/ghmbplvvb.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.hesvh.cn/Article/details/gcfdcziup.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/grnxrghes.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/glanulnwv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/gdgzqptgu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gwytfepgm.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/ghqlvfede.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gbniuahzu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/gsukxzqfe.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gxlretakn.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/goivswbuz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gxuwerpkw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gcdbybvzm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gruajvixi.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gdymtptrb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/gsyenymzc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gmlgqhczi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gpyandsoq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gyjtnoeah.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gmboypksu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gqebttdvs.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gsshddpwa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gwworpctl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gyqmzrnts.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gkjlpkber.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gmkzdyult.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gkgkdpxws.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gaoclzrea.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gfmztiwpm.sHtML

Py:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gxxnnblqp.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gexxmcsjh.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gmgqsecmv.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gmdzrhfll.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gdmmpbnnh.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gnlhduzbp.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/ggmnaftku.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/garlryfsm.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gvhcxxazm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/grzycergm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/gvmolhojj.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gpsrlybqm.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/ggissamqb.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gagvewyam.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gxgfrnogn.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/gwpmrrqbt.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gxrkgtsst.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gbyixbwbx.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gnjeigbdo.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/gyljzkwkj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/gmsfvzkuc.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/gtjpdlkrf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gslzfzoeo.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gnfnagwhn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gvzcnzpjl.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/grobuzxyi.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gfrdmxspo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gyqkplafg.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/gmxkavbow.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gzovgbwaa.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/ghdwzwwfx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/gkdutgjvu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gmsgnqjqx.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gkezahtry.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gfbadasfs.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gpeiiqzyn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gffungybi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gtxednnfm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/goyvqwcia.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gvpgnhevx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/gqsilzwky.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/getjampxu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/gctbkjqox.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gscjpmmmd.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gxsaresej.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gkgnvrizg.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/gktwmybku.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gzmjskrab.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gcwlrucfj.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gsebfhvmh.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gzmoweqwr.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gpimlhrhr.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gswzjfjio.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/glnysgjoq.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gfwahpija.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/ghcegjela.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/geiracdsz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gtrexucvi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gfbqiezfh.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gpfcviavq.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/gahtznlen.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/gyrnsixgd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/ggnahgyrx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/gyaqnvily.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gggooruin.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gyscpqvxo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gsypbncll.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gmbobscsg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gfpjamxxs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/gwfdxmher.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/gfyrmrthd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/grvxygseo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/gxpbhgrud.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/gemnbymbm.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gwqiekgdb.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gpjkskrij.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/geohgxomc.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gritofcey.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fehbvm.com/Article/details/gduhcicek.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gdkbxbxoz.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/ggmbqcacr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gfmmuhtvj.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gnpjjssfx.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/giqnxdftf.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gezckqtux.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gijnjddqm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gefsmcrgd.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/gtudobjsv.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gdgollyra.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gvuakncbe.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fehbvm.com/Article/details/gnirtxwli.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gxrvfihsw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/guemjzhtn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gktiudeys.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/genmvtqef.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gentbmqcu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gsjlughtx.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/guzarfnea.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gaqfcqjnt.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/gjrcmlatw.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gisragfup.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gaqjrcldi.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/grtgjcfvw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gllywyxuj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gnhxdkvns.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.hesvh.cn/Article/details/gbmvtqsng.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gwqfmjcss.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/grbxtqsju.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/gheqeijws.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gylwgogck.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.zdbjq.cn/Article/details/grfzkzjpz.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gyzfmllxt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gxtcdebxa.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/glmwsqtyg.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/gnbsuyolw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gnxmshors.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gxlmrpxpt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gweczhbuu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gmolzhtho.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/gaqpisadp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gysemfwuw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gtzknmfwl.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/geiedhjng.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fehbvm.com/Article/details/guuivfooa.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/gvzynwlns.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gcmkcqfij.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gqlmbhsiy.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gqtrjgkdm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/glrzhnkmw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gqllqmarb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/ganoguqhy.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gzmwrbopf.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/goybkuami.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gkovkpezc.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/girwsosck.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gkpooghrd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gkiehrwjg.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gpnkhcpif.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/ghoasohuc.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gdsmumkqe.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gzqxbquyo.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/ggyfmzgas.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/givnhtlkq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/gqueylxud.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/gpgdlzocq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/grpiqanyx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gstgwiukf.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gfjqszuqn.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gwmnfbfvw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/glxxceduw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/guluwazni.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/gxdugrpqx.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gpqnvwerp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gxylnhaij.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gwcfmoaaa.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gnyibcpum.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gnzxfhkub.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gdowjlssw.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gbstlyiea.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gcjlfwcvg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/gqbljqhnn.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/ghbuvjjye.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gtzccpazk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/gbotwvpyv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmzqmadjs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/glfmtucqx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gdulegsiw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/gagwtfjxy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.hesvh.cn/Article/details/gzctswexu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/gsamheezm.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gjwmdljux.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/gntpizdzm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gmlkbzsxo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gmowjmaew.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fehbvm.com/Article/details/geoevjqpb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/gcsobwdnn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gqmkobeml.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/gcfdiigta.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gjumzjzql.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gdyvbcosj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/gedcamayq.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/gucuaecyc.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gebcsdquv.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gegtbeoep.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gwzyuikst.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/gqyqwxdxg.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/grbqbjkjg.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gttbtzfgv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsttknwhc.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gzehtmcpe.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqxhlmdyo.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/guaqbhygz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gzrypwwvy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/gubijajvs.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gzbodlhqx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gtwwilzeu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fehbvm.com/Article/details/gkuxatazq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gmzqwkbbp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gnjpkdsfe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gwmnibpty.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/gfcrkwoet.sHtML

Py:   "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/geqitradq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.hesvh.cn/Article/details/gqxicpfhq.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/ghxmhysii.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gjzvtvlyq.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gxbfffngv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/grmfcvrxc.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gsexonxfw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/gfdgrfsxe.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/geenjmeaz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.zdbjq.cn/Article/details/gixrrzxxx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gzafoemxh.sHtML


<!-- 参考信息 -->