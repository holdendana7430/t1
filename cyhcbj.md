代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yueranfly.top/gtfoequpix.html

[R34] 退出时清理
来源：http://hz.xingfuxueyuan.xyz/gtwwhgzhgh.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.feifeiyinyue.top/gtnpdfzaxu.html

[R35] 后台执行并等待
来源：http://hz.guowangkeji.top/gtxkqkagef.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xziqi.cn/gtkzjqmcej.html

[R36] 并发执行多个任务
来源：http://hz.bjfxy.top/gtdsnobxny.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhiwuduotai.top/gtiaccbzkq.html

[R37] 把输出赋给变量
来源：http://hz.yj20258888.top/gtxpmjreay.html

files=$(ls -1)
来源：http://hz.daria6918.cn/gtcopebaew.html

[R38] 管道串联
来源：http://hz.cucudq.cn/gtbiypwken.html

cat a.txt | grep -i error | wc -l
来源：http://hz.tianlin.xyz/gtebekzgvv.html

[R39] 重定向标准输出与错误
来源：http://hz.ivvv.top/gtpfeskknf.html

cmd > out.log 2>&1
来源：http://hz.shanyushiyangtech.top/gtwvcszrwy.html

[R40] 追加写日志
来源：http://hz.c1oappe.top/gtpdqathxg.html

echo "log" >> out.log
来源：http://hz.shzxlz.cn/gtmicocpeh.html

[R41] 丢弃输出
来源：http://hz.nanxuanxn.top/gtitjrnaop.html

cmd >/dev/null 2>&1
来源：http://hz.jinyuanbaomall.cn/gtdlgilfgc.html

[R42] 输入重定向
来源：http://hz.redwolf501.top/gtwfmpuxwm.html

wc -l < a.txt
来源：http://hz.chenlongwang.top/gtulxlvtzn.html

[R43] 按名字查找文件
来源：http://hz.yongpay.top/gtnanwlpsu.html

find . -name "*.log" -type f
来源：http://hz.svipenyu.cn/gtgzdybmon.html

[R44] 按修改时间查找
来源：http://hz.shanyushiyangtech.top/gttutuohvq.html

find . -mtime -7 -type f
来源：http://hz.zhoulong.xyz/gtgicxbuov.html

[R45] 批量删除
来源：http://hz.bjfxy.top/gtsrzaejwo.html

find . -name "*.tmp" -delete
来源：http://hz.quarkkingdee.top/gtthywjsuk.html

[R46] 递归替换文件内容
来源：http://hz.fengsongda.top/gtvsmnrkpw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yuxming.cn/gtaoxdcmlh.html

[R47] sed 单行替换
来源：http://hz.ywan-chungtsiang.top/gtzfpaavzi.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.dianchejie.cn/gtgahrogqx.html

[R48] awk 取指定列
来源：http://hz.meibo888.top/gtepdommvy.html

awk '{print $1, $3}' a.txt
来源：http://hz.yuxming.cn/gtskadbsqj.html

[R49] awk 带条件
来源：http://hz.yuxming.cn/gtigtpwjwe.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.aibaodan.cn/gtesbccphj.html

[R50] awk 求和
来源：http://hz.jinqigfzy.top/gtkitboqon.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.redwolf501.top/gtwztummml.html

[R51] 排序去重取前几
来源：http://hz.jqgfzy.top/gtmzbjagla.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ivvv.top/gtrtgcwxje.html

[R52] 统计行数
来源：http://hz.jinyuanbaomall.cn/gtdjdlrmkb.html

wc -l a.txt
来源：http://hz.ehwqpu.com/gtvtcapbkw.html

[R53] 查看文件头与实时尾
来源：http://hz.xziqi.cn/gtsykkjtok.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.sufxvd.cn/gtleqoyitz.html

[R54] 比较两个文件
来源：http://hz.xylfe.cn/gtplorcpdb.html

diff a.txt b.txt
来源：http://hz.smart0.xyz/gtnmfrzjmf.html

[R55] 压缩与解压
来源：http://hz.ybcxt.top/gtfnvjbcyc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ydjk.org.cn/gtrfhsfhpw.html

[R56] 远程拷贝
来源：http://hz.quarkkingdee.top/gtxgwbsgfj.html

scp file user@host:/path/
来源：http://hz.yj20258888.top/gtbvyrxuwn.html

[R57] 远程执行命令
来源：http://hz.bjfxy.top/gtvptmiqhb.html

ssh user@host 'uptime'
来源：http://hz.daria6918.cn/gtgfgunups.html

[R58] 下载文件
来源：http://hz.gzhubu.top/gtshtnbvqu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.shanyushiyangtech.top/gtuhiwrqqo.html

[R59] 发 POST JSON
来源：http://hz.nanxinkj.top/gtumisuryz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.sysykeji.top/gtbsjojime.html

[R60] 只看 HTTP 状态码
来源：http://hz.shanyushiyangkeji.top/gthprvujlw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.tian-w.cn/gtkfxucllt.html

[R61] 磁盘占用
来源：http://hz.haohaochexian.top/gtchoifpbo.html

df -h;  du -sh *
来源：http://hz.shanyushiyangtech.top/gtwgipawzt.html

[R62] 找最占空间的文件
来源：http://hz.zdqjudy.top/gttodnuycm.html

du -ah . | sort -rh | head -10
来源：http://hz.hfpthk.cn/gtejnbcjdf.html

[R63] 内存与进程
来源：http://hz.quarkkingdee.top/gtugqodzvj.html

free -h;  ps aux | grep nginx
来源：http://hz.xingfuxueyuan.xyz/gtkjipmkvg.html

[R64] 结束进程
来源：http://hz.chenjidiqi.icu/gtsviskbqb.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hongshengwenyu.top/gtqirvkcbq.html

[R65] 查看端口占用
来源：http://hz.cucudq.cn/gtmezmspnx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.shanyushiyangkeji.top/gtzqxjjooi.html

[R66] 定时任务
来源：http://hz.shanyushiyangtech.top/gtucckgzlw.html

crontab -e;  crontab -l
来源：http://hz.cashguo.top/gtcyfteiom.html

[R67] 生成随机十六进制串
来源：http://hz.havefunace.top/gtcrijggzl.html

openssl rand -hex 16
来源：http://hz.kuanghao11.cn/gteprbxfxq.html

[R68] 计算文件校验值
来源：http://hz.zhaomingkeji.xyz/gtltyemckp.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.aizwys.cn/gtvlropxff.html

[R69] 生成随机密码
来源：http://hz.fengsongda.top/gtfinoeyrf.html

head -c 16 /dev/urandom | base64
来源：http://hz.ivvv.top/gtrcqfabbc.html

[R70] 时间戳与互转
来源：http://hz.ppjwa.cn/gtykadnegj.html

date +%s;  date -d @1700000000
来源：http://hz.bjfxy.top/gtqwaokped.html

[R71] 日期格式化
来源：http://hz.sxryk.cn/gtcdvudpdy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.nwbrower.top/gtwvuzwtmv.html

[R72] 等待端口就绪
来源：http://hz.tanke756.top/gtobsdkkqi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.gaohongyu789.top/gtoousllvw.html

[R73] 分割大日志
来源：http://hz.hammf.cn/gthnfzzupm.html

split -l 1000 big.log part_
来源：http://hz.shzxlz.cn/gtyndqyztp.html

[R74] 批量重命名
来源：http://hz.9152youxi.cn/gtmkabjjul.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhixingplan.top/gtxhxdrvud.html

[R75] 导出环境变量
来源：http://hz.yueranfly.top/gteevriewb.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.52xcode.cn/gtqljivlgi.html

[R76] 使用临时文件
来源：http://hz.zhaomingkeji.xyz/gtuychpazq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenlongwang.top/gtccyjcpyv.html

[R77] 读取用户输入
来源：http://hz.zdqjudy.top/gtlbmcfmev.html

read -rp "请输入: " ans
来源：http://hz.nanxinkj.top/gtmjbazasv.html

[R78] 交互式菜单
来源：http://hz.yangfankeji.com/gttefkyoiw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.svipenyu.cn/gtfacbsszj.html

[R79] 解析命令行选项
来源：http://hz.andypj.xyz/gtflzyevqj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jqgufenzy.top/gtgvnkaxmo.html

[R80] 查看脚本执行耗时
来源：http://hz.hnqzz.top/gtanvcanna.html

time ./run.sh
来源：http://hz.yanxiufei.cn/gtmymnhaik.html

================================================================================
来源：http://hz.sufxvd.cn/gtjsikzwfh.html

S. C / C++ 专题
来源：http://hz.0kj1m.cn/gtiinwdqol.html

================================================================================
来源：http://hz.gogol.net.cn/gtyoxnldvd.html

[S01] C：Hello World
来源：http://hz.bjfxy.top/gtlgykjvtq.html

#include <stdio.h>
来源：http://hz.yj202588.top/gtadrercpf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hongshengwenyu.top/gtvdhkfecg.html

[S02] C：变量与格式化输出
来源：http://hz.feifeiyinyue.top/gtwlbtxqpr.html

int a = 10; printf("%d\n", a);
来源：http://hz.yuanzhike.top/gtwitmvfce.html

[S03] C：读入整数
来源：http://hz.jianghu66.top/gtrglsqhpq.html

int x; scanf("%d", &x);
来源：http://hz.pengpengdd.cyou/gtzepwhmlo.html

[S04] C：字符串复制
来源：http://hz.chenzaomai.com/gtydyofbjk.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jinqigfzy.top/gtenupdygc.html

[S05] C：字符串长度
来源：http://hz.hfpthk.cn/gtbyiakqhf.html

strlen(s)
来源：http://hz.yj202588.top/gtrdyguxvj.html

[S06] C：字符串比较
来源：http://hz.xinyue.icu/gtuvzzswzw.html

strcmp(a, b) == 0
来源：http://hz.tianlin.xyz/gtpaiyappb.html

[S07] C：数组遍历求和
来源：http://hz.sysykeji.top/gtivkdnbgc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.haohaochexian.top/gtarxvmhce.html

[S08] C：动态内存分配与释放
来源：http://hz.hnxiangtu.top/gtcnxgsiyv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.tianlin.xyz/gtgzbyakcl.html

[S09] C：结构体定义与初始化
来源：http://hz.snrcjt.cn/gtgmnldvok.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yj20258888.top/gtythbtshn.html

[S10] C：指针与解引用
来源：http://hz.andypj.xyz/gtrhindmhi.html

int *p = &a;  *p = 5;
来源：http://hz.havefunace.top/gtauocpqqp.html

[S11] C：逐行读文件
来源：http://hz.jlsjyb.cn/gtpbictlai.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.tian-w.cn/gtwsgyeywk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.nwbrower.top/gtehztnnwf.html

fclose(f);
来源：http://hz.ppjwa.cn/gtnxvzoyod.html

[S12] C：写文件
来源：http://hz.snrcjt.cn/gtuntpomhu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xylfe.cn/gtklgskvlv.html

[S13] C：宏定义
来源：http://hz.yj202588.top/gtastqslzf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jianghu66.top/gtfcocbypd.html

[S14] C：枚举
来源：http://hz.c1oappe.top/gterygelop.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yongpay.top/gtbezqntft.html

[S15] C：类型转换
来源：http://hz.hfpthk.cn/gthdwseqtt.html

(double) a / b
来源：http://hz.meibo888.top/gtvzfohiaq.html

[S16] C：位操作置位
来源：http://hz.zhaomingkeji.xyz/gtzvtkmhex.html

x |= (1 << 3);
来源：http://hz.sysykeji.top/gtxrpkrqdi.html

[S17] C：安全拼接字符串
来源：http://hz.sxryk.cn/gtzaflliel.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.pengpengdd.cyou/gtjynszhal.html

[S18] C：命令行参数
来源：http://hz.zhiwuduotai.top/gtwlboetmr.html

int main(int argc, char **argv)
来源：http://hz.zhongyouzk.top/gtveqdjyba.html

[S19] C：快速排序
来源：http://hz.yonumen.top/gtvweiwvth.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.chenzaomai.com/gtjlalpepe.html

[S20] C：二分查找
来源：http://hz.ppjwa.cn/gtdsgtapxb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.bjfxy.top/gtdqihcgtx.html

[S21] C：字符类别判断
来源：http://hz.dianchejie.cn/gtlpwvqmty.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhongyouzk.top/gtozavkcpo.html

[S22] C：字符串转数字
来源：http://hz.kuanghao11.cn/gttkjluwve.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.dashuyun.cn/gtpjkwxtmb.html

[S23] C：随机数
来源：http://hz.pycfn.com/gtlqloqplg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.chenzaomai.com/gtbbrmhmko.html

[S24] C：获取本地时间
来源：http://hz.tian-w.cn/gtoqptfktd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yj202588.top/gttnuyfodr.html

[S25] C：内存拷贝
来源：http://hz.jlsjyb.cn/gturimurgr.html

memcpy(dst, src, n);
来源：http://hz.xinyue.icu/gtywxmvcez.html

[S26] C：内存清零
来源：http://hz.ppjwa.cn/gtvphfeusj.html

memset(a, 0, sizeof a);
来源：http://hz.aibaodan.cn/gtbrxaoveh.html

[S27] C：定义常量
来源：http://hz.cucudq.cn/gtimmhyioa.html

const double PI = 3.14159;
来源：http://hz.zdqjudy.top/gtsnmexjvp.html

[S28] C：静态变量
来源：http://hz.zhaomingkeji.xyz/gtpobytgpc.html

static int counter = 0;
来源：http://hz.zhoulong.xyz/gttkdtkawt.html

[S29] C：变参函数
来源：http://hz.9152youxi.cn/gtsanuukvl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yvedp.cn/gtnnvcuesv.html

[S30] C：头文件保护
来源：http://hz.zhongyouzk.top/gtkmdgxozk.html

#ifndef X_H
来源：http://hz.shanyushiyangkeji.top/gtnuhfnibu.html

#define X_H
来源：http://hz.jlsjyb.cn/gthfrcudeo.html

#endif
来源：http://hz.nanxuanxn.top/gtgylyennn.html

[S31] C++：Hello World
来源：http://hz.52xcode.cn/gtjdgenfnr.html

#include <iostream>
来源：http://hz.kuanghao11.cn/gtrnqmwaox.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jqgufenzy.top/gtqohymmep.html

[S32] C++：字符串
来源：http://hz.gogol.net.cn/gtymwjdaiy.html

std::string s = "hi";  s += "!";
来源：http://hz.smart0.xyz/gtnohqfbgf.html

[S33] C++：vector 增删
来源：http://hz.ivvv.top/gtlnnjevyy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.316326.xyz/gtxboiurgv.html

[S34] C++：遍历 vector
来源：http://hz.zhoulong.xyz/gtcyqulkpx.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shangyingyoupin.top/gtfxtmwljx.html

[S35] C++：map
来源：http://hz.meibo888.top/gtlajffgfq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hfpthk.cn/gtannfhpqw.html

[S36] C++：unordered_map
来源：http://hz.guannengcc.top/gtkvyzqvay.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nwbrower.top/gtmoqjbdas.html

[S37] C++：set
来源：http://hz.c1oappe.top/gttfqtegbf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.c1oappe.top/gtdlrqvgue.html

[S38] C++：排序
来源：http://hz.shanyushiyangkeji.top/gtjsxogtzc.html

std::sort(v.begin(), v.end());
来源：http://hz.shanyushiyangtech.top/gtsvosyvca.html

[S39] C++：自定义比较器排序
来源：http://hz.aizwys.cn/gtqqonanrf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.pycfn.com/gtodlvjfov.html

[S40] C++：查找元素
来源：http://hz.tanke756.top/gtflihtacw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yuxming.cn/gtrtrvrhjy.html

[S41] C++：类与构造函数
来源：http://hz.jinyuanbaomall.cn/gtshbbiruh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hongshengwenyu.top/gtcswaixnb.html

[S42] C++：继承与虚函数
来源：http://hz.meibo888.top/gtybshzrsi.html

class B : public Base { public: void f() override {} };
来源：http://hz.meibo888.top/gtbrqnsing.html

[S43] C++：智能指针
来源：http://hz.birdmap.top/gtsiitzniy.html

auto p = std::make_unique<int>(5);
来源：http://hz.chenzaomai.com/gtbzmxvovt.html

[S44] C++：引用传参
来源：http://hz.gzhubu.top/gtinhsnbjv.html

void inc(int &x) { ++x; }
来源：http://hz.gogol.net.cn/gtqtwfirln.html

[S45] C++：lambda
来源：http://hz.cucudq.cn/gtkateerzr.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zycfv.cn/gtnqchntxd.html

[S46] C++：函数模板
来源：http://hz.bjfxy.top/gtxviawhvv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.aibaodan.cn/gticssajny.html

[S47] C++：结构化绑定遍历
来源：http://hz.yangfankeji.com/gtnzffrobt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhijiandao.cn/gthgalsqkq.html

[S48] C++：逐行读文件
来源：http://hz.cucudq.cn/gtyukeqjbt.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.haohaochexian.top/gtltaghztv.html

while (std::getline(in, line)) { }
来源：http://hz.shanyushiyangtech.top/gtxhhoiypu.html

[S49] C++：写文件
来源：http://hz.pycfn.com/gtbrtiehpz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.snrcjt.cn/gtjqajhlub.html

[S50] C++：格式化数字
来源：http://hz.meibo888.top/gtlfrncuds.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yangfankeji.com/gtlohprlat.html

[S51] C++：显式类型转换
来源：http://hz.zhaomingkeji.xyz/gttwuvovtp.html

static_cast<double>(a) / b
来源：http://hz.cheryme.top/gtlbomaccu.html

[S52] C++：const 与 noexcept
来源：http://hz.xuanzx.com/gtncgonymg.html

int size() const noexcept { return n_; }
来源：http://hz.hongshengwenyu.top/gtqraesiuw.html

[S53] C++：移动语义
来源：http://hz.52xcode.cn/gtemjndoul.html

std::vector<int> w = std::move(v);
来源：http://hz.aizwys.cn/gtwzhkvbvw.html

[S54] C++：异常处理
来源：http://hz.chenzaomai.com/gtldxmlllh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhoulong.xyz/gtjppvkfmu.html

[S55] C++：结构化绑定
来源：http://hz.yj202588.top/gtijyqllfg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.gzhubu.top/gtfowvzzpc.html

[S56] C++：optional
来源：http://hz.smart0.xyz/gthhtaqgnd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jlsjyb.cn/gtqjyspiuq.html

[S57] C++：编译期常量
来源：http://hz.gzhubu.top/gtnsvgutzr.html

constexpr int N = 10;
来源：http://hz.hnxiangtu.top/gtwpdmromt.html

[S58] C++：命名空间
来源：http://hz.tian-w.cn/gtblrvwgny.html

namespace ns { int f() { return 1; } }
来源：http://hz.birdmap.top/gtloqgtgxl.html

[S59] C++：静态断言
来源：http://hz.gzhubu.top/gtyplhejqj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jyoumei.cn/gtgpbcnnbc.html

[S60] C++：遍历并删除元素
来源：http://hz.meibo888.top/gthwfaoddy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.fzhhl.top/gtxmurcmdy.html

================================================================================
来源：http://hz.daxiang520.top/gtenftrajy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shanyushiyangtech.top/gtmsxmoduu.html

================================================================================
来源：http://hz.shuidangran.top/gthnbapkrt.html

[T01] Kotlin：Hello World
来源：http://hz.tianlin.xyz/gtzdbxklpt.html

println("Hello")
来源：http://hz.cdnleiting.top/gtcirsntbx.html

[T02] Kotlin：变量
来源：http://hz.hysaishi.cn/gtxondddfj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.aizwys.cn/gtpmchcooy.html

[T03] Kotlin：字符串模板
来源：http://hz.shuidangran.top/gtxcglkwin.html

"值: $b"
来源：http://hz.ppjwa.cn/gtvrsnpkrw.html

[T04] Kotlin：空安全
来源：http://hz.ppjwa.cn/gtutcropen.html

val n: String? = null;  n?.length
来源：http://hz.shuidangran.top/gtuhgbrwyn.html

[T05] Kotlin：when 表达式
来源：http://hz.shangyingyoupin.top/gtuuibugux.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yanxiufei.cn/gtgugkkpda.html

[T06] Kotlin：集合映射
来源：http://hz.xuanzx.com/gtznnperau.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.cashguo.top/gtgjmczpfi.html

[T07] Kotlin：集合过滤
来源：http://hz.ppjwa.cn/gtshclzzij.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhengqikj.top/gtrrrxwnma.html

[T08] Kotlin：数据类
来源：http://hz.cqqwz.cn/gtbxtpjzzy.html

data class User(val name: String, val age: Int)
来源：http://hz.yj202588.top/gtzurjpqrd.html

[T09] Kotlin：扩展函数
来源：http://hz.ydjk.org.cn/gttdkckubc.html

fun String.exclaim() = this + "!"
来源：http://hz.zdqjudy.top/gtvjdcuqps.html

[T10] Kotlin：默认参数
来源：http://hz.pycfn.com/gtbentqzhr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.sweek.top/gtegdpjbbu.html

[T11] Kotlin：协程
来源：http://hz.ppjwa.cn/gtcguqtwqg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.birdmap.top/gtdabrabta.html

[T12] Kotlin：解构声明
来源：http://hz.jinghuilouyu.cn/gtsqvmpkjg.html

val (a, b) = Pair(1, 2)
来源：http://hz.xinyue.icu/gtcfimiwkm.html

[T13] Kotlin：只读 Map
来源：http://hz.zdqjudy.top/gtscuzcnug.html

val m = mapOf("a" to 1)
来源：http://hz.ydjk.org.cn/gtbscxacxg.html

[T14] Kotlin：循环
来源：http://hz.gogol.net.cn/gtkqryevqf.html

for (i in 1..10) println(i)
来源：http://hz.cucudq.cn/gtcpdgaikc.html

[T15] Kotlin：接口
来源：http://hz.havefunace.top/gthucwvxmj.html

interface Shape { fun area(): Double }
来源：http://hz.dianchejie.cn/gtcfqwmufm.html

[T16] Swift：Hello World
来源：http://hz.fengsongda.top/gtnuslodfc.html

print("Hello")
来源：http://hz.haohaochexian.top/gtwkljemwe.html

[T17] Swift：变量与常量
来源：http://hz.jinqigufen.top/gtsmbumiyv.html

var a = 1;  let b = 2
来源：http://hz.sufxvd.cn/gtivdqtcoz.html

[T18] Swift：字符串插值
来源：http://hz.guowangkeji.top/gtrfrzevjo.html

"值: \(b)"
来源：http://hz.sxryk.cn/gtllwkshld.html

[T19] Swift：可选绑定
来源：http://hz.hywenlv.cn/gttyfaaioe.html

if let n = opt { print(n) }
来源：http://hz.ppjwa.cn/gtdpyezpjb.html

[T20] Swift：数组操作
来源：http://hz.sysykeji.top/gtipichxyj.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jlsjyb.cn/gtokbambua.html

[T21] Swift：遍历
来源：http://hz.meibo888.top/gtbnltvxlg.html

for x in a { print(x) }
来源：http://hz.hammf.cn/gtmsqprgxh.html

[T22] Swift：字典
来源：http://hz.mhx1999.top/gtilghpqpf.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zycfv.cn/gtwxktbppb.html

[T23] Swift：函数
来源：http://hz.gogol.net.cn/gtnhthlkyc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yonumen.top/gtxchagfdi.html

[T24] Swift：闭包
来源：http://hz.meibo888.top/gtfzibkgnd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.fzhhl.top/gtrjesihzr.html

[T25] Swift：结构体
来源：http://hz.quarkkingdee.top/gtwfhompku.html

struct P { var x: Int }
来源：http://hz.tianlin.xyz/gtqbaaymtp.html

[T26] Swift：类与重写
来源：http://hz.yueranfly.top/gtiroiimhj.html

class A: Base { override func f() {} }
来源：http://hz.gotoacloud.top/gtlwqdwrth.html

[T27] Swift：错误处理
来源：http://hz.snrcjt.cn/gtuwmpdpww.html

do { try f() } catch { print(error) }
来源：http://hz.fzhhl.top/gtmykwfcjw.html

[T28] Swift：枚举
来源：http://hz.jqgfzy.top/gtxsktkcff.html

enum Color { case red, green }
来源：http://hz.zycfv.cn/gtvkhkrjpo.html

[T29] Swift：guard 提前返回
来源：http://hz.gaohongyu789.top/gtekuvyhcf.html

guard let x = opt else { return }
来源：http://hz.hysaishi.cn/gtnqvfuzeu.html

[T30] Swift：协议
来源：http://hz.kuanghao11.cn/gtrwhlcioq.html

protocol Shape { func area() -> Double }
来源：http://hz.redwolf501.top/gtyfnvxkxn.html

[T31] Lua：Hello World
来源：http://hz.sxryk.cn/gtytqhdtde.html

print("Hello")
来源：http://hz.ehwqpu.com/gtdbgsmwam.html

[T32] Lua：局部变量
来源：http://hz.yanxiufei.cn/gtatrnfrpv.html

local a = 1
来源：http://hz.jqgfzy.top/gtasoywokk.html

[T33] Lua：表（数组）
来源：http://hz.guowangkeji.top/gtjvpgsmzv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.shuidangran.top/gtaqfbrrjx.html

[T34] Lua：遍历表
来源：http://hz.mhx1999.top/gtnlxkafmv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jqgfzy.top/gtxkzlkhck.html

[T35] Lua：字典表
来源：http://hz.hywenlv.cn/gtmlsyxtjc.html

local d = { a = 1 };  d.b = 2
来源：http://hz.kuanghao11.cn/gtdndbtqvk.html

[T36] Lua：函数
来源：http://hz.xylfe.cn/gttskqpsrx.html

function add(a, b) return a + b end
来源：http://hz.zhoulong.xyz/gteawzjvhf.html


<!-- 参考信息 -->