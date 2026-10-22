代发 wailian999

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xruoydqa.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2kteghvps.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2nvjsoxzb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ivsmuwmu.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2cignoqlk.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2iisnbtdm.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2xsqvsirn.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2idihlmec.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tkxkkokp.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2tdpownyh.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2zcbwbppa.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2vbqnfiuv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2volaaedo.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2mkvyurei.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2jombvspn.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vldwrerc.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2dngichcn.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2waloosha.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2kedcqrfe.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2bzlnrdjx.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2gvpbumcm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzbttaqj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2uxsigord.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2wkvsruxx.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cgntcxxu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmyzboto.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rgvlldmb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2wodvcgua.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2bsgkpbqv.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dcagfqff.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2fyszgdtq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qkuiqils.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2nlyrjitc.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2drgteynj.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2sukpiaym.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2bflosfgn.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2xipsicbe.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nodlyoxv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2lqtejcsw.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2zpwueamw.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2fggxegyh.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2rovoamfe.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2qpyucpkz.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2smzvedkg.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ftodzrtq.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2aiolyghd.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2smsnewjp.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2cmuttzhk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2euqvpnkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2plultoag.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uiekretn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rxgzxtjl.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2sfencffs.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2bdlfrujm.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2fhncutzl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ptkadftp.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2fenuklxy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2tttqyoyk.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2krappdud.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2benzzcmy.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2tuuxqrvp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2fipezegf.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2zsaccsyb.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2lxipdzgr.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2biqlxjkg.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2yspjfnfk.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2xmgfnpjj.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2phuohbqb.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2wtcqmgko.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ytpbvqpa.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2xfeyehwh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2nkwuxuqm.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bwtpwobh.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2hfwjkbbt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2aqngtpdx.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qvvjjqhq.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2vvwcorwl.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2khjiumxz.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2tkrlwkwr.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ixspwvzb.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2fkbvdube.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2jcjuehsm.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2qiqnvxao.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2idbeurbz.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2cuqdacmp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2dgbxdsjk.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2erclvpvg.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2eggfmshc.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2fektbtne.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2aobdlqwv.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2feabalmr.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2mixhmqrl.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2pcuuipmy.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2hrlzvtld.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2yprpttrx.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2zzicjnxp.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ujxbvgsm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2rrrrmevr.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2icxovdzb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ohyjnmxg.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2yhowdjni.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2wsgdyyed.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2oivlhcxf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2yzlqjfra.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2noefpwew.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2gxgypbxc.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2zeabqjfa.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2jijwyymi.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2mgkhzgpu.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2gynaqmqt.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2nwyejbkf.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2urexwhmc.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2bbzniiup.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2umftnxxl.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jdggckof.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2cgbdcgng.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2obnhrrep.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2aevegvum.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2tehfzaac.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2qicomonv.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2zknqftfu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2hzkdmtli.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2jylnpjhc.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2zpkwsgzl.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2ojixhuuc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2kdbsapff.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2gxfjkocd.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2mkfbnpqk.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2arxyqbni.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2odmbnlfy.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2fsewsnso.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2hfcrrgnc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2odwgbjan.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2bizmwjxq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2efaorsrs.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2ymxkzmzh.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ebenrtjz.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2ehnvwmjq.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2wxbceouy.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2qrachaps.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2eoqitjur.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2emvpsfoo.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2dnejwrgc.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2lvzevwny.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ikksjhqt.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2bfcqcyec.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2skmjjqgw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2bttxpycd.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2yudeabnz.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2dpdqesco.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2wpzlnhjc.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rowjhodt.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2srfpuipk.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2teoalwfu.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2peplqjom.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2cbzyfzjv.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2zscezxjp.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2hpbqzbzp.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2bcrctuei.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2mcmrhymx.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2qgeqxshv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2vbuzdytm.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2kimejfzr.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2stxjighp.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2feqgkfuk.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ivqbeqit.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2lbbtdgui.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tuitgqns.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2hwhsigtr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2phrlevwi.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2ldvjxfvc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fliqvswg.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2ebxpjszn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2tmhbqvjz.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2sghylccv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2mzpdrypn.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2tcothyyy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2bxznojtt.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lqewfjka.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2aohslljs.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2lsrnjuru.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2eulfmcjs.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2dqgpmdwh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2gmrnvnem.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2twmsxpkg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2hvtrerez.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2jnszceys.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2ghesrcyd.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2tutkzqrz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2cfcozcpp.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2pmmhixdg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2cavejesl.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2cccbpstg.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2xiulqrzy.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2xcnkqfzf.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2nkerfzdh.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2yhnptosu.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2aexmqixs.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2muwsutuc.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2plzqspop.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2kopjcdoj.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2mlzuxgtc.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2pgpobzff.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ysyaozsh.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2xgmhaqda.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2aipepnuf.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2zdtnfinz.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2vpmysdxw.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2jpfcpdwt.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2lvnruzsv.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2uihbfxmc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2itglchwv.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2thyzmnan.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2tgasesch.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2xxogzwqy.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2dxzcomgk.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2kbplwpwu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2gxvygqpm.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2iouaxolz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2fjjabsos.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2eklvjtgg.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2rwlwhdfc.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2snpiqncu.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2qfhymoom.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2oymhsihr.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2zdxydchp.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2erxqtqqo.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ttgkivba.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2mcksieun.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lnhqvucr.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2ydxwqimu.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fqasjiok.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2weoyvedj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ixyzmegd.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gvlwrmgu.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qhpfllpm.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2nfzzrcbp.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2qdkawrpx.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2toajwtef.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2nevytuuv.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2jvmgbsvs.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2cldqqfww.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2zrvkyptg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2oyrnhrgl.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ysaymzlq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2sdyyfcvb.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dxrlaovj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2hrpuluzs.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2jikugdsm.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ncizqmwn.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2xfjpbmpi.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2kbozzakw.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2qvnxkwfs.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2erdcvzti.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2uvsqivsi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2zvtirtio.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2vmopbbla.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2kwfpxufw.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2lknklhwx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2uclbylig.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2natxbdfn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kismtecg.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mpmzwwns.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2qlpvfkhw.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ljhnxkiy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2aqkkqsgi.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2umaciwje.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2nxjrhacc.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2ihddxruj.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2nwbxvfyw.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2olwxfnrr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2gtkcannz.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2avttvecm.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2bswhpmtm.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2remdndfw.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qchokbnn.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ikqiuhij.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vkhvregk.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2wcsyxjcs.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hehxwxzs.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2wxebgllj.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2upjxptpt.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2ukfzranm.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2dsecgjcs.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2txkmmkmx.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2omdsnssw.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2tcosyfxu.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2izwvjxzb.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2ditegzpe.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2ilqertgs.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2tbcpumvv.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ynsrtjhp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gyfivryh.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2ukjfldfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dnoypbcb.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2gkcpihyr.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2hvwszmty.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2paxmogtu.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2uswgyzky.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2mjvtkctk.html


<!-- 参考信息 -->