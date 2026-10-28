代发 wailian999

[U07] Py：反转字典键值
来源：http://hz.yj202588.top/gtmztjotbs.html

{v: k for k, v in d.items()}
来源：http://hz.dashuyun.cn/gtnuoepmbn.html

[U08] Py：展平二维列表
来源：http://hz.zhongyouzk.top/gtamvhmjcq.html

[y for x in nested for y in x]
来源：http://hz.redwolf501.top/gtgjnphhlv.html

[U09] Py：字典取最大值的键
来源：http://hz.shzxlz.cn/gtzawvhoiu.html

max(d, key=d.get)
来源：http://hz.jiagoushi.top/gtpvndrutw.html

[U10] Py：按值排序字典
来源：http://hz.fengsongda.top/gtpqwqmbdg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yuxming.cn/gtgylagtxe.html

[U11] Py：生成器表达式
来源：http://hz.jiagoushi.top/gtvoelpjwd.html

(x * 2 for x in arr)
来源：http://hz.pengpengdd.cyou/gtvvovylwk.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.chenzaomai.com/gthfqktate.html

Counter(arr).most_common(3)
来源：http://hz.jinqigfzy.top/gtmmxznepw.html

[U13] Py：固定长度队列
来源：http://hz.mhx1999.top/gtcufveicm.html

deque(maxlen=10)
来源：http://hz.tian-w.cn/gtgltkovlx.html

[U14] Py：分组收集到列表
来源：http://hz.gotoacloud.top/gtcaweyrwx.html

defaultdict(list)
来源：http://hz.yvedp.cn/gtuslpwbhz.html

[U15] Py：高精度计时
来源：http://hz.guannengcc.top/gtcqmgezeq.html

t = time.perf_counter()
来源：http://hz.pengpengdd.cyou/gtzivjbqrs.html

[U16] Py：命令行参数解析
来源：http://hz.fengsongda.top/gtldnjpnxg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.cashguo.top/gtlnsdshqo.html

[U17] Py：初始化日志
来源：http://hz.guannengcc.top/gtzgswhqpb.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.bjfxy.top/gtutjljjdo.html

[U18] Py：预编译正则
来源：http://hz.tian-w.cn/gthvsjidze.html

pat = re.compile(r"\d+")
来源：http://hz.zhongyouzk.top/gtnmsndqbt.html

[U19] Py：正则替换带回调
来源：http://hz.jqgufenzy.top/gtskgvbzbk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.sxryk.cn/gtslldlqup.html

[U20] Py：缓存函数结果
来源：http://hz.havefunace.top/gtjhmeaiod.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhongyouzk.top/gtiksuqpzc.html

[U21] Py：自定义上下文管理器
来源：http://hz.jinghuilouyu.cn/gtxrmbulll.html

@contextlib.contextmanager
来源：http://hz.xuanzx.com/gtggtbuztg.html

[U22] Py：矩阵转置
来源：http://hz.cheryme.top/gtrofahwwx.html

list(zip(*m))
来源：http://hz.redwolf501.top/gtsuhwqudy.html

[U23] Py：分块读取大文件
来源：http://hz.daria6918.cn/gtjkkedtla.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.dianchejie.cn/gtkgjlviso.html

[U24] Py：路径操作
来源：http://hz.jinqigfzy.top/gtchslsdru.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.tianlin.xyz/gtpvxvlmzm.html

[U25] Py：CSV 按字典读
来源：http://hz.yj202588.top/gtxbabsoxr.html

csv.DictReader(f)
来源：http://hz.guannengcc.top/gtfakpgwko.html

[U26] Py：并发下载
来源：http://hz.gotoacloud.top/gthgbvntpj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.gotoacloud.top/gtborsurbd.html

[U27] Py：异步 HTTP
来源：http://hz.zhongyouzk.top/gtcabatzlj.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.vqdsnc.cn/gtcjhdaznr.html

[U28] Py：类型别名
来源：http://hz.kuanghao11.cn/gtqvrqgjco.html

UserId = int
来源：http://hz.pycfn.com/gtobkxxale.html

[U29] Py：属性校验
来源：http://hz.andypj.xyz/gtavknermw.html

@property 与 @x.setter 配合
来源：http://hz.andypj.xyz/gtodhjgida.html

[U30] Py：数据类
来源：http://hz.zycfv.cn/gtlfwexgzc.html

@dataclass(slots=True)
来源：http://hz.xuanzx.com/gtsvsfvklv.html

[U31] Py：单测
来源：http://hz.sweek.top/gtskcgeyrc.html

python -m pytest -q
来源：http://hz.chenjidiqi.icu/gtmxxqdgfy.html

[U32] Py：代码格式化
来源：http://hz.dianchejie.cn/gtmvswjnos.html

ruff format . && ruff check --fix .
来源：http://hz.hfpthk.cn/gtfeyxxxze.html

[U33] Py：打包发布
来源：http://hz.sxryk.cn/gtqkjyejcs.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.meibo888.top/gtdskxdnmu.html

[U34] Py：判断编码
来源：http://hz.dianchejie.cn/gtgvuxatab.html

chardet.detect(raw)
来源：http://hz.ydzc1.top/gtffpadbbh.html

[U35] Py：发送邮件
来源：http://hz.ppjwa.cn/gtfnotpbnq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.fengsongda.top/gtzislwkdz.html

[U36] Py：定时任务
来源：http://hz.sweek.top/gtkhuprkrl.html

schedule.every(10).minutes.do(job)
来源：http://hz.hnxiangtu.top/gtwetudjex.html

[U37] Py：读写 Excel
来源：http://hz.ppjwa.cn/gtaqjggrmc.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.ybcxt.top/gtkcvhhxvi.html

[U38] Py：获取脚本所在目录
来源：http://hz.smart0.xyz/gtraizdifi.html

Path(__file__).resolve().parent
来源：http://hz.chenlongwang.top/gtvxewfguz.html

[U39] Py：判断是否在交互环境
来源：http://hz.bjfxy.top/gtqganvymt.html

sys.stdout.isatty()
来源：http://hz.gaohongyu789.top/gtzkcwuiil.html

[U40] Py：打印到标准错误
来源：http://hz.ybcxt.top/gtyfeoasxz.html

print("err", file=sys.stderr)
来源：http://hz.haohaochexian.top/gtkesluugs.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.xinyue.icu/gtyvtrtdhg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.daria6918.cn/gtcdzfzyuw.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.svipenyu.cn/gthwrgyaeb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.pengpengdd.cyou/gtqsqikzgk.html

[U43] PHP：声明命名空间
来源：http://hz.ybcxt.top/gtjnzjirrk.html

namespace App\Http;
来源：http://hz.fengsongda.top/gtotaqpolz.html

[U44] PHP：开启严格类型
来源：http://hz.havefunace.top/gtbupwsulx.html

declare(strict_types=1);
来源：http://hz.xinyue.icu/gtusglqdok.html

[U45] PHP：类型声明与返回类型
来源：http://hz.xingfuxueyuan.xyz/gtwprkulqm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zdqjudy.top/gtptpybnwh.html

[U46] PHP：可空类型
来源：http://hz.zhiwuduotai.top/gtmeqfbcyh.html

?string $name = null
来源：http://hz.chenjidiqi.icu/gthohizkom.html

[U47] PHP：联合类型
来源：http://hz.yanxiufei.cn/gtuwfukdlq.html

int|string $id
来源：http://hz.tianlin.xyz/gtshnnvbzu.html

[U48] PHP：纯枚举
来源：http://hz.zycfv.cn/gtelfvqggw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.hysaishi.cn/gtfzakxnzk.html

[U49] PHP：只读属性
来源：http://hz.xziqi.cn/gtwuuyyikm.html

public readonly string $name
来源：http://hz.yongpay.top/gtpgknuyqk.html

[U50] PHP：构造器属性提升
来源：http://hz.svipenyu.cn/gtgpqcqoya.html

public function __construct(private int $id) {}
来源：http://hz.xuanzx.com/gtifmtwbkz.html

[U51] PHP：数组解构
来源：http://hz.yuxming.cn/gtkniwakkm.html

[$a, $b] = $arr;
来源：http://hz.nwbrower.top/gttnahicgd.html

[U52] PHP：箭头函数
来源：http://hz.nanxinkj.top/gtyfaxfmbp.html

$double = fn($x) => $x * 2;
来源：http://hz.0kj1m.cn/gtbgcfycop.html

[U53] PHP：空合并运算符
来源：http://hz.chenzaomai.com/gteucoosly.html

$v = $a ?? $b ?? "default";
来源：http://hz.gzhubu.top/gtygjwcmjj.html

[U54] PHP：空安全调用
来源：http://hz.ehwqpu.com/gthbqkuozp.html

$obj?->method()
来源：http://hz.shuidangran.top/gtaahmphnj.html

[U55] PHP：match 表达式
来源：http://hz.jlsjyb.cn/gtcppontfb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yvedp.cn/gttskjumop.html

[U56] PHP：命名参数
来源：http://hz.tanke756.top/gtezvmpdhc.html

f(a: 1, b: 2)
来源：http://hz.fengsongda.top/gtsxuhzgvj.html

[U57] PHP：字符串插值
来源：http://hz.guannengcc.top/gtnnqmoxsr.html

"值: {$a}"
来源：http://hz.wangshuangyany.cn/gtzqoaovet.html

[U58] PHP：数组三件套
来源：http://hz.fzhhl.top/gtubderbik.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.zhiwuduotai.top/gticawilsj.html

[U59] PHP：自定义排序
来源：http://hz.havefunace.top/gtnqmctzcl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.redwolf501.top/gtnwhhryeq.html

[U60] PHP：JSON 编解码
来源：http://hz.chenlongwang.top/gtiqhzjgmf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jqgufenzy.top/gtsuneuqek.html

[U61] PHP：正则
来源：http://hz.shanyushiyangtech.top/gtgqxamsec.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.gogol.net.cn/gtouwxxjya.html

[U62] PHP：日期对象
来源：http://hz.jiagoushi.top/gtfyjthgyr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.snrcjt.cn/gtwnqupjqu.html

[U63] PHP：文件读写
来源：http://hz.ppjwa.cn/gthdynditd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jqgfzy.top/gtteeoyepa.html

[U64] PHP：目录遍历
来源：http://hz.jinqigfzy.top/gtchyforot.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yonumen.top/gtgqztcpxy.html

[U65] PHP：会话
来源：http://hz.yuanzhike.top/gtdrjbaehj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.tian-w.cn/gtjemjfahe.html

[U66] PHP：设置 Cookie
来源：http://hz.xylfe.cn/gtoznswygw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.sysykeji.top/gtumwufiim.html

[U67] PHP：处理文件上传
来源：http://hz.cqqwz.cn/gtqnzmgouv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.aizwys.cn/gtctoxhbdm.html

[U68] PHP：PDO 连接
来源：http://hz.xinyue.icu/gtxpjbzrev.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.tanke756.top/gtxwyfzcup.html

[U69] PHP：PDO 预处理
来源：http://hz.c1oappe.top/gtkwroezej.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.dashuyun.cn/gtpgoycelx.html

[U70] PHP：PDO 事务
来源：http://hz.yanxiufei.cn/gtcpccpwbj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.9152youxi.cn/gtcvrklgjb.html

[U71] PHP：抛出异常
来源：http://hz.gogol.net.cn/gtxebntxik.html

throw new RuntimeException("失败", 500);
来源：http://hz.xingfuxueyuan.xyz/gtiuehkzmw.html

[U72] PHP：写错误日志
来源：http://hz.guowangkeji.top/gtxwaamuny.html

error_log("失败: " . $e->getMessage());
来源：http://hz.shangyingyoupin.top/gtghskpkbf.html

[U73] PHP：读取 ini 配置
来源：http://hz.zhaomingkeji.xyz/gtvjislvva.html

parse_ini_file("config.ini", true)
来源：http://hz.zhoulong.xyz/gtprjkxjmt.html

[U74] PHP：读取环境变量
来源：http://hz.jiagoushi.top/gtjiuxlsjg.html

getenv("APP_ENV") ?: "production"
来源：http://hz.wangdashe.top/gtihzqhppe.html

[U75] PHP：依赖注入
来源：http://hz.ivvv.top/gtbkwzpmyl.html

composer require psr/container
来源：http://hz.yuxming.cn/gtjevszmwb.html

[U76] PHP：简单路由
来源：http://hz.jianghu66.top/gtefojaook.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.aizwys.cn/gtncavmoyn.html

[U77] PHP：模板渲染
来源：http://hz.havefunace.top/gtkzavvgjy.html

composer require twig/twig
来源：http://hz.ydjk.org.cn/gtmszznveh.html

[U78] PHP：单元测试
来源：http://hz.quarkkingdee.top/gtqymvsvhw.html

composer require --dev phpunit/phpunit
来源：http://hz.52xcode.cn/gtkxdqqzyf.html

[U79] PHP：静态分析
来源：http://hz.shanyushiyangtech.top/gtzwueoepw.html

composer require --dev phpstan/phpstan
来源：http://hz.shangyingyoupin.top/gtsztpmpwb.html

[U80] PHP：代码规范修复
来源：http://hz.ehwqpu.com/gtkocrnayu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.316326.xyz/gtbnbdowmu.html

[U81] JS：初始化项目
来源：http://hz.snrcjt.cn/gtvmfvstbx.html

npm init -y;  npm i express
来源：http://hz.jiagoushi.top/gtomfzcsof.html

[U82] JS：package.json 脚本
来源：http://hz.guowangkeji.top/gtpnhqjdkg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.aibaodan.cn/gtcsbwneni.html

[U83] JS：ES Module 导入导出
来源：http://hz.redwolf501.top/gtaknjnlcc.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.c1oappe.top/gtkzfpwxog.html

[U84] JS：CommonJS 写法
来源：http://hz.svipenyu.cn/gtxbloczfv.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.hnqzz.top/gtfkoztxfd.html

[U85] JS：可选链
来源：http://hz.yuanzhike.top/gtiovfxfqg.html

a?.b?.c
来源：http://hz.pengpengdd.cyou/gtxttimeuz.html

[U86] JS：空值合并
来源：http://hz.xylfe.cn/gtaahnjdjs.html

a ?? b
来源：http://hz.iojbl.cn/gtwaqfkvas.html

[U87] JS：解构默认值
来源：http://hz.xinyue.icu/gtcssmcmpk.html

const { a = 1, b = 2 } = obj;
来源：http://hz.nanxinkj.top/gtkyezbgyl.html

[U88] JS：对象展开合并
来源：http://hz.hammf.cn/gtjtwnommi.html

{ ...a, ...b }
来源：http://hz.havefunace.top/gtllxofofh.html

[U89] JS：数组去重
来源：http://hz.aizwys.cn/gtzxusjblh.html

[...new Set(arr)]
来源：http://hz.feifeiyinyue.top/gtgkpqwins.html

[U90] JS：数字数组排序
来源：http://hz.ydzc1.top/gtydsprfvz.html

[...arr].sort((a, b) => a - b)
来源：http://hz.guowangkeji.top/gtlticbhjh.html

[U91] JS：对象键值遍历
来源：http://hz.xinyue.icu/gtxjrgdovp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.zhoulong.xyz/gtihyqfjji.html

[U92] JS：深拷贝
来源：http://hz.cdnleiting.top/gtvhpiusln.html

structuredClone(obj)
来源：http://hz.cheryme.top/gtzpjfutsz.html

[U93] JS：模板字符串
来源：http://hz.xinyue.icu/gtctbpimdk.html

`共 ${n} 条`
来源：http://hz.bjfxy.top/gtvtuncpgu.html

[U94] JS：箭头函数
来源：http://hz.cdnleiting.top/gtwjcczgfc.html

const double = x => x * 2;
来源：http://hz.ybcxt.top/gtxvafilzi.html

[U95] JS：Promise 包装
来源：http://hz.jqgfzy.top/gtkczcuwca.html

new Promise((resolve, reject) => {})
来源：http://hz.zhiwuduotai.top/gtfrfrvrpx.html

[U96] JS：async/await 与异常
来源：http://hz.hfpthk.cn/gtydcaligy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.feifeiyinyue.top/gtkgtnjlwj.html

[U97] JS：并发请求
来源：http://hz.xziqi.cn/gttkxzfuep.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.smart0.xyz/gtwrjivjbk.html

[U98] JS：fetch 带 JSON
来源：http://hz.tanke756.top/gthfzabzdi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.hammf.cn/gtnwitwxxd.html

[U99] JS：事件监听
来源：http://hz.feifeiyinyue.top/gtntesrbuv.html

el.addEventListener("click", e => {})
来源：http://hz.zhongyouzk.top/gtblttatwe.html

[U100] JS：DOM 查询
来源：http://hz.zhengqikj.top/gtlnebheug.html

document.querySelector(".item")
来源：http://hz.ydzc1.top/gtaxyrdxew.html

[U101] JS：classList 操作
来源：http://hz.pengpengdd.cyou/gtvgkzehtl.html

el.classList.toggle("active")
来源：http://hz.guowangkeji.top/gtolqkvfnv.html

[U102] JS：本地存储
来源：http://hz.ivvv.top/gtzteexnwh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jyoumei.cn/gtyvdwqpla.html

[U103] JS：定时器
来源：http://hz.mhx1999.top/gtzpmlcdsm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.ehwqpu.com/gtmvdvplqv.html

[U104] JS：防抖
来源：http://hz.tianlin.xyz/gtriakqcnb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nwbrower.top/gttonalqru.html

[U105] JS：节流
来源：http://hz.hnqzz.top/gtuygznawc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.meibo888.top/gtywichumo.html

[U106] JS：日期格式化
来源：http://hz.aizwys.cn/gtsefdjxwi.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.haohaochexian.top/gtaodjbyfl.html

[U107] JS：数字千分位
来源：http://hz.xuetiantiany.cn/gtnjmfllkw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.cashguo.top/gtkrngsdld.html

[U108] JS：随机整数
来源：http://hz.dianchejie.cn/gtipktymcr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yuanzhike.top/gtofpwdwge.html

[U109] JS：数组分组
来源：http://hz.dashuyun.cn/gtsdmgzjhy.html

Object.groupBy(arr, x => x.type)
来源：http://hz.havefunace.top/gtlvegideg.html

[U110] JS：数组分块
来源：http://hz.daxiang520.top/gtcwivsaep.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.tian-w.cn/gtcvvmhlop.html

[U111] JS：对象转 Map
来源：http://hz.jqgufenzy.top/gtqiqywkkg.html

new Map(Object.entries(obj))
来源：http://hz.meibo888.top/gtitdwyccv.html

[U112] JS：字符串补位
来源：http://hz.gaohongyu789.top/gtpureagpx.html

"7".padStart(3, "0")
来源：http://hz.sufxvd.cn/gtxmonqyqm.html

[U113] JS：正则替换全部
来源：http://hz.zdqjudy.top/gtinkxppka.html

s.replaceAll("a", "b")
来源：http://hz.jyoumei.cn/gtssvdvooy.html

[U114] JS：JSON 深比较
来源：http://hz.bjfxy.top/gtnvxkiamf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cqqwz.cn/gtprnizyrr.html

[U115] JS：生成 UUID
来源：http://hz.316326.xyz/gtzpyqjwea.html

crypto.randomUUID()
来源：http://hz.daria6918.cn/gtqroehymo.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.fzhhl.top/gtyuhbeoyz.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yuxming.cn/gtkupeeptd.html

[U117] JS：单元测试
来源：http://hz.yuxming.cn/gtfnnktcwg.html

npm i -D vitest;  npx vitest
来源：http://hz.yj202588.top/gtjgnuixrp.html

[U118] JS：开发服务器
来源：http://hz.dashuyun.cn/gtqzcdhpal.html

npm i -D vite;  npx vite
来源：http://hz.jianghu66.top/gtlialcpik.html

[U119] JS：生产构建
来源：http://hz.ybcxt.top/gtjoujnizt.html

npx vite build
来源：http://hz.jiagoushi.top/gtefqivldc.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.xingfuxueyuan.xyz/gtbdtxcyfv.html

import.meta.env.VITE_API_URL
来源：http://hz.yj202588.top/gtztlopjpv.html

================================================================================
来源：http://hz.sxryk.cn/gtxggjrvzk.html

统计汇总
来源：http://hz.xingfuxueyuan.xyz/gtmfmhkajk.html

================================================================================
来源：http://hz.mhx1999.top/gtefyrwyhs.html

按语言统计（条）：
来源：http://hz.jqgufenzy.top/gtgyvewdbc.html

Python ......... 252
来源：http://hz.yangfankeji.com/gtrmiajauc.html

PHP ............ 252
来源：http://hz.yj20258888.top/gtwnzuxlrl.html

JavaScript ..... 252
来源：http://hz.yvedp.cn/gtrhqqfkmk.html

TypeScript ..... 212
来源：http://hz.gotoacloud.top/gtmzdxeaum.html

Java ........... 212
来源：http://hz.ywan-chungtsiang.top/gtxvljxdte.html

Go ............. 212
来源：http://hz.yueranfly.top/gtvhuxtalm.html

Ruby ........... 212
来源：http://hz.hnqzz.top/gtcewqmism.html

C# ............. 212
来源：http://hz.ehwqpu.com/gtlnobgdre.html

C .............. 30
来源：http://hz.zhengqikj.top/gtpgesuuin.html

C++ ............ 30
来源：http://hz.smart0.xyz/gtfyqihmlf.html

SQL ............ 90
来源：http://hz.yj202588.top/gtkdvaydrx.html

Bash ........... 80
来源：http://hz.guowangkeji.top/gtqiqpleft.html

Kotlin ......... 15
来源：http://hz.nanxuanxn.top/gtzivympna.html

Swift .......... 15
来源：http://hz.kuanghao11.cn/gtslvjkokl.html

Lua ............ 10
来源：http://hz.ehwqpu.com/gtikboqhum.html

Perl ........... 10
来源：http://hz.quarkkingdee.top/gtdotoehck.html

Scala .......... 10
来源：http://hz.feifeiyinyue.top/gtzgdlpiky.html

------------------------------------
来源：http://hz.ybcxt.top/gthmkzftri.html

合计 ........... 2106 条
来源：http://hz.yuanzhike.top/gtbutvlyab.html

按章节统计：
来源：http://hz.shuidangran.top/gteeesclxz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.xylfe.cn/gtexxuwmvu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.haohaochexian.top/gtdxwbdrkq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.ehwqpu.com/gtasmactzk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.ybcxt.top/gtsyixxeaw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.xuanzx.com/gtllgangsl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.birdmap.top/gtxmjcigsh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.cashguo.top/gtdjnzassj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.meibo888.top/gttnckeabm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.aibaodan.cn/gtackeozye.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.haohaochexian.top/gtlluthlew.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.andypj.xyz/gtbeorvhst.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zhongyouzk.top/gtujxlqmsj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.yuanzhike.top/gtrapgreee.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.hywenlv.cn/gtxrvaqncs.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.tanke756.top/gtivruosav.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.hysaishi.cn/gtmuxsqdag.html

Q SQL 专题                              90
来源：http://hz.kuanghao11.cn/gterlvxsin.html

R Bash 专题                             80
来源：http://hz.xylfe.cn/gtqjqdueko.html

S C / C++ 专题                          60
来源：http://hz.yuanzhike.top/gtlltvnuhm.html

T 其他语言补充                          60
来源：http://hz.yuxming.cn/gtbqtplcnv.html

U 高频实用片段                         120
来源：http://hz.cashguo.top/gtphydcgwx.html

------------------------------------
来源：http://hz.zhiwuduotai.top/gtiarznmau.html

合计                                  2106 条
来源：http://hz.sweek.top/gtmhlfoflg.html

--------------------------------------------------------------------------------
来源：http://hz.chenzaomai.com/gtqnwbtggk.html

使用提醒
来源：http://hz.hnxiangtu.top/gtxlgjmthy.html

--------------------------------------------------------------------------------
来源：http://hz.yuxming.cn/gtycptnqzg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.vqdsnc.cn/gtsrpmqegs.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.hysaishi.cn/gthbbcghjw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.zhengqikj.top/gtayeopois.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.jqgfzy.top/gtxhwuwxtw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.gzhubu.top/gtovazwixi.html

—— 文件结束 ——
来源：http://hz.zhoulong.xyz/gtyopwjwpc.html

================================================================================
来源：http://hz.guowangkeji.top/gtbaxbypcr.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.nwbrower.top/gtdagqnejp.html

Common Programming Examples Cheat Book
来源：http://hz.jiagoushi.top/gthhxtphzy.html

================================================================================
来源：http://hz.hywenlv.cn/gtiwhospxs.html

【收录内容】
来源：http://hz.smart0.xyz/gtdcqabiis.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.zhengqikj.top/gtfvbynnvj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.ywan-chungtsiang.top/gtdhhfhycl.html

SQL · Bash · C · C++
来源：http://hz.yuanzhike.top/gtlfxgrxwd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.c1oappe.top/gtxkwprbvj.html

【使用说明】
来源：http://hz.hysaishi.cn/gtndvzqxue.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.yuanzhike.top/gtlxlftkcj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.zycfv.cn/gtfuskdtyr.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.zhongyouzk.top/gtziyrwfro.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.yj20258888.top/gtgsqgvakq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.xingfuxueyuan.xyz/gtcvhxdgri.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.sysykeji.top/gtrntrolia.html


<!-- 参考信息 -->