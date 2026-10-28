代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://hz.tianlin.xyz/gtalpxnpcc.html

[T55] Scala：集合过滤
来源：http://hz.xinyue.icu/gttsqtylcx.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jinyuanbaomall.cn/gtphchpgev.html

[T56] Scala：样例类
来源：http://hz.jinqigfzy.top/gtxnrlkzuq.html

case class User(name: String, age: Int)
来源：http://hz.tianlin.xyz/gtwidwmhuy.html

[T57] Scala：模式匹配
来源：http://hz.cdnleiting.top/gtyfquczbb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.pycfn.com/gtrxhjxukt.html

[T58] Scala：函数定义
来源：http://hz.xylfe.cn/gtzdwqegtz.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.tianlin.xyz/gthwgwjfkg.html

[T59] Scala：循环
来源：http://hz.ywan-chungtsiang.top/gthjzpqjzh.html

for (i <- 1 to 10) println(i)
来源：http://hz.cqqwz.cn/gtvbskifop.html

[T60] Scala：折叠
来源：http://hz.wangshuangyany.cn/gtffythslm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hammf.cn/gtaewgpipr.html

================================================================================
来源：http://hz.cqqwz.cn/gtennmegrp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yj20258888.top/gtjjdwlfrr.html

================================================================================
来源：http://hz.zhongyouzk.top/gtaieebfck.html

[U01] Py：创建虚拟环境
来源：http://hz.yangfankeji.com/gtmndchiyu.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.snrcjt.cn/gtjkhcdqai.html

[U02] Py：导出 / 安装依赖
来源：http://hz.pengpengdd.cyou/gtfjpneijk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.shuidangran.top/gtvcwlpzko.html

[U03] Py：加载 .env 配置
来源：http://hz.xuetiantiany.cn/gtueworygp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jyoumei.cn/gthjgxmpnt.html

[U04] Py：变量调试打印
来源：http://hz.9152youxi.cn/gtsstjybfm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jiagoushi.top/gtuahfgeis.html

[U05] Py：列表去重且保序
来源：http://hz.xingfuxueyuan.xyz/gtepaftcae.html

list(dict.fromkeys(arr))
来源：http://hz.xuetiantiany.cn/gtjzchcftt.html

[U06] Py：合并两个字典
来源：http://hz.sweek.top/gtnyymvruq.html

{**a, **b}
来源：http://hz.jinqigfzy.top/gtjopdcnjh.html

[U07] Py：反转字典键值
来源：http://hz.jqgfzy.top/gtcrlxyhfs.html

{v: k for k, v in d.items()}
来源：http://hz.tianlin.xyz/gtzunsfhhy.html

[U08] Py：展平二维列表
来源：http://hz.dianchejie.cn/gtozxdovnp.html

[y for x in nested for y in x]
来源：http://hz.shanyushiyangkeji.top/gthlpmtsos.html

[U09] Py：字典取最大值的键
来源：http://hz.chenzaomai.com/gtjmurgtol.html

max(d, key=d.get)
来源：http://hz.jinghuilouyu.cn/gtxgqejwim.html

[U10] Py：按值排序字典
来源：http://hz.birdmap.top/gtliiqvalu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.zdqjudy.top/gtfjjnrglj.html

[U11] Py：生成器表达式
来源：http://hz.redwolf501.top/gtwigbvxen.html

(x * 2 for x in arr)
来源：http://hz.aibaodan.cn/gtwhsjolbq.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zdqjudy.top/gtgsjmvxxh.html

Counter(arr).most_common(3)
来源：http://hz.jlsjyb.cn/gtjepwfknt.html

[U13] Py：固定长度队列
来源：http://hz.c1oappe.top/gtekeqyfsq.html

deque(maxlen=10)
来源：http://hz.aibaodan.cn/gtavuukbuh.html

[U14] Py：分组收集到列表
来源：http://hz.cqqwz.cn/gtjrspbyjv.html

defaultdict(list)
来源：http://hz.zhoulong.xyz/gtypbjrzbw.html

[U15] Py：高精度计时
来源：http://hz.meibo888.top/gtudvcnoee.html

t = time.perf_counter()
来源：http://hz.redwolf501.top/gtiocgolky.html

[U16] Py：命令行参数解析
来源：http://hz.xingfuxueyuan.xyz/gtppstoneh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.xuanzx.com/gtgomywjcc.html

[U17] Py：初始化日志
来源：http://hz.9152youxi.cn/gthpywreta.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.wangshuangyany.cn/gtzyjxmznn.html

[U18] Py：预编译正则
来源：http://hz.tianlin.xyz/gtliyznwpw.html

pat = re.compile(r"\d+")
来源：http://hz.wangshuangyany.cn/gtxgzayvyv.html

[U19] Py：正则替换带回调
来源：http://hz.guannengcc.top/gtqyubrjtt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.quarkkingdee.top/gtvgofwgmo.html

[U20] Py：缓存函数结果
来源：http://hz.iojbl.cn/gtjxtpfcqz.html

@functools.lru_cache(maxsize=None)
来源：http://hz.xuetiantiany.cn/gtwdyarzmj.html

[U21] Py：自定义上下文管理器
来源：http://hz.quarkkingdee.top/gtoebggcdw.html

@contextlib.contextmanager
来源：http://hz.zhongyouzk.top/gtiyakaxxp.html

[U22] Py：矩阵转置
来源：http://hz.jiagoushi.top/gtcvwhfqxh.html

list(zip(*m))
来源：http://hz.zhaomingkeji.xyz/gtqclwqgjq.html

[U23] Py：分块读取大文件
来源：http://hz.havefunace.top/gtbrhstayn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.zycfv.cn/gtctdrlizj.html

[U24] Py：路径操作
来源：http://hz.316326.xyz/gthhvghptx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.gogol.net.cn/gtoqfryhqy.html

[U25] Py：CSV 按字典读
来源：http://hz.haohaochexian.top/gtwxmrjhec.html

csv.DictReader(f)
来源：http://hz.jinqigufen.top/gtagsyyana.html

[U26] Py：并发下载
来源：http://hz.xuanzx.com/gtpyqqcijg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.52xcode.cn/gtzfdlwcwl.html

[U27] Py：异步 HTTP
来源：http://hz.pycfn.com/gtlmgsyvcf.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.fengsongda.top/gtfbanbhrk.html

[U28] Py：类型别名
来源：http://hz.sxryk.cn/gttjpxsdrz.html

UserId = int
来源：http://hz.gaohongyu789.top/gtydfafotu.html

[U29] Py：属性校验
来源：http://hz.redwolf501.top/gtnrekwlja.html

@property 与 @x.setter 配合
来源：http://hz.vqdsnc.cn/gtblrcyyos.html

[U30] Py：数据类
来源：http://hz.shangyingyoupin.top/gtsiveirum.html

@dataclass(slots=True)
来源：http://hz.dashuyun.cn/gtrwetofbw.html

[U31] Py：单测
来源：http://hz.hnxiangtu.top/gtrtokibrq.html

python -m pytest -q
来源：http://hz.zhongyouzk.top/gtlcctgrxb.html

[U32] Py：代码格式化
来源：http://hz.yvedp.cn/gtzzxcwvkq.html

ruff format . && ruff check --fix .
来源：http://hz.52xcode.cn/gtvoekscua.html

[U33] Py：打包发布
来源：http://hz.yvedp.cn/gtuivwejoh.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.xziqi.cn/gtxeqnamou.html

[U34] Py：判断编码
来源：http://hz.redwolf501.top/gtdazaltso.html

chardet.detect(raw)
来源：http://hz.0kj1m.cn/gteoqonhsi.html

[U35] Py：发送邮件
来源：http://hz.fengsongda.top/gtpmhfxljq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.jinqigufen.top/gtbrazcldh.html

[U36] Py：定时任务
来源：http://hz.ydzc1.top/gtxlsebqfa.html

schedule.every(10).minutes.do(job)
来源：http://hz.andypj.xyz/gtafdswrvt.html

[U37] Py：读写 Excel
来源：http://hz.shanyushiyangtech.top/gtktydshkm.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.xinyue.icu/gtkijipvub.html

[U38] Py：获取脚本所在目录
来源：http://hz.hysaishi.cn/gtumtiwuce.html

Path(__file__).resolve().parent
来源：http://hz.cqqwz.cn/gtumrivglg.html

[U39] Py：判断是否在交互环境
来源：http://hz.zhiwuduotai.top/gtsbsogzhu.html

sys.stdout.isatty()
来源：http://hz.jiagoushi.top/gtljfjhdbc.html

[U40] Py：打印到标准错误
来源：http://hz.hammf.cn/gtrvkcnrbm.html

print("err", file=sys.stderr)
来源：http://hz.shzxlz.cn/gtkwrtqrpv.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.hywenlv.cn/gthjenkvcb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.nanxuanxn.top/gtlcfszyns.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.sufxvd.cn/gtsdjpzohe.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.shanyushiyangtech.top/gtahkjluqy.html

[U43] PHP：声明命名空间
来源：http://hz.jqgufenzy.top/gtamwgotyg.html

namespace App\Http;
来源：http://hz.9152youxi.cn/gtvjhndblv.html

[U44] PHP：开启严格类型
来源：http://hz.shanyushiyangkeji.top/gthajeitln.html

declare(strict_types=1);
来源：http://hz.hysaishi.cn/gtuzrspiek.html

[U45] PHP：类型声明与返回类型
来源：http://hz.hywenlv.cn/gtevltfmfb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhixingplan.top/gtrptsywkq.html

[U46] PHP：可空类型
来源：http://hz.zhixingplan.top/gtnhlsgfca.html

?string $name = null
来源：http://hz.zdqjudy.top/gtymmobvzz.html

[U47] PHP：联合类型
来源：http://hz.yj20258888.top/gtjxnblvpf.html

int|string $id
来源：http://hz.iojbl.cn/gtakgbfyvr.html

[U48] PHP：纯枚举
来源：http://hz.yongpay.top/gtnuxuqjff.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.zhixingplan.top/gtzzuhgxcr.html

[U49] PHP：只读属性
来源：http://hz.cucudq.cn/gtgujzprax.html

public readonly string $name
来源：http://hz.zhaomingkeji.xyz/gtdzeptixa.html

[U50] PHP：构造器属性提升
来源：http://hz.zhengqikj.top/gtmlhrxeus.html

public function __construct(private int $id) {}
来源：http://hz.jinghuilouyu.cn/gtinoupaet.html

[U51] PHP：数组解构
来源：http://hz.hammf.cn/gtsuqgzkas.html

[$a, $b] = $arr;
来源：http://hz.zdqjudy.top/gtwxnojnos.html

[U52] PHP：箭头函数
来源：http://hz.ehwqpu.com/gtkxsutkwn.html

$double = fn($x) => $x * 2;
来源：http://hz.cucudq.cn/gtqwsifisy.html

[U53] PHP：空合并运算符
来源：http://hz.ydjk.org.cn/gtqdivjvrj.html

$v = $a ?? $b ?? "default";
来源：http://hz.feifeiyinyue.top/gtywvgstkm.html

[U54] PHP：空安全调用
来源：http://hz.0kj1m.cn/gtubeulbir.html

$obj?->method()
来源：http://hz.nanxuanxn.top/gtbfytkqve.html

[U55] PHP：match 表达式
来源：http://hz.yuanzhike.top/gticjbopmp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.c1oappe.top/gtvxafzpuo.html

[U56] PHP：命名参数
来源：http://hz.havefunace.top/gtexvyowqh.html

f(a: 1, b: 2)
来源：http://hz.cdnleiting.top/gtrebguqlk.html

[U57] PHP：字符串插值
来源：http://hz.jiagoushi.top/gtfebzjvxd.html

"值: {$a}"
来源：http://hz.hnqzz.top/gtrqoavylx.html

[U58] PHP：数组三件套
来源：http://hz.yueranfly.top/gtjnbkohxi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.gotoacloud.top/gtdhsfkhvh.html

[U59] PHP：自定义排序
来源：http://hz.xingfuxueyuan.xyz/gtneubxtkc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yueranfly.top/gtgmshkquz.html

[U60] PHP：JSON 编解码
来源：http://hz.yj202588.top/gtyvsjcsnn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.yj20258888.top/gtotmruqwi.html

[U61] PHP：正则
来源：http://hz.0kj1m.cn/gtycqlkhas.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.xingfuxueyuan.xyz/gtvpptrhmr.html

[U62] PHP：日期对象
来源：http://hz.chenjidiqi.icu/gtcfiecdms.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.cqqwz.cn/gtedqikncn.html

[U63] PHP：文件读写
来源：http://hz.feifeiyinyue.top/gtbzqfplkz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.fzhhl.top/gtfxlzgzav.html

[U64] PHP：目录遍历
来源：http://hz.yj20258.top/gtkvxwsgut.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.zdqjudy.top/gtybvtsubd.html

[U65] PHP：会话
来源：http://hz.jinghuilouyu.cn/gtmztijmjo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.redwolf501.top/gtaopylgvq.html

[U66] PHP：设置 Cookie
来源：http://hz.snrcjt.cn/gtfuusvqyt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yanxiufei.cn/gtphmbrmgh.html

[U67] PHP：处理文件上传
来源：http://hz.iojbl.cn/gtzgfawtte.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.xylfe.cn/gtaizumwev.html

[U68] PHP：PDO 连接
来源：http://hz.sufxvd.cn/gtubdblmqz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.gogol.net.cn/gtfdfkzzgf.html

[U69] PHP：PDO 预处理
来源：http://hz.jinqigufen.top/gtvmktiqvq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.sufxvd.cn/gtvzvbclsu.html

[U70] PHP：PDO 事务
来源：http://hz.xinyue.icu/gttwigjngx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.yj202588.top/gtcomxexku.html

[U71] PHP：抛出异常
来源：http://hz.tian-w.cn/gtydcxyttn.html

throw new RuntimeException("失败", 500);
来源：http://hz.kuanghao11.cn/gtjlgocdoi.html

[U72] PHP：写错误日志
来源：http://hz.dashuyun.cn/gtnogthhxm.html

error_log("失败: " . $e->getMessage());
来源：http://hz.yanxiufei.cn/gtisfpbmkd.html

[U73] PHP：读取 ini 配置
来源：http://hz.tanke756.top/gtbtutdyog.html

parse_ini_file("config.ini", true)
来源：http://hz.nwbrower.top/gttrlxevxm.html

[U74] PHP：读取环境变量
来源：http://hz.snrcjt.cn/gtlhczpaay.html

getenv("APP_ENV") ?: "production"
来源：http://hz.yj20258.top/gtkoqumfxo.html

[U75] PHP：依赖注入
来源：http://hz.andypj.xyz/gtynpiwmwd.html

composer require psr/container
来源：http://hz.mhx1999.top/gtfkixueur.html

[U76] PHP：简单路由
来源：http://hz.jqgufenzy.top/gtqdpwjlqr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.hnqzz.top/gtdjarxujg.html

[U77] PHP：模板渲染
来源：http://hz.birdmap.top/gtsayllofg.html

composer require twig/twig
来源：http://hz.jqgfzy.top/gtmcdxrzpd.html

[U78] PHP：单元测试
来源：http://hz.birdmap.top/gtkezrjbkr.html

composer require --dev phpunit/phpunit
来源：http://hz.316326.xyz/gtiavjulxy.html

[U79] PHP：静态分析
来源：http://hz.cqqwz.cn/gterngcqtn.html

composer require --dev phpstan/phpstan
来源：http://hz.svipenyu.cn/gtsljustdz.html

[U80] PHP：代码规范修复
来源：http://hz.shuidangran.top/gtbpvzodhs.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.fengsongda.top/gtjweyvqdw.html

[U81] JS：初始化项目
来源：http://hz.hywenlv.cn/gtllbfcrth.html

npm init -y;  npm i express
来源：http://hz.shzxlz.cn/gtgototqsx.html

[U82] JS：package.json 脚本
来源：http://hz.xylfe.cn/gtvutyohhd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.snrcjt.cn/gtqkzhvlth.html

[U83] JS：ES Module 导入导出
来源：http://hz.birdmap.top/gtzprwhyvu.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.ydjk.org.cn/gtyeeodtbg.html

[U84] JS：CommonJS 写法
来源：http://hz.jinqigufen.top/gteabxkksf.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.hongshengwenyu.top/gtpowevnej.html

[U85] JS：可选链
来源：http://hz.sufxvd.cn/gtxwhqwjgv.html

a?.b?.c
来源：http://hz.zycfv.cn/gtpspffynh.html

[U86] JS：空值合并
来源：http://hz.gaohongyu789.top/gtvgtnmblm.html

a ?? b
来源：http://hz.ywan-chungtsiang.top/gtitnlddcg.html

[U87] JS：解构默认值
来源：http://hz.hywenlv.cn/gtqhhygojf.html

const { a = 1, b = 2 } = obj;
来源：http://hz.zhijiandao.cn/gtfajhbdin.html

[U88] JS：对象展开合并
来源：http://hz.cdnleiting.top/gtdkoobdvf.html

{ ...a, ...b }
来源：http://hz.cdnleiting.top/gtwlvhjodz.html

[U89] JS：数组去重
来源：http://hz.gaohongyu789.top/gtgapgkjul.html

[...new Set(arr)]
来源：http://hz.shuidangran.top/gtlxseuroq.html

[U90] JS：数字数组排序
来源：http://hz.smart0.xyz/gttwhxprwx.html

[...arr].sort((a, b) => a - b)
来源：http://hz.dashuyun.cn/gtcdqdwhat.html

[U91] JS：对象键值遍历
来源：http://hz.jlsjyb.cn/gtmzxfczko.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.ydzc1.top/gtcfijsqnp.html

[U92] JS：深拷贝
来源：http://hz.gaohongyu789.top/gtpqzjwrga.html

structuredClone(obj)
来源：http://hz.shangyingyoupin.top/gtqsryjzyw.html

[U93] JS：模板字符串
来源：http://hz.pycfn.com/gtcqvxihxt.html

`共 ${n} 条`
来源：http://hz.nwbrower.top/gtglavpoxn.html

[U94] JS：箭头函数
来源：http://hz.shanyushiyangkeji.top/gtapqfybuj.html

const double = x => x * 2;
来源：http://hz.jinyuanbaomall.cn/gtuynnoftf.html

[U95] JS：Promise 包装
来源：http://hz.sweek.top/gtcrjdlmdl.html

new Promise((resolve, reject) => {})
来源：http://hz.xylfe.cn/gtzjbutpbq.html

[U96] JS：async/await 与异常
来源：http://hz.ybcxt.top/gtgoaorufg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.zhoulong.xyz/gtkymynisr.html

[U97] JS：并发请求
来源：http://hz.gotoacloud.top/gtfxhgkhdg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.vqdsnc.cn/gtkrjentzq.html

[U98] JS：fetch 带 JSON
来源：http://hz.hnxiangtu.top/gttoigngzr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.zhongyouzk.top/gttyfxixuf.html

[U99] JS：事件监听
来源：http://hz.yangfankeji.com/gtroruehad.html

el.addEventListener("click", e => {})
来源：http://hz.yueranfly.top/gtefbyzlbg.html

[U100] JS：DOM 查询
来源：http://hz.zhongyouzk.top/gtdsojxqov.html

document.querySelector(".item")
来源：http://hz.yvedp.cn/gthputezss.html

[U101] JS：classList 操作
来源：http://hz.jlsjyb.cn/gtflbbqtko.html

el.classList.toggle("active")
来源：http://hz.shuidangran.top/gtqwwchpek.html

[U102] JS：本地存储
来源：http://hz.dashuyun.cn/gtoscifhfa.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.9152youxi.cn/gtxpgspkdj.html

[U103] JS：定时器
来源：http://hz.pengpengdd.cyou/gthcosyucj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zhiwuduotai.top/gttnfxobgs.html

[U104] JS：防抖
来源：http://hz.pycfn.com/gtpgulbhge.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj202588.top/gtglsvdbrl.html

[U105] JS：节流
来源：http://hz.vqdsnc.cn/gtjiuaqwxf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.snrcjt.cn/gtdbdlcyhf.html

[U106] JS：日期格式化
来源：http://hz.sufxvd.cn/gtwmbvebbv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yanxiufei.cn/gtnjgsyazm.html

[U107] JS：数字千分位
来源：http://hz.wangdashe.top/gtrzfjkifb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.ehwqpu.com/gtsbrzizra.html

[U108] JS：随机整数
来源：http://hz.nanxuanxn.top/gtetxpwbjb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yongpay.top/gtmnmryfll.html

[U109] JS：数组分组
来源：http://hz.52xcode.cn/gtxhbwrwts.html

Object.groupBy(arr, x => x.type)
来源：http://hz.yonumen.top/gtfawvxjcl.html

[U110] JS：数组分块
来源：http://hz.yj202588.top/gttxxrykcd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yonumen.top/gtqwrcfktp.html

[U111] JS：对象转 Map
来源：http://hz.yuanzhike.top/gtknxnnvmm.html

new Map(Object.entries(obj))
来源：http://hz.pengpengdd.cyou/gtruovuwio.html

[U112] JS：字符串补位
来源：http://hz.yonumen.top/gteyzkiokp.html

"7".padStart(3, "0")
来源：http://hz.jianghu66.top/gtkdirdxee.html

[U113] JS：正则替换全部
来源：http://hz.tian-w.cn/gtjjlwspgp.html

s.replaceAll("a", "b")
来源：http://hz.jqgufenzy.top/gttkpupvii.html

[U114] JS：JSON 深比较
来源：http://hz.hammf.cn/gtszqdsbzf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhongyouzk.top/gtkhciboqr.html

[U115] JS：生成 UUID
来源：http://hz.yueranfly.top/gtfqnnpeot.html

crypto.randomUUID()
来源：http://hz.iojbl.cn/gtmtobkgrf.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.smart0.xyz/gtgklmenhv.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yuxming.cn/gtynaaikpw.html

[U117] JS：单元测试
来源：http://hz.shzxlz.cn/gtxmweqqdg.html

npm i -D vitest;  npx vitest
来源：http://hz.c1oappe.top/gtngyvktbk.html

[U118] JS：开发服务器
来源：http://hz.birdmap.top/gtemqtiara.html

npm i -D vite;  npx vite
来源：http://hz.yj20258.top/gtcxfnjzeh.html

[U119] JS：生产构建
来源：http://hz.cheryme.top/gtdtzvpglr.html

npx vite build
来源：http://hz.9152youxi.cn/gtztvzrazo.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yj202588.top/gtccseamgu.html

import.meta.env.VITE_API_URL
来源：http://hz.yuxming.cn/gtgmxgqgik.html

================================================================================
来源：http://hz.gotoacloud.top/gtvmfvhryg.html

统计汇总
来源：http://hz.tian-w.cn/gtpnygddvx.html

================================================================================
来源：http://hz.daria6918.cn/gtjqkyhsob.html

按语言统计（条）：
来源：http://hz.smart0.xyz/gtiryrllhd.html

Python ......... 252
来源：http://hz.cheryme.top/gthgibzyxo.html

PHP ............ 252
来源：http://hz.kuanghao11.cn/gtiaqifecy.html

JavaScript ..... 252
来源：http://hz.xuetiantiany.cn/gtqaggcajc.html

TypeScript ..... 212
来源：http://hz.yangfankeji.com/gtvdtkkidl.html

Java ........... 212
来源：http://hz.aizwys.cn/gtestrhrvh.html

Go ............. 212
来源：http://hz.shanyushiyangtech.top/gtfiawvlja.html

Ruby ........... 212
来源：http://hz.yanxiufei.cn/gtmtvocjvq.html

C# ............. 212
来源：http://hz.mhx1999.top/gtgoubajec.html

C .............. 30
来源：http://hz.guannengcc.top/gtxjqycqmu.html

C++ ............ 30
来源：http://hz.daria6918.cn/gtfddyfkso.html

SQL ............ 90
来源：http://hz.zhijiandao.cn/gtnvfdutzr.html

Bash ........... 80
来源：http://hz.zhengqikj.top/gtswgiybmo.html

Kotlin ......... 15
来源：http://hz.cheryme.top/gtwtupshak.html

Swift .......... 15
来源：http://hz.cqqwz.cn/gtdebknvnx.html

Lua ............ 10
来源：http://hz.bjfxy.top/gthcgrdtil.html

Perl ........... 10
来源：http://hz.sweek.top/gtzonpphqo.html

Scala .......... 10
来源：http://hz.daxiang520.top/gtuoyrgpii.html

------------------------------------
来源：http://hz.daxiang520.top/gtuslishue.html

合计 ........... 2106 条
来源：http://hz.jqgufenzy.top/gtvbotwdys.html

按章节统计：
来源：http://hz.yuanzhike.top/gtbjsctsut.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.c1oappe.top/gtucvhloup.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.sysykeji.top/gtjsjmafgd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jianghu66.top/gtfguerdhl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.xinyue.icu/gtrymuqhtp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.ivvv.top/gtkgjhaxlg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.ivvv.top/gtwculktqe.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.tian-w.cn/gtnsbkrcxf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zhiwuduotai.top/gttrawtvcx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.nanxuanxn.top/gtbgzodtde.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.zhoulong.xyz/gtkbygcwcv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.zhijiandao.cn/gteztxtftc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yvedp.cn/gtenkmqasp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zycfv.cn/gtfqmzkzvy.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.haohaochexian.top/gtqyykhgsw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.zhijiandao.cn/gtpzkhxhoz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.haohaochexian.top/gtmgjyckex.html

Q SQL 专题                              90
来源：http://hz.yuxming.cn/gtigiqfcnn.html

R Bash 专题                             80
来源：http://hz.birdmap.top/gtheommhys.html

S C / C++ 专题                          60
来源：http://hz.hnxiangtu.top/gtghcwfgse.html

T 其他语言补充                          60
来源：http://hz.jlsjyb.cn/gtycstjfyb.html


<!-- 参考信息 -->