代发 wailian999

[T45] Perl：数组遍历
来源：http://hz.daria6918.cn/gtwkxvpynd.html

for my $x (@arr) { print $x; }
来源：http://hz.316326.xyz/gtqpuvmsgv.html

[T46] Perl：哈希操作
来源：http://hz.yueranfly.top/gteleoouxm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jinqigufen.top/gtulbpbspk.html

[T47] Perl：正则捕获
来源：http://hz.yj20258.top/gtzlrindyz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jiagoushi.top/gtmjvmpjin.html

[T48] Perl：正则替换
来源：http://hz.jqgfzy.top/gtopbkldnt.html

$s =~ s/old/new/g;
来源：http://hz.gogol.net.cn/gttlgdokfc.html

[T49] Perl：函数
来源：http://hz.mhx1999.top/gtsyzbsldm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.cqqwz.cn/gtwonvpeof.html

[T50] Perl：逐行读文件
来源：http://hz.iojbl.cn/gtxfkpjvvg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.9152youxi.cn/gtnkdrryay.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.sufxvd.cn/gtmavezbrc.html

[T51] Scala：Hello World
来源：http://hz.hnxiangtu.top/gttleplcvo.html

println("Hello")
来源：http://hz.jianghu66.top/gtforuwuiv.html

[T52] Scala：变量
来源：http://hz.jlsjyb.cn/gtylctniwg.html

val a = 1;  var b = 2
来源：http://hz.dianchejie.cn/gtzqmootqh.html

[T53] Scala：字符串插值
来源：http://hz.xziqi.cn/gtjddmwrpz.html

s"值: $b"
来源：http://hz.jqgfzy.top/gtibgoenlz.html

[T54] Scala：集合映射
来源：http://hz.jinqigfzy.top/gtaooevptb.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.hnqzz.top/gtnsejxrxj.html

[T55] Scala：集合过滤
来源：http://hz.bjfxy.top/gtbfujyivl.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.shzxlz.cn/gtlwqvxttj.html

[T56] Scala：样例类
来源：http://hz.jinyuanbaomall.cn/gtxnqbrbcq.html

case class User(name: String, age: Int)
来源：http://hz.ydzc1.top/gtisylmxye.html

[T57] Scala：模式匹配
来源：http://hz.bjfxy.top/gtddbauydr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.chenjidiqi.icu/gtdohhyjio.html

[T58] Scala：函数定义
来源：http://hz.jyoumei.cn/gturehnkpo.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.fengsongda.top/gtayypoyfu.html

[T59] Scala：循环
来源：http://hz.kuanghao11.cn/gtcztxbgey.html

for (i <- 1 to 10) println(i)
来源：http://hz.jinqigfzy.top/gtsjhlpkso.html

[T60] Scala：折叠
来源：http://hz.tianlin.xyz/gtjfdbgkou.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zycfv.cn/gtckzudjkc.html

================================================================================
来源：http://hz.hammf.cn/gtrtokrfzm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zycfv.cn/gtzibplojp.html

================================================================================
来源：http://hz.zhixingplan.top/gtvlgykhtd.html

[U01] Py：创建虚拟环境
来源：http://hz.yvedp.cn/gtieiloeah.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.feifeiyinyue.top/gtaehfutdo.html

[U02] Py：导出 / 安装依赖
来源：http://hz.xinyue.icu/gtcvedfgou.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.xuanzx.com/gtzeftxgov.html

[U03] Py：加载 .env 配置
来源：http://hz.ppjwa.cn/gtdvmnhory.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jinyuanbaomall.cn/gtsbhagxkl.html

[U04] Py：变量调试打印
来源：http://hz.jinghuilouyu.cn/gtwlfetwme.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jlsjyb.cn/gtybmeujnu.html

[U05] Py：列表去重且保序
来源：http://hz.shanyushiyangkeji.top/gtxsowondc.html

list(dict.fromkeys(arr))
来源：http://hz.yj20258.top/gtzftezkzy.html

[U06] Py：合并两个字典
来源：http://hz.snrcjt.cn/gtvgetltfa.html

{**a, **b}
来源：http://hz.feifeiyinyue.top/gtywqvzdki.html

[U07] Py：反转字典键值
来源：http://hz.shanyushiyangkeji.top/gtqkiqqnee.html

{v: k for k, v in d.items()}
来源：http://hz.feifeiyinyue.top/gtwhjuenfx.html

[U08] Py：展平二维列表
来源：http://hz.jyoumei.cn/gtxxnxyduw.html

[y for x in nested for y in x]
来源：http://hz.smart0.xyz/gtdctscekc.html

[U09] Py：字典取最大值的键
来源：http://hz.pengpengdd.cyou/gtajtfhkqz.html

max(d, key=d.get)
来源：http://hz.snrcjt.cn/gtkmrhnlai.html

[U10] Py：按值排序字典
来源：http://hz.yvedp.cn/gtpmsleltv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.dashuyun.cn/gtvzpkwdgh.html

[U11] Py：生成器表达式
来源：http://hz.gotoacloud.top/gtwomnijcg.html

(x * 2 for x in arr)
来源：http://hz.c1oappe.top/gtgcirssgv.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.jinyuanbaomall.cn/gtytpwoscd.html

Counter(arr).most_common(3)
来源：http://hz.jinghuilouyu.cn/gtmollgnrr.html

[U13] Py：固定长度队列
来源：http://hz.xuanzx.com/gtcwnyazmi.html

deque(maxlen=10)
来源：http://hz.sxryk.cn/gtgbjnhccr.html

[U14] Py：分组收集到列表
来源：http://hz.jqgufenzy.top/gtwiquoxvm.html

defaultdict(list)
来源：http://hz.chenlongwang.top/gtdjvxunaw.html

[U15] Py：高精度计时
来源：http://hz.sysykeji.top/gtgkklfjjl.html

t = time.perf_counter()
来源：http://hz.gogol.net.cn/gtyrrnqqad.html

[U16] Py：命令行参数解析
来源：http://hz.sweek.top/gtcfcmofob.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.zycfv.cn/gtynxezpsa.html

[U17] Py：初始化日志
来源：http://hz.yj202588.top/gtxonisfuy.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.vqdsnc.cn/gtzoveacch.html

[U18] Py：预编译正则
来源：http://hz.yangfankeji.com/gttdrbeqab.html

pat = re.compile(r"\d+")
来源：http://hz.zhoulong.xyz/gtmfsxabsx.html

[U19] Py：正则替换带回调
来源：http://hz.chenjidiqi.icu/gtwfhauokx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.xziqi.cn/gtithxvuan.html

[U20] Py：缓存函数结果
来源：http://hz.hammf.cn/gtdcxugavi.html

@functools.lru_cache(maxsize=None)
来源：http://hz.nanxinkj.top/gtjopilvdb.html

[U21] Py：自定义上下文管理器
来源：http://hz.xylfe.cn/gtvozsknin.html

@contextlib.contextmanager
来源：http://hz.birdmap.top/gtxgqdlgsi.html

[U22] Py：矩阵转置
来源：http://hz.pycfn.com/gtkykfkyux.html

list(zip(*m))
来源：http://hz.nwbrower.top/gtesjkkdpm.html

[U23] Py：分块读取大文件
来源：http://hz.xingfuxueyuan.xyz/gtdjyzsrrz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.dashuyun.cn/gtkxwzrlsx.html

[U24] Py：路径操作
来源：http://hz.zhoulong.xyz/gtpubpsgvt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.fzhhl.top/gtelrakhyn.html

[U25] Py：CSV 按字典读
来源：http://hz.xingfuxueyuan.xyz/gtkjcfzqum.html

csv.DictReader(f)
来源：http://hz.meibo888.top/gtqjokaxdr.html

[U26] Py：并发下载
来源：http://hz.dianchejie.cn/gtmwsahirv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.snrcjt.cn/gtjucuaijd.html

[U27] Py：异步 HTTP
来源：http://hz.c1oappe.top/gttaxkbxlj.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.tanke756.top/gtseuefwqv.html

[U28] Py：类型别名
来源：http://hz.hnqzz.top/gtocxqitwr.html

UserId = int
来源：http://hz.yj20258.top/gtallvewfr.html

[U29] Py：属性校验
来源：http://hz.jianghu66.top/gtzfcvikmx.html

@property 与 @x.setter 配合
来源：http://hz.hongshengwenyu.top/gtuiygyrhj.html

[U30] Py：数据类
来源：http://hz.yj202588.top/gtwzxmqbtq.html

@dataclass(slots=True)
来源：http://hz.gotoacloud.top/gtdlvgbapo.html

[U31] Py：单测
来源：http://hz.xuanzx.com/gtbgsicqds.html

python -m pytest -q
来源：http://hz.ywan-chungtsiang.top/gtddvfctgl.html

[U32] Py：代码格式化
来源：http://hz.zycfv.cn/gttloqrwjp.html

ruff format . && ruff check --fix .
来源：http://hz.sufxvd.cn/gtvfympdsp.html

[U33] Py：打包发布
来源：http://hz.birdmap.top/gtmbdbyrqb.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.tianlin.xyz/gtzxvjwzzi.html

[U34] Py：判断编码
来源：http://hz.52xcode.cn/gtllfrtqyh.html

chardet.detect(raw)
来源：http://hz.hongshengwenyu.top/gtbnavdirw.html

[U35] Py：发送邮件
来源：http://hz.hnqzz.top/gtzngyaess.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.shzxlz.cn/gtlydiybyp.html

[U36] Py：定时任务
来源：http://hz.yj202588.top/gtfzcbjxmn.html

schedule.every(10).minutes.do(job)
来源：http://hz.cucudq.cn/gtfshhrfmi.html

[U37] Py：读写 Excel
来源：http://hz.hongshengwenyu.top/gteehuwzcd.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.xylfe.cn/gtgnwphxns.html

[U38] Py：获取脚本所在目录
来源：http://hz.sysykeji.top/gtdmqnbbwd.html

Path(__file__).resolve().parent
来源：http://hz.mhx1999.top/gtxxypasfg.html

[U39] Py：判断是否在交互环境
来源：http://hz.fzhhl.top/gtgtjkxdpx.html

sys.stdout.isatty()
来源：http://hz.andypj.xyz/gtfesibxay.html

[U40] Py：打印到标准错误
来源：http://hz.0kj1m.cn/gtymvwwcny.html

print("err", file=sys.stderr)
来源：http://hz.wangshuangyany.cn/gtkysfztql.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.dianchejie.cn/gtklflyzdj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.hongshengwenyu.top/gtpvnscyoh.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.snrcjt.cn/gtfjghtxsu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.fzhhl.top/gtxpdxocwp.html

[U43] PHP：声明命名空间
来源：http://hz.zhongyouzk.top/gtnjsitjql.html

namespace App\Http;
来源：http://hz.chenlongwang.top/gtonviccdq.html

[U44] PHP：开启严格类型
来源：http://hz.ybcxt.top/gtivjovsqk.html

declare(strict_types=1);
来源：http://hz.shuidangran.top/gtjwniicqa.html

[U45] PHP：类型声明与返回类型
来源：http://hz.ybcxt.top/gtjfqqgajc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj20258.top/gteashufqr.html

[U46] PHP：可空类型
来源：http://hz.52xcode.cn/gtivfqwhtr.html

?string $name = null
来源：http://hz.zhengqikj.top/gtsmihkwpb.html

[U47] PHP：联合类型
来源：http://hz.hnqzz.top/gtjguzxxnd.html

int|string $id
来源：http://hz.yangfankeji.com/gtfqfybltq.html

[U48] PHP：纯枚举
来源：http://hz.gogol.net.cn/gtbxhohaod.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yuxming.cn/gtdcvbvauk.html

[U49] PHP：只读属性
来源：http://hz.xingfuxueyuan.xyz/gttgoajcza.html

public readonly string $name
来源：http://hz.chenlongwang.top/gtvoaxvzcm.html

[U50] PHP：构造器属性提升
来源：http://hz.jlsjyb.cn/gtpvtwlhxg.html

public function __construct(private int $id) {}
来源：http://hz.guowangkeji.top/gtvojhfthn.html

[U51] PHP：数组解构
来源：http://hz.yj20258888.top/gtggdmknzk.html

[$a, $b] = $arr;
来源：http://hz.hammf.cn/gtqhxzoheg.html

[U52] PHP：箭头函数
来源：http://hz.jlsjyb.cn/gtwjmofivw.html

$double = fn($x) => $x * 2;
来源：http://hz.yj202588.top/gtupakagok.html

[U53] PHP：空合并运算符
来源：http://hz.daxiang520.top/gtzxkfscuz.html

$v = $a ?? $b ?? "default";
来源：http://hz.xingfuxueyuan.xyz/gtkseqykjq.html

[U54] PHP：空安全调用
来源：http://hz.xinyue.icu/gtarzbrhjc.html

$obj?->method()
来源：http://hz.xuanzx.com/gtztclqwyi.html

[U55] PHP：match 表达式
来源：http://hz.wangshuangyany.cn/gtbaiutgqd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.xuetiantiany.cn/gtybjmbbqu.html

[U56] PHP：命名参数
来源：http://hz.fengsongda.top/gtqiszcbjq.html

f(a: 1, b: 2)
来源：http://hz.zhixingplan.top/gtblsmluqb.html

[U57] PHP：字符串插值
来源：http://hz.hfpthk.cn/gtjuarqzxk.html

"值: {$a}"
来源：http://hz.smart0.xyz/gtjuiqxjci.html

[U58] PHP：数组三件套
来源：http://hz.aibaodan.cn/gtyppxnnhm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.guannengcc.top/gtobykoguu.html

[U59] PHP：自定义排序
来源：http://hz.dianchejie.cn/gtyadqvbba.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhiwuduotai.top/gttiyuxgkf.html

[U60] PHP：JSON 编解码
来源：http://hz.ydjk.org.cn/gtgkizzykq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.pengpengdd.cyou/gtmmyukywm.html

[U61] PHP：正则
来源：http://hz.birdmap.top/gtfhbjerfr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.andypj.xyz/gtvwuvvlbf.html

[U62] PHP：日期对象
来源：http://hz.yj20258888.top/gtdnffzkgx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.ivvv.top/gtzsqyhhwg.html

[U63] PHP：文件读写
来源：http://hz.zhengqikj.top/gtyywfxjih.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.9152youxi.cn/gtsgagqrgt.html

[U64] PHP：目录遍历
来源：http://hz.zhixingplan.top/gtpmqcqyal.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.xziqi.cn/gtkbwpqxds.html

[U65] PHP：会话
来源：http://hz.jianghu66.top/gthqggyyhp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.svipenyu.cn/gtljrsbwiw.html

[U66] PHP：设置 Cookie
来源：http://hz.sxryk.cn/gtyfwxwovq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.fengsongda.top/gtoxsbcvxp.html

[U67] PHP：处理文件上传
来源：http://hz.tian-w.cn/gthdedotyf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.jinghuilouyu.cn/gtpnyibszd.html

[U68] PHP：PDO 连接
来源：http://hz.zhijiandao.cn/gtbodchosb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.cucudq.cn/gtkspqzkep.html

[U69] PHP：PDO 预处理
来源：http://hz.aizwys.cn/gtqlbowlof.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.zdqjudy.top/gtvohzauoo.html

[U70] PHP：PDO 事务
来源：http://hz.daria6918.cn/gtdzwkacxq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.zhiwuduotai.top/gtuuzdgmzm.html

[U71] PHP：抛出异常
来源：http://hz.jqgfzy.top/gtokcmonij.html

throw new RuntimeException("失败", 500);
来源：http://hz.316326.xyz/gtaxlutfoz.html

[U72] PHP：写错误日志
来源：http://hz.jyoumei.cn/gtjappbghf.html

error_log("失败: " . $e->getMessage());
来源：http://hz.zhixingplan.top/gtyajrmgyt.html

[U73] PHP：读取 ini 配置
来源：http://hz.mhx1999.top/gtlyycoyaa.html

parse_ini_file("config.ini", true)
来源：http://hz.shuidangran.top/gtbzyuddaf.html

[U74] PHP：读取环境变量
来源：http://hz.iojbl.cn/gtrsxhzmwp.html

getenv("APP_ENV") ?: "production"
来源：http://hz.yueranfly.top/gtuppcipwo.html

[U75] PHP：依赖注入
来源：http://hz.ehwqpu.com/gtgpivqcvp.html

composer require psr/container
来源：http://hz.jinqigfzy.top/gtzjzagjfn.html

[U76] PHP：简单路由
来源：http://hz.chenjidiqi.icu/gtsagvftuq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.cqqwz.cn/gtlqnfxtgy.html

[U77] PHP：模板渲染
来源：http://hz.zhongyouzk.top/gtwmcvcxhb.html

composer require twig/twig
来源：http://hz.hywenlv.cn/gtumxrnexr.html

[U78] PHP：单元测试
来源：http://hz.andypj.xyz/gtzozrudui.html

composer require --dev phpunit/phpunit
来源：http://hz.yonumen.top/gthknsgyfs.html

[U79] PHP：静态分析
来源：http://hz.shanyushiyangtech.top/gtdvjakcnh.html

composer require --dev phpstan/phpstan
来源：http://hz.meibo888.top/gtnpcpprme.html

[U80] PHP：代码规范修复
来源：http://hz.nwbrower.top/gtzsrdgbjy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.hongshengwenyu.top/gtyvjariqe.html

[U81] JS：初始化项目
来源：http://hz.cdnleiting.top/gtnkolekgl.html

npm init -y;  npm i express
来源：http://hz.daria6918.cn/gtegjxgjvj.html

[U82] JS：package.json 脚本
来源：http://hz.0kj1m.cn/gtjbmmclfi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.birdmap.top/gtwyktaynb.html

[U83] JS：ES Module 导入导出
来源：http://hz.jianghu66.top/gtjgllaavz.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yangfankeji.com/gtamyloeqs.html

[U84] JS：CommonJS 写法
来源：http://hz.xinyue.icu/gtollhvfef.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.bjfxy.top/gtmllyhzxe.html

[U85] JS：可选链
来源：http://hz.jinqigufen.top/gtvieckpmq.html

a?.b?.c
来源：http://hz.nanxinkj.top/gtcjttvlbp.html

[U86] JS：空值合并
来源：http://hz.yvedp.cn/gtotgmjiwj.html

a ?? b
来源：http://hz.cdnleiting.top/gtykhpjyhl.html

[U87] JS：解构默认值
来源：http://hz.shanyushiyangkeji.top/gtzhcvsrvv.html

const { a = 1, b = 2 } = obj;
来源：http://hz.jianghu66.top/gtowluonpi.html

[U88] JS：对象展开合并
来源：http://hz.gotoacloud.top/gtgmmyeboy.html

{ ...a, ...b }
来源：http://hz.aibaodan.cn/gtfvwiyedq.html

[U89] JS：数组去重
来源：http://hz.xziqi.cn/gttfvjqefv.html

[...new Set(arr)]
来源：http://hz.fzhhl.top/gtbiubneaf.html

[U90] JS：数字数组排序
来源：http://hz.xinyue.icu/gtgniaokvz.html

[...arr].sort((a, b) => a - b)
来源：http://hz.c1oappe.top/gtrldeisng.html

[U91] JS：对象键值遍历
来源：http://hz.hammf.cn/gtiiotgbyy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jinqigufen.top/gtbdcxzujh.html

[U92] JS：深拷贝
来源：http://hz.sweek.top/gtmmcobcys.html

structuredClone(obj)
来源：http://hz.yvedp.cn/gtkfdmybjp.html

[U93] JS：模板字符串
来源：http://hz.birdmap.top/gtpntuesms.html

`共 ${n} 条`
来源：http://hz.ydzc1.top/gtmbkbkyam.html

[U94] JS：箭头函数
来源：http://hz.iojbl.cn/gtjwjowbya.html

const double = x => x * 2;
来源：http://hz.fengsongda.top/gtmndqwkoi.html

[U95] JS：Promise 包装
来源：http://hz.shzxlz.cn/gthkvoefbl.html

new Promise((resolve, reject) => {})
来源：http://hz.hnxiangtu.top/gtysqmyzpj.html

[U96] JS：async/await 与异常
来源：http://hz.aibaodan.cn/gtjrnddexw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.sxryk.cn/gtygoujskb.html

[U97] JS：并发请求
来源：http://hz.dashuyun.cn/gtjblmygmt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hywenlv.cn/gtzrqtsbmq.html

[U98] JS：fetch 带 JSON
来源：http://hz.ppjwa.cn/gtevkoqcxj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.snrcjt.cn/gtnawbyjei.html

[U99] JS：事件监听
来源：http://hz.chenzaomai.com/gthetqfgsq.html

el.addEventListener("click", e => {})
来源：http://hz.aizwys.cn/gtotvvcfxh.html

[U100] JS：DOM 查询
来源：http://hz.meibo888.top/gtekuonevm.html

document.querySelector(".item")
来源：http://hz.jinghuilouyu.cn/gtskfuwywh.html

[U101] JS：classList 操作
来源：http://hz.jqgfzy.top/gtgpziknsc.html

el.classList.toggle("active")
来源：http://hz.dashuyun.cn/gtdtkznmgy.html

[U102] JS：本地存储
来源：http://hz.shanyushiyangtech.top/gtnhdiehmf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.xuetiantiany.cn/gtdqcdvhcr.html

[U103] JS：定时器
来源：http://hz.meibo888.top/gtrnffhiji.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.meibo888.top/gtoxphhbgv.html

[U104] JS：防抖
来源：http://hz.redwolf501.top/gtszsjlrqh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jqgufenzy.top/gtniekzrky.html

[U105] JS：节流
来源：http://hz.zhongyouzk.top/gtqaayoxym.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.cucudq.cn/gtrqtpuaxj.html

[U106] JS：日期格式化
来源：http://hz.ybcxt.top/gtjjqgobcr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.jiagoushi.top/gtymnemfar.html

[U107] JS：数字千分位
来源：http://hz.yj20258.top/gttrwekhjg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.ehwqpu.com/gtrpjoqofx.html

[U108] JS：随机整数
来源：http://hz.tanke756.top/gtycsljaht.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yueranfly.top/gturpepmtt.html

[U109] JS：数组分组
来源：http://hz.shuidangran.top/gtjcuknnrt.html

Object.groupBy(arr, x => x.type)
来源：http://hz.zhixingplan.top/gteoydrcaz.html

[U110] JS：数组分块
来源：http://hz.jyoumei.cn/gtowkcixjx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.9152youxi.cn/gtviisbfet.html

[U111] JS：对象转 Map
来源：http://hz.snrcjt.cn/gtafiwvrge.html

new Map(Object.entries(obj))
来源：http://hz.shzxlz.cn/gtqbjzyzug.html

[U112] JS：字符串补位
来源：http://hz.yuxming.cn/gtgegfnqqs.html

"7".padStart(3, "0")
来源：http://hz.ppjwa.cn/gtufozlcyy.html

[U113] JS：正则替换全部
来源：http://hz.wangshuangyany.cn/gtwtgwiqrs.html

s.replaceAll("a", "b")
来源：http://hz.nwbrower.top/gtojlfrffx.html

[U114] JS：JSON 深比较
来源：http://hz.zhixingplan.top/gtgcsdtcbo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cdnleiting.top/gtooqvogcd.html

[U115] JS：生成 UUID
来源：http://hz.xziqi.cn/gtvwwujrus.html

crypto.randomUUID()
来源：http://hz.shuidangran.top/gtkqrxeoyg.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.birdmap.top/gtqvfbgzsm.html

/** @param {string} name */ function f(name) {}
来源：http://hz.jinqigfzy.top/gtcpxwyfmr.html

[U117] JS：单元测试
来源：http://hz.kuanghao11.cn/gtfneprswm.html

npm i -D vitest;  npx vitest
来源：http://hz.ydzc1.top/gtodfyhpcz.html

[U118] JS：开发服务器
来源：http://hz.quarkkingdee.top/gtaowefwyv.html

npm i -D vite;  npx vite
来源：http://hz.zhaomingkeji.xyz/gtzmqdkruo.html

[U119] JS：生产构建
来源：http://hz.ydjk.org.cn/gteucolegk.html

npx vite build
来源：http://hz.pycfn.com/gtsvkuxamp.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.xylfe.cn/gtodjnvkyy.html

import.meta.env.VITE_API_URL
来源：http://hz.gotoacloud.top/gtnzifryma.html

================================================================================
来源：http://hz.shuidangran.top/gtgdeshhju.html

统计汇总
来源：http://hz.bjfxy.top/gtiplofknx.html

================================================================================
来源：http://hz.nwbrower.top/gtkpswdmvu.html

按语言统计（条）：
来源：http://hz.nanxuanxn.top/gtwzwxtdhl.html

Python ......... 252
来源：http://hz.havefunace.top/gtzaqebhtb.html

PHP ............ 252
来源：http://hz.dashuyun.cn/gthixxvrbv.html

JavaScript ..... 252
来源：http://hz.zhixingplan.top/gtabkthcyy.html

TypeScript ..... 212
来源：http://hz.ybcxt.top/gtiubatjxy.html

Java ........... 212
来源：http://hz.jinqigfzy.top/gtltswuhps.html

Go ............. 212
来源：http://hz.ppjwa.cn/gtvzhjlxqp.html

Ruby ........... 212
来源：http://hz.dianchejie.cn/gtpjamawhg.html

C# ............. 212
来源：http://hz.shzxlz.cn/gtzebbcgnq.html

C .............. 30
来源：http://hz.shangyingyoupin.top/gtzinpxumj.html

C++ ............ 30
来源：http://hz.ydjk.org.cn/gtfeaxxroq.html

SQL ............ 90
来源：http://hz.nanxinkj.top/gtsthqexnz.html

Bash ........... 80
来源：http://hz.gzhubu.top/gtecicszee.html

Kotlin ......... 15
来源：http://hz.xinyue.icu/gtqbatzlew.html

Swift .......... 15
来源：http://hz.tanke756.top/gtzvweewus.html

Lua ............ 10
来源：http://hz.yuanzhike.top/gthstnvzsz.html

Perl ........... 10
来源：http://hz.aibaodan.cn/gtppnibdzf.html

Scala .......... 10
来源：http://hz.shanyushiyangkeji.top/gtpmwjpgsr.html

------------------------------------
来源：http://hz.gzhubu.top/gtzcsceaqo.html

合计 ........... 2106 条
来源：http://hz.andypj.xyz/gtznmmlxzj.html

按章节统计：
来源：http://hz.tanke756.top/gtwewhlhzb.html


<!-- 参考信息 -->