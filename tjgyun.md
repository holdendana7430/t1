代发 wailian999

[T45] Perl：数组遍历
来源：http://hz.feifeiyinyue.top/gtzrublxao.html

for my $x (@arr) { print $x; }
来源：http://hz.havefunace.top/gttjlmsgxi.html

[T46] Perl：哈希操作
来源：http://hz.tanke756.top/gthdqihndd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zhijiandao.cn/gtwsylvlxy.html

[T47] Perl：正则捕获
来源：http://hz.wangshuangyany.cn/gtyslpkofi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ywan-chungtsiang.top/gtfvfreubf.html

[T48] Perl：正则替换
来源：http://hz.cqqwz.cn/gtsyyrjugp.html

$s =~ s/old/new/g;
来源：http://hz.zdqjudy.top/gtfsupcpvx.html

[T49] Perl：函数
来源：http://hz.cashguo.top/gtsthlonds.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.xinyue.icu/gtcxhcbizw.html

[T50] Perl：逐行读文件
来源：http://hz.andypj.xyz/gtcuhbntec.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.0kj1m.cn/gtwygupfye.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zhiwuduotai.top/gtlwisnquw.html

[T51] Scala：Hello World
来源：http://hz.mhx1999.top/gtpbxrxyel.html

println("Hello")
来源：http://hz.kuanghao11.cn/gtzxqocgap.html

[T52] Scala：变量
来源：http://hz.svipenyu.cn/gtlsfmhbsg.html

val a = 1;  var b = 2
来源：http://hz.sweek.top/gtkistzond.html

[T53] Scala：字符串插值
来源：http://hz.shzxlz.cn/gtlgpzsmtx.html

s"值: $b"
来源：http://hz.chenlongwang.top/gtizxwdojy.html

[T54] Scala：集合映射
来源：http://hz.yuanzhike.top/gtcupnewpc.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.jqgufenzy.top/gtpxlpkoqx.html

[T55] Scala：集合过滤
来源：http://hz.zhongyouzk.top/gthlveuttg.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.birdmap.top/gtamwqwtvs.html

[T56] Scala：样例类
来源：http://hz.yangfankeji.com/gtfzqnwylo.html

case class User(name: String, age: Int)
来源：http://hz.c1oappe.top/gtqlcdqdba.html

[T57] Scala：模式匹配
来源：http://hz.9152youxi.cn/gtjeaefrpu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.snrcjt.cn/gtsajhgwsd.html

[T58] Scala：函数定义
来源：http://hz.ybcxt.top/gtftvhbzqy.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zhixingplan.top/gteybehirv.html

[T59] Scala：循环
来源：http://hz.meibo888.top/gttqffseip.html

for (i <- 1 to 10) println(i)
来源：http://hz.gogol.net.cn/gtoskvroxr.html

[T60] Scala：折叠
来源：http://hz.hnxiangtu.top/gtbtngnugl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zhengqikj.top/gttffearce.html

================================================================================
来源：http://hz.zhixingplan.top/gtlbhlgivl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jqgfzy.top/gttqcdhxyo.html

================================================================================
来源：http://hz.haohaochexian.top/gtdyvpbxjm.html

[U01] Py：创建虚拟环境
来源：http://hz.bjfxy.top/gtsmcunglw.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.cqqwz.cn/gtcsffgglw.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zhoulong.xyz/gtyeazspln.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.hongshengwenyu.top/gtmyldkxmo.html

[U03] Py：加载 .env 配置
来源：http://hz.yonumen.top/gtmfkwaplp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.pycfn.com/gtybmffyro.html

[U04] Py：变量调试打印
来源：http://hz.yuanzhike.top/gtcensfqws.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.meibo888.top/gtnrolkpvu.html

[U05] Py：列表去重且保序
来源：http://hz.shuidangran.top/gtwtgqwjzi.html

list(dict.fromkeys(arr))
来源：http://hz.mhx1999.top/gtaujwtvsw.html

[U06] Py：合并两个字典
来源：http://hz.52xcode.cn/gtmpegntef.html

{**a, **b}
来源：http://hz.quarkkingdee.top/gtawqbpxxz.html

[U07] Py：反转字典键值
来源：http://hz.wangshuangyany.cn/gtdwzwbmrw.html

{v: k for k, v in d.items()}
来源：http://hz.cdnleiting.top/gtnknpcrmp.html

[U08] Py：展平二维列表
来源：http://hz.zhijiandao.cn/gtiwndexvu.html

[y for x in nested for y in x]
来源：http://hz.zycfv.cn/gtzsmvcldl.html

[U09] Py：字典取最大值的键
来源：http://hz.shzxlz.cn/gtvatkjyeu.html

max(d, key=d.get)
来源：http://hz.sysykeji.top/gtqdydwkuc.html

[U10] Py：按值排序字典
来源：http://hz.redwolf501.top/gtpkyrmvfw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.sweek.top/gtvbzqcwek.html

[U11] Py：生成器表达式
来源：http://hz.sufxvd.cn/gtovjyljvd.html

(x * 2 for x in arr)
来源：http://hz.cdnleiting.top/gtijajyehm.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.hnxiangtu.top/gtaeojigit.html

Counter(arr).most_common(3)
来源：http://hz.sweek.top/gtgmfvwvqe.html

[U13] Py：固定长度队列
来源：http://hz.quarkkingdee.top/gtjaovietw.html

deque(maxlen=10)
来源：http://hz.sweek.top/gtuhavxnne.html

[U14] Py：分组收集到列表
来源：http://hz.yvedp.cn/gtvzaixany.html

defaultdict(list)
来源：http://hz.xylfe.cn/gtnhzoerqw.html

[U15] Py：高精度计时
来源：http://hz.yueranfly.top/gtppkpkyht.html

t = time.perf_counter()
来源：http://hz.yanxiufei.cn/gtaupdnlbt.html

[U16] Py：命令行参数解析
来源：http://hz.nanxinkj.top/gtqfkluizm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.52xcode.cn/gtafrimgcv.html

[U17] Py：初始化日志
来源：http://hz.jqgfzy.top/gtzjysspkf.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jqgufenzy.top/gtytnxpqrc.html

[U18] Py：预编译正则
来源：http://hz.guannengcc.top/gtkgpbbdej.html

pat = re.compile(r"\d+")
来源：http://hz.gogol.net.cn/gtifbpacpp.html

[U19] Py：正则替换带回调
来源：http://hz.daria6918.cn/gtxreiiqch.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.cqqwz.cn/gtvlbqjvdp.html

[U20] Py：缓存函数结果
来源：http://hz.shuidangran.top/gtogwbngnq.html

@functools.lru_cache(maxsize=None)
来源：http://hz.meibo888.top/gtfwdczbrv.html

[U21] Py：自定义上下文管理器
来源：http://hz.yj202588.top/gtzvkrgisf.html

@contextlib.contextmanager
来源：http://hz.hongshengwenyu.top/gtlyfmrjqh.html

[U22] Py：矩阵转置
来源：http://hz.yj20258888.top/gthzexaquv.html

list(zip(*m))
来源：http://hz.yuanzhike.top/gtudkiunqx.html

[U23] Py：分块读取大文件
来源：http://hz.yj20258888.top/gtwhfwnfjs.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jqgfzy.top/gtuajvhuoy.html

[U24] Py：路径操作
来源：http://hz.9152youxi.cn/gtxvjkkymv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.gzhubu.top/gtbultahmq.html

[U25] Py：CSV 按字典读
来源：http://hz.shzxlz.cn/gtxnetmlgn.html

csv.DictReader(f)
来源：http://hz.shuidangran.top/gtbjeuabge.html

[U26] Py：并发下载
来源：http://hz.haohaochexian.top/gtdpndzhds.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.tian-w.cn/gtgdyerzpl.html

[U27] Py：异步 HTTP
来源：http://hz.cheryme.top/gthoslaxpo.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.gzhubu.top/gtpklxshcz.html

[U28] Py：类型别名
来源：http://hz.zhaomingkeji.xyz/gtkdjeqduj.html

UserId = int
来源：http://hz.yuxming.cn/gtiucugkbu.html

[U29] Py：属性校验
来源：http://hz.jiagoushi.top/gtcqhpikse.html

@property 与 @x.setter 配合
来源：http://hz.zhixingplan.top/gtykfbgdko.html

[U30] Py：数据类
来源：http://hz.ybcxt.top/gtsnpeyfhw.html

@dataclass(slots=True)
来源：http://hz.c1oappe.top/gtqrljyfny.html

[U31] Py：单测
来源：http://hz.yuxming.cn/gtwrpohffh.html

python -m pytest -q
来源：http://hz.yanxiufei.cn/gtoeijqyrq.html

[U32] Py：代码格式化
来源：http://hz.jqgufenzy.top/gtvjxdzcun.html

ruff format . && ruff check --fix .
来源：http://hz.guowangkeji.top/gtpvspzlsz.html

[U33] Py：打包发布
来源：http://hz.birdmap.top/gtuwhbkesk.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jqgfzy.top/gtyjljslli.html

[U34] Py：判断编码
来源：http://hz.ywan-chungtsiang.top/gtqfkqtuij.html

chardet.detect(raw)
来源：http://hz.nanxuanxn.top/gtabjcngyj.html

[U35] Py：发送邮件
来源：http://hz.aizwys.cn/gtzpohkukk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.zhoulong.xyz/gtpmolrtom.html

[U36] Py：定时任务
来源：http://hz.yuanzhike.top/gtsrphekie.html

schedule.every(10).minutes.do(job)
来源：http://hz.shanyushiyangkeji.top/gtcbkobexp.html

[U37] Py：读写 Excel
来源：http://hz.gotoacloud.top/gtjhizeeqv.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.hammf.cn/gtbkterepo.html

[U38] Py：获取脚本所在目录
来源：http://hz.xinyue.icu/gtgzvbvokv.html

Path(__file__).resolve().parent
来源：http://hz.iojbl.cn/gtmhvmwuzz.html

[U39] Py：判断是否在交互环境
来源：http://hz.chenzaomai.com/gtylrzjqfk.html

sys.stdout.isatty()
来源：http://hz.cucudq.cn/gtsirgwgmt.html

[U40] Py：打印到标准错误
来源：http://hz.hnqzz.top/gtyxecpbvn.html

print("err", file=sys.stderr)
来源：http://hz.jiagoushi.top/gtygheuvvm.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.dashuyun.cn/gtbrgxfbjt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.shuidangran.top/gtpkasrkpw.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.wangdashe.top/gtvgprtyey.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.pycfn.com/gtckonrlhd.html

[U43] PHP：声明命名空间
来源：http://hz.ydjk.org.cn/gthaeajksm.html

namespace App\Http;
来源：http://hz.jqgfzy.top/gtbqxccdwf.html

[U44] PHP：开启严格类型
来源：http://hz.shanyushiyangtech.top/gtgqydkzmr.html

declare(strict_types=1);
来源：http://hz.xuanzx.com/gtgtwrdtbu.html

[U45] PHP：类型声明与返回类型
来源：http://hz.shanyushiyangkeji.top/gtxzddleqt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.guannengcc.top/gtjohlcxrs.html

[U46] PHP：可空类型
来源：http://hz.nanxinkj.top/gtexxzbkcm.html

?string $name = null
来源：http://hz.zhiwuduotai.top/gtvwvsicll.html

[U47] PHP：联合类型
来源：http://hz.zdqjudy.top/gtnggmgsqy.html

int|string $id
来源：http://hz.hywenlv.cn/gtbzxlwawm.html

[U48] PHP：纯枚举
来源：http://hz.kuanghao11.cn/gtrblwpked.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.shzxlz.cn/gtkevxjfzl.html

[U49] PHP：只读属性
来源：http://hz.aizwys.cn/gtoszwmfaf.html

public readonly string $name
来源：http://hz.yvedp.cn/gttqnfwavp.html

[U50] PHP：构造器属性提升
来源：http://hz.ivvv.top/gtfnbmydxb.html

public function __construct(private int $id) {}
来源：http://hz.ppjwa.cn/gteewgtcep.html

[U51] PHP：数组解构
来源：http://hz.yangfankeji.com/gtnhctqzjj.html

[$a, $b] = $arr;
来源：http://hz.daxiang520.top/gtfimglabo.html

[U52] PHP：箭头函数
来源：http://hz.gotoacloud.top/gtudicxxld.html

$double = fn($x) => $x * 2;
来源：http://hz.guowangkeji.top/gtpwwfsfxb.html

[U53] PHP：空合并运算符
来源：http://hz.ppjwa.cn/gtrphiyaez.html

$v = $a ?? $b ?? "default";
来源：http://hz.hysaishi.cn/gtfhzhpqyr.html

[U54] PHP：空安全调用
来源：http://hz.yvedp.cn/gtzerrwwxo.html

$obj?->method()
来源：http://hz.chenjidiqi.icu/gtxjfaxnou.html

[U55] PHP：match 表达式
来源：http://hz.xuanzx.com/gtbikjpvvr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.zhixingplan.top/gttjydxqld.html

[U56] PHP：命名参数
来源：http://hz.jiagoushi.top/gtcixpwkgd.html

f(a: 1, b: 2)
来源：http://hz.ybcxt.top/gtrrygkkna.html

[U57] PHP：字符串插值
来源：http://hz.cqqwz.cn/gtkonoeumf.html

"值: {$a}"
来源：http://hz.c1oappe.top/gtikihubwi.html

[U58] PHP：数组三件套
来源：http://hz.fengsongda.top/gtpyghuxmh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.xziqi.cn/gtzykbwdpj.html

[U59] PHP：自定义排序
来源：http://hz.hnxiangtu.top/gtdixokjom.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yuanzhike.top/gtkbtdwowx.html

[U60] PHP：JSON 编解码
来源：http://hz.yvedp.cn/gtwtfiwbki.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jyoumei.cn/gtosxewznc.html

[U61] PHP：正则
来源：http://hz.haohaochexian.top/gtuehkpyax.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.cqqwz.cn/gtvgaryatz.html

[U62] PHP：日期对象
来源：http://hz.havefunace.top/gtjpgpmgll.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.pengpengdd.cyou/gtylsipujd.html

[U63] PHP：文件读写
来源：http://hz.cashguo.top/gtckqpgxnz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yj202588.top/gtsyhsbmcz.html

[U64] PHP：目录遍历
来源：http://hz.zhongyouzk.top/gtrnyojzoo.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.daria6918.cn/gtofxkloro.html

[U65] PHP：会话
来源：http://hz.aizwys.cn/gteakwnneq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.xingfuxueyuan.xyz/gtopankpum.html

[U66] PHP：设置 Cookie
来源：http://hz.chenlongwang.top/gtcmunuhwl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yvedp.cn/gtterwjcoq.html

[U67] PHP：处理文件上传
来源：http://hz.yj20258.top/gtoouriqcy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.xuanzx.com/gtnqcnutvy.html

[U68] PHP：PDO 连接
来源：http://hz.aibaodan.cn/gthnkwxhti.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yangfankeji.com/gtsdjbubcl.html

[U69] PHP：PDO 预处理
来源：http://hz.zhijiandao.cn/gtrgueyktk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.havefunace.top/gtfgdzrazu.html

[U70] PHP：PDO 事务
来源：http://hz.xingfuxueyuan.xyz/gtimedrjpa.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.cashguo.top/gthqqsmkro.html

[U71] PHP：抛出异常
来源：http://hz.52xcode.cn/gtigampvvh.html

throw new RuntimeException("失败", 500);
来源：http://hz.xuanzx.com/gtrjfmzmlw.html

[U72] PHP：写错误日志
来源：http://hz.sufxvd.cn/gtgpykzxio.html

error_log("失败: " . $e->getMessage());
来源：http://hz.chenjidiqi.icu/gtqrfxnckl.html

[U73] PHP：读取 ini 配置
来源：http://hz.ywan-chungtsiang.top/gtpagpnsgu.html

parse_ini_file("config.ini", true)
来源：http://hz.tanke756.top/gtmcsqqvok.html

[U74] PHP：读取环境变量
来源：http://hz.mhx1999.top/gtrdkgjoqs.html

getenv("APP_ENV") ?: "production"
来源：http://hz.zhixingplan.top/gtezdgbsqu.html

[U75] PHP：依赖注入
来源：http://hz.yuxming.cn/gteirmazcy.html

composer require psr/container
来源：http://hz.yongpay.top/gttwtdpxsw.html

[U76] PHP：简单路由
来源：http://hz.bjfxy.top/gtfxavluya.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.hfpthk.cn/gtqzxeafjo.html

[U77] PHP：模板渲染
来源：http://hz.zhoulong.xyz/gtifmtajoe.html

composer require twig/twig
来源：http://hz.daxiang520.top/gttrxtexvq.html

[U78] PHP：单元测试
来源：http://hz.yueranfly.top/gtrrumvlfn.html

composer require --dev phpunit/phpunit
来源：http://hz.zhixingplan.top/gtvyyaharb.html

[U79] PHP：静态分析
来源：http://hz.zycfv.cn/gtygpbhgnf.html

composer require --dev phpstan/phpstan
来源：http://hz.jqgfzy.top/gtwoipngei.html

[U80] PHP：代码规范修复
来源：http://hz.hysaishi.cn/gtcdupryiv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.guannengcc.top/gttzmwdxnf.html

[U81] JS：初始化项目
来源：http://hz.316326.xyz/gtfoqpfdbh.html

npm init -y;  npm i express
来源：http://hz.52xcode.cn/gtkatbekip.html

[U82] JS：package.json 脚本
来源：http://hz.nanxuanxn.top/gthqjutwqu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.xylfe.cn/gtnhmipvxx.html

[U83] JS：ES Module 导入导出
来源：http://hz.jqgufenzy.top/gtbqftwrua.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.chenlongwang.top/gtwozbfjao.html

[U84] JS：CommonJS 写法
来源：http://hz.guowangkeji.top/gtarewxsjz.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.xziqi.cn/gtycecwmzz.html

[U85] JS：可选链
来源：http://hz.jinqigufen.top/gtnxknungj.html

a?.b?.c
来源：http://hz.yj20258888.top/gtbfloodeb.html

[U86] JS：空值合并
来源：http://hz.feifeiyinyue.top/gtmmtihtyi.html

a ?? b
来源：http://hz.jinghuilouyu.cn/gtbyxdndpf.html

[U87] JS：解构默认值
来源：http://hz.dianchejie.cn/gtxvkkfcmo.html

const { a = 1, b = 2 } = obj;
来源：http://hz.guowangkeji.top/gtjgjovrip.html

[U88] JS：对象展开合并
来源：http://hz.nanxinkj.top/gttdbwicpt.html

{ ...a, ...b }
来源：http://hz.wangshuangyany.cn/gtclhijoek.html

[U89] JS：数组去重
来源：http://hz.shuidangran.top/gtfcnqgnnk.html

[...new Set(arr)]
来源：http://hz.pengpengdd.cyou/gtvpdwbllq.html

[U90] JS：数字数组排序
来源：http://hz.yj20258.top/gtxfoacjrn.html

[...arr].sort((a, b) => a - b)
来源：http://hz.gogol.net.cn/gtxwetmqbq.html

[U91] JS：对象键值遍历
来源：http://hz.gogol.net.cn/gtqijtpmih.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.shuidangran.top/gtdbbtuokk.html

[U92] JS：深拷贝
来源：http://hz.yj202588.top/gtmfgccaln.html

structuredClone(obj)
来源：http://hz.yueranfly.top/gtvvzipczp.html

[U93] JS：模板字符串
来源：http://hz.daxiang520.top/gtenolirav.html

`共 ${n} 条`
来源：http://hz.chenzaomai.com/gtqrzafxbm.html

[U94] JS：箭头函数
来源：http://hz.cashguo.top/gtbacywuyd.html

const double = x => x * 2;
来源：http://hz.wangshuangyany.cn/gtviihdegc.html

[U95] JS：Promise 包装
来源：http://hz.vqdsnc.cn/gtovjrgoeg.html

new Promise((resolve, reject) => {})
来源：http://hz.vqdsnc.cn/gtjjjqtbcs.html

[U96] JS：async/await 与异常
来源：http://hz.zhixingplan.top/gtkuyfyuuu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.hfpthk.cn/gtqkugdrtn.html

[U97] JS：并发请求
来源：http://hz.snrcjt.cn/gtqcihehnn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinqigufen.top/gttspjaqyu.html

[U98] JS：fetch 带 JSON
来源：http://hz.jiagoushi.top/gtauobuwsq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yueranfly.top/gtbcwaqlcu.html

[U99] JS：事件监听
来源：http://hz.quarkkingdee.top/gthixxdshf.html

el.addEventListener("click", e => {})
来源：http://hz.chenjidiqi.icu/gtulrxulqh.html

[U100] JS：DOM 查询
来源：http://hz.ppjwa.cn/gtvaykbnqc.html

document.querySelector(".item")
来源：http://hz.xuanzx.com/gtdhoglaxi.html

[U101] JS：classList 操作
来源：http://hz.jinqigfzy.top/gtrunnfver.html

el.classList.toggle("active")
来源：http://hz.iojbl.cn/gtufoygcmt.html

[U102] JS：本地存储
来源：http://hz.hongshengwenyu.top/gtphuuvpsi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.shanyushiyangkeji.top/gtrfxzspwa.html

[U103] JS：定时器
来源：http://hz.zhiwuduotai.top/gtbmzwttcf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.jianghu66.top/gtdtcvmoge.html

[U104] JS：防抖
来源：http://hz.sufxvd.cn/gtleiqmiur.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sweek.top/gtiyjnytsb.html

[U105] JS：节流
来源：http://hz.guowangkeji.top/gtdpwblpzv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.vqdsnc.cn/gtsdjdjyzs.html

[U106] JS：日期格式化
来源：http://hz.sufxvd.cn/gtguqfibdl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.fengsongda.top/gterlbybao.html

[U107] JS：数字千分位
来源：http://hz.tanke756.top/gtlmlvhggn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zhengqikj.top/gtvnmyinac.html

[U108] JS：随机整数
来源：http://hz.haohaochexian.top/gtjofxrsrd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.mhx1999.top/gtkvszrpbj.html

[U109] JS：数组分组
来源：http://hz.xuanzx.com/gtgnvktcmw.html

Object.groupBy(arr, x => x.type)
来源：http://hz.gogol.net.cn/gtzlhghjis.html

[U110] JS：数组分块
来源：http://hz.mhx1999.top/gtoserbcpy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.sysykeji.top/gthlwfbnda.html

[U111] JS：对象转 Map
来源：http://hz.jinyuanbaomall.cn/gtiicxgdow.html

new Map(Object.entries(obj))
来源：http://hz.gogol.net.cn/gtgocjhivz.html

[U112] JS：字符串补位
来源：http://hz.zycfv.cn/gtwmwnkwvo.html

"7".padStart(3, "0")
来源：http://hz.fzhhl.top/gtzyapxuio.html

[U113] JS：正则替换全部
来源：http://hz.mhx1999.top/gtguokngwk.html

s.replaceAll("a", "b")
来源：http://hz.chenlongwang.top/gtfebysqpr.html

[U114] JS：JSON 深比较
来源：http://hz.jianghu66.top/gtdhbdnmup.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yongpay.top/gthclzpsfh.html

[U115] JS：生成 UUID
来源：http://hz.sweek.top/gtmxzpdinp.html

crypto.randomUUID()
来源：http://hz.shuidangran.top/gtmtvqqfvz.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.nanxuanxn.top/gtcpsmatse.html

/** @param {string} name */ function f(name) {}
来源：http://hz.zhixingplan.top/gtjgyxpswd.html

[U117] JS：单元测试
来源：http://hz.tanke756.top/gtrvqwjtde.html

npm i -D vitest;  npx vitest
来源：http://hz.jinqigufen.top/gtzwoopopj.html

[U118] JS：开发服务器
来源：http://hz.shanyushiyangtech.top/gtkbcwwuzb.html

npm i -D vite;  npx vite
来源：http://hz.hywenlv.cn/gtxzxdybrt.html

[U119] JS：生产构建
来源：http://hz.c1oappe.top/gtmhaqwzyr.html

npx vite build
来源：http://hz.nwbrower.top/gtmqzbgbrr.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.shangyingyoupin.top/gtaqfluryg.html

import.meta.env.VITE_API_URL
来源：http://hz.zhengqikj.top/gtsjsddrgx.html

================================================================================
来源：http://hz.pycfn.com/gtvgpchkjg.html

统计汇总
来源：http://hz.wangdashe.top/gtgkwavclv.html

================================================================================
来源：http://hz.iojbl.cn/gtkrwuiahv.html

按语言统计（条）：
来源：http://hz.gotoacloud.top/gtkwjdgzqd.html

Python ......... 252
来源：http://hz.hnqzz.top/gtvyzsbhrs.html

PHP ............ 252
来源：http://hz.yueranfly.top/gtyyoghopu.html

JavaScript ..... 252
来源：http://hz.hfpthk.cn/gtfaadlpnf.html

TypeScript ..... 212
来源：http://hz.chenjidiqi.icu/gtsfnkhdga.html

Java ........... 212
来源：http://hz.52xcode.cn/gtntcigrbq.html

Go ............. 212
来源：http://hz.pengpengdd.cyou/gtbqaifnef.html

Ruby ........... 212
来源：http://hz.52xcode.cn/gtxeyrpwhz.html

C# ............. 212
来源：http://hz.zhixingplan.top/gtfazyyohc.html

C .............. 30
来源：http://hz.tian-w.cn/gtcurndwmd.html

C++ ............ 30
来源：http://hz.jyoumei.cn/gtufzqanyp.html

SQL ............ 90
来源：http://hz.yongpay.top/gthyvavipg.html

Bash ........... 80
来源：http://hz.chenzaomai.com/gtqhaszkkr.html

Kotlin ......... 15
来源：http://hz.ivvv.top/gtllrcyolj.html

Swift .......... 15
来源：http://hz.xuetiantiany.cn/gtztyirkop.html

Lua ............ 10
来源：http://hz.xuetiantiany.cn/gtimguauqy.html

Perl ........... 10
来源：http://hz.0kj1m.cn/gtstopzpjg.html

Scala .......... 10
来源：http://hz.0kj1m.cn/gtdrhljjmv.html

------------------------------------
来源：http://hz.chenzaomai.com/gtpurylpaq.html

合计 ........... 2106 条
来源：http://hz.yuxming.cn/gtkizyioxr.html

按章节统计：
来源：http://hz.quarkkingdee.top/gtfaxxxxpt.html


<!-- 参考信息 -->