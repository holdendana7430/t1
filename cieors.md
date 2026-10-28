代发 wailian999

[U11] Py：生成器表达式
来源：http://hz.cashguo.top/gtvtfjuxrv.html

(x * 2 for x in arr)
来源：http://hz.shzxlz.cn/gthmumqyqq.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yuxming.cn/gtbnmrccgz.html

Counter(arr).most_common(3)
来源：http://hz.jiagoushi.top/gtpojiyfrn.html

[U13] Py：固定长度队列
来源：http://hz.shangyingyoupin.top/gtqeidxcng.html

deque(maxlen=10)
来源：http://hz.yj20258.top/gtelkuzolc.html

[U14] Py：分组收集到列表
来源：http://hz.jyoumei.cn/gtlsznvhdf.html

defaultdict(list)
来源：http://hz.jinghuilouyu.cn/gtyzrytezc.html

[U15] Py：高精度计时
来源：http://hz.hywenlv.cn/gtlkirgogv.html

t = time.perf_counter()
来源：http://hz.yj20258888.top/gtbljhtpmy.html

[U16] Py：命令行参数解析
来源：http://hz.ppjwa.cn/gtpdejwekv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.xziqi.cn/gtvuaaujhw.html

[U17] Py：初始化日志
来源：http://hz.chenjidiqi.icu/gtsyyrqddm.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.sxryk.cn/gtauhzqfjj.html

[U18] Py：预编译正则
来源：http://hz.daria6918.cn/gtugwbmctr.html

pat = re.compile(r"\d+")
来源：http://hz.hnxiangtu.top/gthuyppsat.html

[U19] Py：正则替换带回调
来源：http://hz.wangshuangyany.cn/gtjtxktors.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.aizwys.cn/gtrhaelelr.html

[U20] Py：缓存函数结果
来源：http://hz.zdqjudy.top/gteyhqrtnb.html

@functools.lru_cache(maxsize=None)
来源：http://hz.fzhhl.top/gtxitnqbei.html

[U21] Py：自定义上下文管理器
来源：http://hz.kuanghao11.cn/gtfiycbfsu.html

@contextlib.contextmanager
来源：http://hz.yueranfly.top/gteaegvblt.html

[U22] Py：矩阵转置
来源：http://hz.dianchejie.cn/gtmqjqhotk.html

list(zip(*m))
来源：http://hz.haohaochexian.top/gtbazudpqa.html

[U23] Py：分块读取大文件
来源：http://hz.fengsongda.top/gtgduerbpr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yanxiufei.cn/gtxpmlvuat.html

[U24] Py：路径操作
来源：http://hz.hywenlv.cn/gtyciyvbqs.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.chenlongwang.top/gtoyqtqcjk.html

[U25] Py：CSV 按字典读
来源：http://hz.sysykeji.top/gtlluftamn.html

csv.DictReader(f)
来源：http://hz.zhongyouzk.top/gtuyqooveq.html

[U26] Py：并发下载
来源：http://hz.mhx1999.top/gtneiggixd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.ivvv.top/gtdljzwilv.html

[U27] Py：异步 HTTP
来源：http://hz.ehwqpu.com/gtjebzqhcb.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.yuanzhike.top/gtrzilcdwd.html

[U28] Py：类型别名
来源：http://hz.316326.xyz/gtbdeundxc.html

UserId = int
来源：http://hz.xuanzx.com/gteoaoeken.html

[U29] Py：属性校验
来源：http://hz.kuanghao11.cn/gtnsqrdako.html

@property 与 @x.setter 配合
来源：http://hz.316326.xyz/gtxjhaqgxr.html

[U30] Py：数据类
来源：http://hz.gzhubu.top/gtgltrclaw.html

@dataclass(slots=True)
来源：http://hz.gaohongyu789.top/gtzhfvwpul.html

[U31] Py：单测
来源：http://hz.c1oappe.top/gtmoeenycw.html

python -m pytest -q
来源：http://hz.gogol.net.cn/gtvabvsrtw.html

[U32] Py：代码格式化
来源：http://hz.zhiwuduotai.top/gtoiuszhbi.html

ruff format . && ruff check --fix .
来源：http://hz.andypj.xyz/gtdugnhqcc.html

[U33] Py：打包发布
来源：http://hz.aizwys.cn/gtbuoyytct.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.9152youxi.cn/gtyxsbinvv.html

[U34] Py：判断编码
来源：http://hz.0kj1m.cn/gtkrqmeujb.html

chardet.detect(raw)
来源：http://hz.ywan-chungtsiang.top/gtctcqeccc.html

[U35] Py：发送邮件
来源：http://hz.zhixingplan.top/gtwgbaatbj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.hnxiangtu.top/gtokbtjkan.html

[U36] Py：定时任务
来源：http://hz.meibo888.top/gtsoebdntl.html

schedule.every(10).minutes.do(job)
来源：http://hz.cqqwz.cn/gtdngtftpr.html

[U37] Py：读写 Excel
来源：http://hz.fzhhl.top/gtlfcyknia.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.jinqigfzy.top/gtjbtvxzsg.html

[U38] Py：获取脚本所在目录
来源：http://hz.zhoulong.xyz/gtbqvptpli.html

Path(__file__).resolve().parent
来源：http://hz.jinyuanbaomall.cn/gtrjphqbgn.html

[U39] Py：判断是否在交互环境
来源：http://hz.jianghu66.top/gtgfjmqmcg.html

sys.stdout.isatty()
来源：http://hz.jqgfzy.top/gtmhweaiwc.html

[U40] Py：打印到标准错误
来源：http://hz.shuidangran.top/gtmpodsokw.html

print("err", file=sys.stderr)
来源：http://hz.jiagoushi.top/gtdpcklpjt.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.cdnleiting.top/gtznulpwbw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.yvedp.cn/gtnemlftmv.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.birdmap.top/gtebbbzhiy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.0kj1m.cn/gtlkylftzk.html

[U43] PHP：声明命名空间
来源：http://hz.gaohongyu789.top/gtihlwdybq.html

namespace App\Http;
来源：http://hz.cdnleiting.top/gtuthdomfv.html

[U44] PHP：开启严格类型
来源：http://hz.andypj.xyz/gtabzfbcyv.html

declare(strict_types=1);
来源：http://hz.gzhubu.top/gtgaydaozh.html

[U45] PHP：类型声明与返回类型
来源：http://hz.cashguo.top/gtdaewwqvl.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ydjk.org.cn/gtcrwqgyoz.html

[U46] PHP：可空类型
来源：http://hz.guannengcc.top/gtyvoipgyx.html

?string $name = null
来源：http://hz.sufxvd.cn/gtfiylwvfb.html

[U47] PHP：联合类型
来源：http://hz.jqgufenzy.top/gtplfaadrq.html

int|string $id
来源：http://hz.ywan-chungtsiang.top/gtphuhjtfw.html

[U48] PHP：纯枚举
来源：http://hz.chenjidiqi.icu/gtovmexozn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.hfpthk.cn/gtwedlwcmz.html

[U49] PHP：只读属性
来源：http://hz.cheryme.top/gtqarjjmjg.html

public readonly string $name
来源：http://hz.birdmap.top/gtazpocsny.html

[U50] PHP：构造器属性提升
来源：http://hz.yj20258.top/gtvkezwryy.html

public function __construct(private int $id) {}
来源：http://hz.mhx1999.top/gthcsfbuwk.html

[U51] PHP：数组解构
来源：http://hz.yuanzhike.top/gtrlfblggg.html

[$a, $b] = $arr;
来源：http://hz.ppjwa.cn/gtfeggkwxe.html

[U52] PHP：箭头函数
来源：http://hz.guannengcc.top/gtsypuetdu.html

$double = fn($x) => $x * 2;
来源：http://hz.yonumen.top/gtqulrxymi.html

[U53] PHP：空合并运算符
来源：http://hz.yvedp.cn/gtqwgnbaym.html

$v = $a ?? $b ?? "default";
来源：http://hz.ybcxt.top/gtkofujwaj.html

[U54] PHP：空安全调用
来源：http://hz.zhoulong.xyz/gtyexxbroh.html

$obj?->method()
来源：http://hz.jinghuilouyu.cn/gthxkcbmtg.html

[U55] PHP：match 表达式
来源：http://hz.gzhubu.top/gtqqehjywh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.haohaochexian.top/gtpscjymkz.html

[U56] PHP：命名参数
来源：http://hz.hammf.cn/gtgvllhwiw.html

f(a: 1, b: 2)
来源：http://hz.yuanzhike.top/gtvbfoctll.html

[U57] PHP：字符串插值
来源：http://hz.yj20258888.top/gtspezrdsq.html

"值: {$a}"
来源：http://hz.zhixingplan.top/gtdqnlowat.html

[U58] PHP：数组三件套
来源：http://hz.sweek.top/gtzytrfbgz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.xinyue.icu/gtzxwhkcnw.html

[U59] PHP：自定义排序
来源：http://hz.shzxlz.cn/gtethfuuof.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jlsjyb.cn/gtaxlrvwyl.html

[U60] PHP：JSON 编解码
来源：http://hz.hongshengwenyu.top/gtcprlckhx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.hnxiangtu.top/gtbetdhhsr.html

[U61] PHP：正则
来源：http://hz.jqgfzy.top/gteybhztpk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.chenzaomai.com/gtuvbnusci.html

[U62] PHP：日期对象
来源：http://hz.hywenlv.cn/gtoritlrxu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.zdqjudy.top/gtcyetgeze.html

[U63] PHP：文件读写
来源：http://hz.quarkkingdee.top/gtwdgwslxj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.feifeiyinyue.top/gtqhognupf.html

[U64] PHP：目录遍历
来源：http://hz.pycfn.com/gtgwiwzuih.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.ppjwa.cn/gtbmytkhum.html

[U65] PHP：会话
来源：http://hz.ydzc1.top/gtholmjvey.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.yj20258.top/gtrinejqeg.html

[U66] PHP：设置 Cookie
来源：http://hz.jlsjyb.cn/gtweiranvj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.gogol.net.cn/gtztbzvcis.html

[U67] PHP：处理文件上传
来源：http://hz.ydjk.org.cn/gtcowcndle.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.jinqigfzy.top/gtumuehgtq.html

[U68] PHP：PDO 连接
来源：http://hz.shzxlz.cn/gtkgzamsjy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.wangshuangyany.cn/gtcwihdhky.html

[U69] PHP：PDO 预处理
来源：http://hz.pengpengdd.cyou/gtnccwowgs.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.316326.xyz/gtbeijjpdi.html

[U70] PHP：PDO 事务
来源：http://hz.hywenlv.cn/gtszjpngdz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.yuxming.cn/gtddurrmmq.html

[U71] PHP：抛出异常
来源：http://hz.nwbrower.top/gtgrswhfjl.html

throw new RuntimeException("失败", 500);
来源：http://hz.cucudq.cn/gtvkkgybrg.html

[U72] PHP：写错误日志
来源：http://hz.xingfuxueyuan.xyz/gtdlpccujh.html

error_log("失败: " . $e->getMessage());
来源：http://hz.jlsjyb.cn/gthmfqnjhf.html

[U73] PHP：读取 ini 配置
来源：http://hz.redwolf501.top/gtjbbfneir.html

parse_ini_file("config.ini", true)
来源：http://hz.kuanghao11.cn/gtzxagialj.html

[U74] PHP：读取环境变量
来源：http://hz.yueranfly.top/gtypnfcjpg.html

getenv("APP_ENV") ?: "production"
来源：http://hz.iojbl.cn/gtynejbtpx.html

[U75] PHP：依赖注入
来源：http://hz.xingfuxueyuan.xyz/gtudadtrhn.html

composer require psr/container
来源：http://hz.jinghuilouyu.cn/gtlhjnqwtg.html

[U76] PHP：简单路由
来源：http://hz.xuetiantiany.cn/gtltagxxwk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.aibaodan.cn/gtdfraboqf.html

[U77] PHP：模板渲染
来源：http://hz.wangdashe.top/gtnyrqmrnb.html

composer require twig/twig
来源：http://hz.xingfuxueyuan.xyz/gtbwsxslva.html

[U78] PHP：单元测试
来源：http://hz.zhengqikj.top/gtfyllubhc.html

composer require --dev phpunit/phpunit
来源：http://hz.aizwys.cn/gtmpxmfmpx.html

[U79] PHP：静态分析
来源：http://hz.jinyuanbaomall.cn/gtezsmvnqm.html

composer require --dev phpstan/phpstan
来源：http://hz.daxiang520.top/gtgjuilmkf.html

[U80] PHP：代码规范修复
来源：http://hz.aibaodan.cn/gtfcouwidz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.ehwqpu.com/gtzhnwthzg.html

[U81] JS：初始化项目
来源：http://hz.zdqjudy.top/gtqrtwifby.html

npm init -y;  npm i express
来源：http://hz.haohaochexian.top/gtwujvmqxm.html

[U82] JS：package.json 脚本
来源：http://hz.aibaodan.cn/gtpjugdgas.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.cucudq.cn/gtbqkzwtcz.html

[U83] JS：ES Module 导入导出
来源：http://hz.xingfuxueyuan.xyz/gtynjyidhi.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.xylfe.cn/gtbbvtvnzi.html

[U84] JS：CommonJS 写法
来源：http://hz.daria6918.cn/gtbhrqfagp.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.316326.xyz/gtgoutihsh.html

[U85] JS：可选链
来源：http://hz.hnxiangtu.top/gtgsmrrrik.html

a?.b?.c
来源：http://hz.sysykeji.top/gtrgxgteoi.html

[U86] JS：空值合并
来源：http://hz.chenzaomai.com/gtcdkyhjgu.html

a ?? b
来源：http://hz.cashguo.top/gtrewrnscd.html

[U87] JS：解构默认值
来源：http://hz.tianlin.xyz/gtuwiitzqk.html

const { a = 1, b = 2 } = obj;
来源：http://hz.sxryk.cn/gtpibohdcx.html

[U88] JS：对象展开合并
来源：http://hz.redwolf501.top/gtlvcerxsj.html

{ ...a, ...b }
来源：http://hz.jianghu66.top/gtxodywvdi.html

[U89] JS：数组去重
来源：http://hz.smart0.xyz/gtlmjghxbi.html

[...new Set(arr)]
来源：http://hz.hongshengwenyu.top/gtfjvelusd.html

[U90] JS：数字数组排序
来源：http://hz.cqqwz.cn/gtccltbzwp.html

[...arr].sort((a, b) => a - b)
来源：http://hz.yuanzhike.top/gthssmitkp.html

[U91] JS：对象键值遍历
来源：http://hz.yj20258888.top/gtudqdqlhy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.zdqjudy.top/gtuwmmdkvb.html

[U92] JS：深拷贝
来源：http://hz.yuanzhike.top/gtfkdizrxk.html

structuredClone(obj)
来源：http://hz.jiagoushi.top/gtnvapvbaz.html

[U93] JS：模板字符串
来源：http://hz.kuanghao11.cn/gtdljddmeg.html

`共 ${n} 条`
来源：http://hz.cheryme.top/gtrzzypvjg.html

[U94] JS：箭头函数
来源：http://hz.kuanghao11.cn/gtgqnairjw.html

const double = x => x * 2;
来源：http://hz.haohaochexian.top/gtyprtnntt.html

[U95] JS：Promise 包装
来源：http://hz.guannengcc.top/gtextrotfx.html

new Promise((resolve, reject) => {})
来源：http://hz.xinyue.icu/gthgvodxrr.html

[U96] JS：async/await 与异常
来源：http://hz.gogol.net.cn/gtszkbjtpe.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yj202588.top/gtexbfihzx.html

[U97] JS：并发请求
来源：http://hz.xingfuxueyuan.xyz/gtbywbvrwt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenlongwang.top/gtoseffzwf.html

[U98] JS：fetch 带 JSON
来源：http://hz.yj20258888.top/gtklsuxsgb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.hysaishi.cn/gtatxvkuxb.html

[U99] JS：事件监听
来源：http://hz.smart0.xyz/gtvtjtfpio.html

el.addEventListener("click", e => {})
来源：http://hz.chenzaomai.com/gtxjvoabnm.html

[U100] JS：DOM 查询
来源：http://hz.jinghuilouyu.cn/gtbrytgwuo.html

document.querySelector(".item")
来源：http://hz.sysykeji.top/gthefbltdf.html

[U101] JS：classList 操作
来源：http://hz.daxiang520.top/gtinbwdrvn.html

el.classList.toggle("active")
来源：http://hz.havefunace.top/gtbsqebzfy.html

[U102] JS：本地存储
来源：http://hz.shanyushiyangkeji.top/gtvrtchaka.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jinyuanbaomall.cn/gtsizcljnj.html

[U103] JS：定时器
来源：http://hz.jianghu66.top/gtpdvojjus.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.guowangkeji.top/gtytldftqz.html

[U104] JS：防抖
来源：http://hz.cheryme.top/gtfhpdnasx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj20258.top/gtiekfvvrs.html

[U105] JS：节流
来源：http://hz.nwbrower.top/gtpwzlrbzr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.hysaishi.cn/gtvrwusgfl.html

[U106] JS：日期格式化
来源：http://hz.yj202588.top/gtxcpjmofs.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.nanxinkj.top/gtklunbabq.html

[U107] JS：数字千分位
来源：http://hz.xuanzx.com/gtedqzrjjf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.ivvv.top/gtaotpkwhu.html

[U108] JS：随机整数
来源：http://hz.jinghuilouyu.cn/gtbsvokzxx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.aizwys.cn/gtagnyrkdl.html

[U109] JS：数组分组
来源：http://hz.chenlongwang.top/gtwadezzmu.html

Object.groupBy(arr, x => x.type)
来源：http://hz.cashguo.top/gtbmkfiufp.html

[U110] JS：数组分块
来源：http://hz.hywenlv.cn/gtufydndwo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yanxiufei.cn/gtqcqorpnl.html

[U111] JS：对象转 Map
来源：http://hz.yuanzhike.top/gtibyugwur.html

new Map(Object.entries(obj))
来源：http://hz.hnxiangtu.top/gtdebrrexu.html

[U112] JS：字符串补位
来源：http://hz.ydjk.org.cn/gtplloegmg.html

"7".padStart(3, "0")
来源：http://hz.shanyushiyangkeji.top/gtovgvmxvj.html

[U113] JS：正则替换全部
来源：http://hz.zycfv.cn/gtxczowshl.html

s.replaceAll("a", "b")
来源：http://hz.sweek.top/gtfbcsihdh.html

[U114] JS：JSON 深比较
来源：http://hz.meibo888.top/gthnkpftdf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ywan-chungtsiang.top/gtnlebxrrv.html

[U115] JS：生成 UUID
来源：http://hz.hnxiangtu.top/gtbkgwpmvp.html

crypto.randomUUID()
来源：http://hz.52xcode.cn/gthnhzvqhr.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.dianchejie.cn/gtngwbbxri.html

/** @param {string} name */ function f(name) {}
来源：http://hz.zhengqikj.top/gtfuzkyeny.html

[U117] JS：单元测试
来源：http://hz.quarkkingdee.top/gtarxpfqss.html

npm i -D vitest;  npx vitest
来源：http://hz.sysykeji.top/gtkjxstqrw.html

[U118] JS：开发服务器
来源：http://hz.birdmap.top/gtnbbrpiyc.html

npm i -D vite;  npx vite
来源：http://hz.chenzaomai.com/gtzdsbbpng.html

[U119] JS：生产构建
来源：http://hz.feifeiyinyue.top/gtimckykbh.html

npx vite build
来源：http://hz.zhongyouzk.top/gtalcmfwxy.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.bjfxy.top/gtzxcdfaoq.html

import.meta.env.VITE_API_URL
来源：http://hz.xuanzx.com/gtffitnipa.html

================================================================================
来源：http://hz.hfpthk.cn/gtxcvodxwg.html

统计汇总
来源：http://hz.jqgfzy.top/gtorecwgwe.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtfidlxqec.html

按语言统计（条）：
来源：http://hz.feifeiyinyue.top/gtwejzbseo.html

Python ......... 252
来源：http://hz.zhoulong.xyz/gtsthobtdk.html

PHP ............ 252
来源：http://hz.smart0.xyz/gtoyubnljd.html

JavaScript ..... 252
来源：http://hz.yueranfly.top/gtybozwjgl.html

TypeScript ..... 212
来源：http://hz.ydjk.org.cn/gtfecpbzqu.html

Java ........... 212
来源：http://hz.cheryme.top/gtewnvqkpj.html

Go ............. 212
来源：http://hz.zycfv.cn/gtuottahtm.html

Ruby ........... 212
来源：http://hz.birdmap.top/gtatzgxwnq.html

C# ............. 212
来源：http://hz.hnqzz.top/gtxmahbmcz.html

C .............. 30
来源：http://hz.pengpengdd.cyou/gtimqoqffm.html

C++ ............ 30
来源：http://hz.sufxvd.cn/gtclwhqghf.html

SQL ............ 90
来源：http://hz.gzhubu.top/gtadtdamif.html

Bash ........... 80
来源：http://hz.snrcjt.cn/gtwseikkwh.html

Kotlin ......... 15
来源：http://hz.nanxuanxn.top/gtxwiglndt.html

Swift .......... 15
来源：http://hz.shangyingyoupin.top/gtrsumkmvi.html

Lua ............ 10
来源：http://hz.chenzaomai.com/gthbgevoav.html

Perl ........... 10
来源：http://hz.shanyushiyangkeji.top/gtrisodqtj.html

Scala .......... 10
来源：http://hz.cdnleiting.top/gtnzaeavls.html

------------------------------------
来源：http://hz.zdqjudy.top/gtmwdzkvxx.html

合计 ........... 2106 条
来源：http://hz.shanyushiyangtech.top/gtqwivsgvc.html

按章节统计：
来源：http://hz.feifeiyinyue.top/gtfijirrtc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.guowangkeji.top/gtvgqdhlpl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.xylfe.cn/gtkbeqivoa.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zhijiandao.cn/gtvlbicakr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.jinqigufen.top/gtmmtakvyw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zhiwuduotai.top/gtalwucvtl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.xingfuxueyuan.xyz/gtsggvebwj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.ivvv.top/gtceqmtsug.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.shangyingyoupin.top/gtzjqlllav.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.sysykeji.top/gtynddpsbd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.tanke756.top/gtvdxsvgks.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.ppjwa.cn/gtutaxbuic.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.xuanzx.com/gtsicjlvxq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zhiwuduotai.top/gtypwguzdn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jianghu66.top/gtfaklmxfw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.zycfv.cn/gtvvkstbog.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.sysykeji.top/gtbxkacrzi.html

Q SQL 专题                              90
来源：http://hz.nanxinkj.top/gtxzgynjdg.html

R Bash 专题                             80
来源：http://hz.sxryk.cn/gtoofnsqjq.html

S C / C++ 专题                          60
来源：http://hz.ydzc1.top/gtytkjdrcp.html

T 其他语言补充                          60
来源：http://hz.c1oappe.top/gtzxbxvkpb.html

U 高频实用片段                         120
来源：http://hz.hfpthk.cn/gtqidjjcdf.html

------------------------------------
来源：http://hz.yanxiufei.cn/gtjqckyljg.html

合计                                  2106 条
来源：http://hz.jqgfzy.top/gthzkdazwu.html

--------------------------------------------------------------------------------
来源：http://hz.feifeiyinyue.top/gtqiwflvjb.html

使用提醒
来源：http://hz.gogol.net.cn/gtsnbnawuh.html

--------------------------------------------------------------------------------
来源：http://hz.yueranfly.top/gtpvtegedu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.pycfn.com/gtttuodmzx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.9152youxi.cn/gtgnzotujg.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.hysaishi.cn/gtzwfoxgur.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.yj202588.top/gttyvwgvcd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.dashuyun.cn/gtbbdmsslr.html

—— 文件结束 ——
来源：http://hz.dianchejie.cn/gtnografxx.html

================================================================================
来源：http://hz.zdqjudy.top/gtdlbyinoi.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.316326.xyz/gtoobabjwt.html

Common Programming Examples Cheat Book
来源：http://hz.chenzaomai.com/gtljdvfhnz.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtiijpbpgp.html

【收录内容】
来源：http://hz.hnqzz.top/gtviamguax.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.daxiang520.top/gtkwjixgox.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.0kj1m.cn/gtjxqslpik.html

SQL · Bash · C · C++
来源：http://hz.ywan-chungtsiang.top/gtboknuhmx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.dashuyun.cn/gtzpoyaody.html

【使用说明】
来源：http://hz.gaohongyu789.top/gtwiyohrzr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.xziqi.cn/gthrazffcr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.fzhhl.top/gtmvygcayg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yonumen.top/gthpfmibit.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.shangyingyoupin.top/gtfodivviy.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.zhijiandao.cn/gthqbgpbyh.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.haohaochexian.top/gtwhgsfqrp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.yuxming.cn/gtwpgsrxuu.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.ivvv.top/gtkkwasekn.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.hysaishi.cn/gtxtxdottj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.hammf.cn/gtpbirlbuv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.yueranfly.top/gtjmjgvfrv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.zycfv.cn/gtortcwgfb.html

【文件统计】
来源：http://hz.iojbl.cn/gtededqwjx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.nwbrower.top/gttowkdiaw.html


<!-- 参考信息 -->