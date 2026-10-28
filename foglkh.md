代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.gzhubu.top/gtocboubtn.html

[R34] 退出时清理
来源：http://hz.mhx1999.top/gteakjggad.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.cashguo.top/gtsxrtvluv.html

[R35] 后台执行并等待
来源：http://hz.fengsongda.top/gtupcshzps.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hywenlv.cn/gtegpacatr.html

[R36] 并发执行多个任务
来源：http://hz.jinqigufen.top/gtcpyscxif.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cheryme.top/gtccrposvi.html

[R37] 把输出赋给变量
来源：http://hz.yangfankeji.com/gtepjyocwr.html

files=$(ls -1)
来源：http://hz.daxiang520.top/gtyfbhxvou.html

[R38] 管道串联
来源：http://hz.sufxvd.cn/gtnhxhydjh.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hnqzz.top/gthkezgybm.html

[R39] 重定向标准输出与错误
来源：http://hz.gotoacloud.top/gtuvbfpwzq.html

cmd > out.log 2>&1
来源：http://hz.jinyuanbaomall.cn/gtahrybomm.html

[R40] 追加写日志
来源：http://hz.jqgufenzy.top/gtdtkfmsad.html

echo "log" >> out.log
来源：http://hz.yuanzhike.top/gtfnfuxdpb.html

[R41] 丢弃输出
来源：http://hz.xinyue.icu/gtqifmbbzm.html

cmd >/dev/null 2>&1
来源：http://hz.smart0.xyz/gtxxgiqqyz.html

[R42] 输入重定向
来源：http://hz.zhengqikj.top/gtkfxliuta.html

wc -l < a.txt
来源：http://hz.dianchejie.cn/gtictvpfai.html

[R43] 按名字查找文件
来源：http://hz.sufxvd.cn/gtmtqfllkw.html

find . -name "*.log" -type f
来源：http://hz.yvedp.cn/gtyjdwtacc.html

[R44] 按修改时间查找
来源：http://hz.shuidangran.top/gtzuatofxg.html

find . -mtime -7 -type f
来源：http://hz.tian-w.cn/gthbarjwpl.html

[R45] 批量删除
来源：http://hz.ybcxt.top/gtnvdjzsbj.html

find . -name "*.tmp" -delete
来源：http://hz.hnqzz.top/gtnbpxoqxq.html

[R46] 递归替换文件内容
来源：http://hz.wangshuangyany.cn/gtkoicdajm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.shangyingyoupin.top/gtbgyeuihw.html

[R47] sed 单行替换
来源：http://hz.cdnleiting.top/gtghdrtnup.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.andypj.xyz/gtuenodotj.html

[R48] awk 取指定列
来源：http://hz.feifeiyinyue.top/gtxpuruwjb.html

awk '{print $1, $3}' a.txt
来源：http://hz.cheryme.top/gtsfetmmjf.html

[R49] awk 带条件
来源：http://hz.zhixingplan.top/gtwgdrofui.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.quarkkingdee.top/gtqmqjnwat.html

[R50] awk 求和
来源：http://hz.zhoulong.xyz/gtdkmkxdfm.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xziqi.cn/gtvfxrpshs.html

[R51] 排序去重取前几
来源：http://hz.hywenlv.cn/gtjlhzyinm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.smart0.xyz/gtpwrujqpw.html

[R52] 统计行数
来源：http://hz.c1oappe.top/gtnlsiyqyw.html

wc -l a.txt
来源：http://hz.wangdashe.top/gtkesjfvom.html

[R53] 查看文件头与实时尾
来源：http://hz.zhijiandao.cn/gtzdzuritw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.dianchejie.cn/gtpipvsxkz.html

[R54] 比较两个文件
来源：http://hz.hywenlv.cn/gtqijjuwpt.html

diff a.txt b.txt
来源：http://hz.pycfn.com/gtuzyvphkr.html

[R55] 压缩与解压
来源：http://hz.yangfankeji.com/gtuaukdlzt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.daxiang520.top/gtjvnmhuly.html

[R56] 远程拷贝
来源：http://hz.zhongyouzk.top/gtezxdnfza.html

scp file user@host:/path/
来源：http://hz.yangfankeji.com/gthqasalkd.html

[R57] 远程执行命令
来源：http://hz.shanyushiyangtech.top/gtanqifdas.html

ssh user@host 'uptime'
来源：http://hz.smart0.xyz/gtipgihxjc.html

[R58] 下载文件
来源：http://hz.sysykeji.top/gthrowjvbj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.pengpengdd.cyou/gtmzifyysl.html

[R59] 发 POST JSON
来源：http://hz.havefunace.top/gtzryhumnl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jlsjyb.cn/gtxzfjhdzf.html

[R60] 只看 HTTP 状态码
来源：http://hz.xuanzx.com/gtyjvbokmv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zycfv.cn/gtsuxdnker.html

[R61] 磁盘占用
来源：http://hz.yongpay.top/gtqnnpgmpz.html

df -h;  du -sh *
来源：http://hz.fzhhl.top/gtkkmneyme.html

[R62] 找最占空间的文件
来源：http://hz.aizwys.cn/gtobtvhslb.html

du -ah . | sort -rh | head -10
来源：http://hz.zycfv.cn/gtowgrqecs.html

[R63] 内存与进程
来源：http://hz.bjfxy.top/gtfpepzpzw.html

free -h;  ps aux | grep nginx
来源：http://hz.zhiwuduotai.top/gtsmktajya.html

[R64] 结束进程
来源：http://hz.haohaochexian.top/gttpsziwzz.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jyoumei.cn/gtmzqhmqne.html

[R65] 查看端口占用
来源：http://hz.chenjidiqi.icu/gtjtznfioe.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xingfuxueyuan.xyz/gtbkqskizi.html

[R66] 定时任务
来源：http://hz.gzhubu.top/gtywtzykjp.html

crontab -e;  crontab -l
来源：http://hz.jinqigfzy.top/gtyxjdzcrn.html

[R67] 生成随机十六进制串
来源：http://hz.gzhubu.top/gtnbavskgq.html

openssl rand -hex 16
来源：http://hz.ydjk.org.cn/gtmifchxdi.html

[R68] 计算文件校验值
来源：http://hz.hysaishi.cn/gtjtzkgcgi.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cheryme.top/gtgkpsaczq.html

[R69] 生成随机密码
来源：http://hz.haohaochexian.top/gtffyytvrl.html

head -c 16 /dev/urandom | base64
来源：http://hz.yj202588.top/gtorypbmnz.html

[R70] 时间戳与互转
来源：http://hz.jqgufenzy.top/gtwbpivelf.html

date +%s;  date -d @1700000000
来源：http://hz.tian-w.cn/gtiquknxds.html

[R71] 日期格式化
来源：http://hz.gaohongyu789.top/gtntqjvyvq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.andypj.xyz/gtsevuwaxb.html

[R72] 等待端口就绪
来源：http://hz.shangyingyoupin.top/gtcetnkbmf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jqgfzy.top/gtzbfiyhkd.html

[R73] 分割大日志
来源：http://hz.yangfankeji.com/gtmmkfnjxe.html

split -l 1000 big.log part_
来源：http://hz.shuidangran.top/gtjkmsxclm.html

[R74] 批量重命名
来源：http://hz.zhoulong.xyz/gtqnklrzpd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yj20258.top/gtlosftloo.html

[R75] 导出环境变量
来源：http://hz.jlsjyb.cn/gtcaoasccj.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.c1oappe.top/gtjlwmunkn.html

[R76] 使用临时文件
来源：http://hz.dashuyun.cn/gtxkpsikcz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hongshengwenyu.top/gtyuxfdjox.html

[R77] 读取用户输入
来源：http://hz.dianchejie.cn/gtcsawdbly.html

read -rp "请输入: " ans
来源：http://hz.yuxming.cn/gtjdumulbv.html

[R78] 交互式菜单
来源：http://hz.cashguo.top/gtzjstodin.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yonumen.top/gtxaukpuca.html

[R79] 解析命令行选项
来源：http://hz.cheryme.top/gtkdrjwmoo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xinyue.icu/gtgcjxcjtz.html

[R80] 查看脚本执行耗时
来源：http://hz.xylfe.cn/gtgpjyybzt.html

time ./run.sh
来源：http://hz.ivvv.top/gtorbmqlyf.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gthgkvvcrb.html

S. C / C++ 专题
来源：http://hz.316326.xyz/gtwprlzcnl.html

================================================================================
来源：http://hz.hammf.cn/gtpquehtaa.html

[S01] C：Hello World
来源：http://hz.yonumen.top/gtaehwzmxd.html

#include <stdio.h>
来源：http://hz.cqqwz.cn/gtpeaxprwe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hywenlv.cn/gtrychzbwk.html

[S02] C：变量与格式化输出
来源：http://hz.yonumen.top/gtjnubjkgg.html

int a = 10; printf("%d\n", a);
来源：http://hz.nwbrower.top/gtannducax.html

[S03] C：读入整数
来源：http://hz.sxryk.cn/gtzdasjqne.html

int x; scanf("%d", &x);
来源：http://hz.chenlongwang.top/gtaqthsjkk.html

[S04] C：字符串复制
来源：http://hz.havefunace.top/gtucnizdnb.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.sysykeji.top/gtiwwhcazr.html

[S05] C：字符串长度
来源：http://hz.zdqjudy.top/gtuauczexb.html

strlen(s)
来源：http://hz.xylfe.cn/gtdpuldqcw.html

[S06] C：字符串比较
来源：http://hz.yueranfly.top/gtkgzdqvib.html

strcmp(a, b) == 0
来源：http://hz.aizwys.cn/gtxequxfgi.html

[S07] C：数组遍历求和
来源：http://hz.hnqzz.top/gtswinhmvc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gogol.net.cn/gtdwpbnnxw.html

[S08] C：动态内存分配与释放
来源：http://hz.feifeiyinyue.top/gtyhufmvsv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinghuilouyu.cn/gtuuszkfqc.html

[S09] C：结构体定义与初始化
来源：http://hz.chenlongwang.top/gtfzprabwe.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.guannengcc.top/gtzaybkakz.html

[S10] C：指针与解引用
来源：http://hz.gotoacloud.top/gtbvdhahuk.html

int *p = &a;  *p = 5;
来源：http://hz.ybcxt.top/gtypoodanh.html

[S11] C：逐行读文件
来源：http://hz.tian-w.cn/gtybtcgmbv.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jinghuilouyu.cn/gtrffcwczt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jqgufenzy.top/gtbynvkopn.html

fclose(f);
来源：http://hz.havefunace.top/gtdngqfakt.html

[S12] C：写文件
来源：http://hz.hfpthk.cn/gtqrfauudz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.snrcjt.cn/gtrkpnszjx.html

[S13] C：宏定义
来源：http://hz.hysaishi.cn/gtxbwxayxu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.sysykeji.top/gtbngjtzqp.html

[S14] C：枚举
来源：http://hz.jyoumei.cn/gtoleviyld.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yuanzhike.top/gtyorxjwqq.html

[S15] C：类型转换
来源：http://hz.svipenyu.cn/gthithraec.html

(double) a / b
来源：http://hz.guannengcc.top/gtliuthfgi.html

[S16] C：位操作置位
来源：http://hz.mhx1999.top/gtvqlgixxl.html

x |= (1 << 3);
来源：http://hz.yueranfly.top/gtvgswrozd.html

[S17] C：安全拼接字符串
来源：http://hz.sysykeji.top/gtjwgxlrdw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ydzc1.top/gtmuoenkni.html

[S18] C：命令行参数
来源：http://hz.sweek.top/gtovbegsft.html

int main(int argc, char **argv)
来源：http://hz.dashuyun.cn/gtaxuifsjl.html

[S19] C：快速排序
来源：http://hz.cashguo.top/gtllcrubgu.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cqqwz.cn/gtzwcfbkxq.html

[S20] C：二分查找
来源：http://hz.sufxvd.cn/gtyhmvagru.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.9152youxi.cn/gtniutjvzk.html

[S21] C：字符类别判断
来源：http://hz.jinqigfzy.top/gtyvegpbne.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.shuidangran.top/gtowygzcgd.html

[S22] C：字符串转数字
来源：http://hz.9152youxi.cn/gthndebcoi.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.gotoacloud.top/gtcefetnqa.html

[S23] C：随机数
来源：http://hz.yj20258.top/gtqsrpreoi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.nwbrower.top/gtlfkespal.html

[S24] C：获取本地时间
来源：http://hz.c1oappe.top/gtsvyoewyh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.cashguo.top/gtonurzsgx.html

[S25] C：内存拷贝
来源：http://hz.shuidangran.top/gtozbyacok.html

memcpy(dst, src, n);
来源：http://hz.jqgfzy.top/gtzwmtaitb.html

[S26] C：内存清零
来源：http://hz.dianchejie.cn/gtdrhuttjz.html

memset(a, 0, sizeof a);
来源：http://hz.svipenyu.cn/gtqbsiysuk.html

[S27] C：定义常量
来源：http://hz.feifeiyinyue.top/gtiqekubwa.html

const double PI = 3.14159;
来源：http://hz.feifeiyinyue.top/gtaobsupkg.html

[S28] C：静态变量
来源：http://hz.dianchejie.cn/gtuafsfsgn.html

static int counter = 0;
来源：http://hz.shanyushiyangtech.top/gtggpgfycd.html

[S29] C：变参函数
来源：http://hz.daxiang520.top/gtfwdjdvbh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jinghuilouyu.cn/gtxtmknett.html

[S30] C：头文件保护
来源：http://hz.cheryme.top/gtmlrcjcdm.html

#ifndef X_H
来源：http://hz.gzhubu.top/gtsyqjdhii.html

#define X_H
来源：http://hz.wangshuangyany.cn/gtkyyabdqw.html

#endif
来源：http://hz.birdmap.top/gtmjnrfuuo.html

[S31] C++：Hello World
来源：http://hz.dashuyun.cn/gtpozfdgpv.html

#include <iostream>
来源：http://hz.zhijiandao.cn/gtafgirufs.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xziqi.cn/gtvhekrfew.html

[S32] C++：字符串
来源：http://hz.hywenlv.cn/gtmvbnptiu.html

std::string s = "hi";  s += "!";
来源：http://hz.tian-w.cn/gtgdjemfnr.html

[S33] C++：vector 增删
来源：http://hz.yvedp.cn/gtqkgloyej.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.daria6918.cn/gtodrdvgdi.html

[S34] C++：遍历 vector
来源：http://hz.zhijiandao.cn/gthzkhfjnz.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cqqwz.cn/gtgbiilzki.html

[S35] C++：map
来源：http://hz.redwolf501.top/gtnogylbts.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.quarkkingdee.top/gtznavlimf.html

[S36] C++：unordered_map
来源：http://hz.jianghu66.top/gtkixwdraq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shuidangran.top/gtoqjwhntb.html

[S37] C++：set
来源：http://hz.dashuyun.cn/gtedklswnw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.shanyushiyangkeji.top/gtxmqsvbbx.html

[S38] C++：排序
来源：http://hz.smart0.xyz/gtpyoofsox.html

std::sort(v.begin(), v.end());
来源：http://hz.fzhhl.top/gthhwnqaez.html

[S39] C++：自定义比较器排序
来源：http://hz.tianlin.xyz/gtabchnftn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yuxming.cn/gtbewaglsr.html

[S40] C++：查找元素
来源：http://hz.nwbrower.top/gtlovedyje.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hnxiangtu.top/gtgvhvuukl.html

[S41] C++：类与构造函数
来源：http://hz.yj20258.top/gtlkxmshqh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.mhx1999.top/gtneyehczr.html

[S42] C++：继承与虚函数
来源：http://hz.aibaodan.cn/gtdwpuynhf.html

class B : public Base { public: void f() override {} };
来源：http://hz.hnxiangtu.top/gtsrjyxekf.html

[S43] C++：智能指针
来源：http://hz.zhijiandao.cn/gtovgrndqx.html

auto p = std::make_unique<int>(5);
来源：http://hz.xuanzx.com/gteimzvcxl.html

[S44] C++：引用传参
来源：http://hz.cdnleiting.top/gtdiuyoght.html

void inc(int &x) { ++x; }
来源：http://hz.316326.xyz/gtbgrafjwg.html

[S45] C++：lambda
来源：http://hz.hywenlv.cn/gtimzyhuce.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jlsjyb.cn/gtonbeejnc.html

[S46] C++：函数模板
来源：http://hz.yvedp.cn/gtyoiyyppg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.tanke756.top/gtuxqdssbm.html

[S47] C++：结构化绑定遍历
来源：http://hz.jinqigufen.top/gtyifoqrtl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhaomingkeji.xyz/gtacvgmsct.html

[S48] C++：逐行读文件
来源：http://hz.jqgufenzy.top/gtfxhfnaji.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.chenjidiqi.icu/gttmvjrocf.html

while (std::getline(in, line)) { }
来源：http://hz.shuidangran.top/gtknrkfxje.html

[S49] C++：写文件
来源：http://hz.aibaodan.cn/gtigalioud.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hnqzz.top/gtpcafkubg.html

[S50] C++：格式化数字
来源：http://hz.zhixingplan.top/gtceqrdmmj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xingfuxueyuan.xyz/gtnizcvdla.html

[S51] C++：显式类型转换
来源：http://hz.gaohongyu789.top/gtunaorglz.html

static_cast<double>(a) / b
来源：http://hz.zhoulong.xyz/gtvwtpoqbd.html

[S52] C++：const 与 noexcept
来源：http://hz.yueranfly.top/gtdfwruigb.html

int size() const noexcept { return n_; }
来源：http://hz.shzxlz.cn/gttrnblvsh.html

[S53] C++：移动语义
来源：http://hz.yanxiufei.cn/gtdfbpsjde.html

std::vector<int> w = std::move(v);
来源：http://hz.jinghuilouyu.cn/gtonnfdree.html

[S54] C++：异常处理
来源：http://hz.316326.xyz/gtjipamper.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.316326.xyz/gtaeqbgtmg.html

[S55] C++：结构化绑定
来源：http://hz.9152youxi.cn/gtwehnpnmf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.cashguo.top/gtfkijsgxv.html

[S56] C++：optional
来源：http://hz.svipenyu.cn/gtcxrsbrod.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jqgufenzy.top/gteijbdhui.html

[S57] C++：编译期常量
来源：http://hz.redwolf501.top/gtzdifqgig.html

constexpr int N = 10;
来源：http://hz.zhijiandao.cn/gtvrarkext.html

[S58] C++：命名空间
来源：http://hz.ydzc1.top/gtzhhsscsd.html

namespace ns { int f() { return 1; } }
来源：http://hz.kuanghao11.cn/gtxojqptty.html

[S59] C++：静态断言
来源：http://hz.316326.xyz/gtemnfirgw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sxryk.cn/gtbuacbwqx.html

[S60] C++：遍历并删除元素
来源：http://hz.yongpay.top/gtzfeytggj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jianghu66.top/gtyfpowvtr.html

================================================================================
来源：http://hz.yvedp.cn/gtonbpsxyv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.wangdashe.top/gtzvwsqzyq.html

================================================================================
来源：http://hz.zhongyouzk.top/gttspkxwjh.html

[T01] Kotlin：Hello World
来源：http://hz.feifeiyinyue.top/gtytupasok.html

println("Hello")
来源：http://hz.hysaishi.cn/gtwgdxnsfo.html

[T02] Kotlin：变量
来源：http://hz.hfpthk.cn/gtlwszpwjk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.52xcode.cn/gtfikbkwxr.html

[T03] Kotlin：字符串模板
来源：http://hz.iojbl.cn/gtkslxgjrz.html

"值: $b"
来源：http://hz.hammf.cn/gtczendpgo.html

[T04] Kotlin：空安全
来源：http://hz.hfpthk.cn/gtolxgaxii.html

val n: String? = null;  n?.length
来源：http://hz.havefunace.top/gtrlnbrlyk.html

[T05] Kotlin：when 表达式
来源：http://hz.feifeiyinyue.top/gtwszupvlu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hnxiangtu.top/gtfkzuwdyh.html

[T06] Kotlin：集合映射
来源：http://hz.jinghuilouyu.cn/gtknekdeev.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jiagoushi.top/gtrfzjyzax.html

[T07] Kotlin：集合过滤
来源：http://hz.yueranfly.top/gtsnjjmiri.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cheryme.top/gtyebrrrew.html

[T08] Kotlin：数据类
来源：http://hz.sxryk.cn/gtssrlqpbt.html

data class User(val name: String, val age: Int)
来源：http://hz.cheryme.top/gteggmfmtt.html

[T09] Kotlin：扩展函数
来源：http://hz.hfpthk.cn/gtwiafqiri.html

fun String.exclaim() = this + "!"
来源：http://hz.tanke756.top/gtuxidvwvu.html

[T10] Kotlin：默认参数
来源：http://hz.hfpthk.cn/gtuwhamgdb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.daxiang520.top/gtkpgxgixu.html

[T11] Kotlin：协程
来源：http://hz.dianchejie.cn/gtjeiutfih.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.tanke756.top/gtoyyppeqv.html

[T12] Kotlin：解构声明
来源：http://hz.meibo888.top/gtwrjyyytp.html

val (a, b) = Pair(1, 2)
来源：http://hz.bjfxy.top/gtzrjembfp.html

[T13] Kotlin：只读 Map
来源：http://hz.hongshengwenyu.top/gtrbxebqfx.html

val m = mapOf("a" to 1)
来源：http://hz.jlsjyb.cn/gtetdmbqqq.html

[T14] Kotlin：循环
来源：http://hz.aizwys.cn/gtblqcdkrv.html

for (i in 1..10) println(i)
来源：http://hz.pengpengdd.cyou/gtkiadcwrb.html

[T15] Kotlin：接口
来源：http://hz.hfpthk.cn/gtwjhhcdyq.html

interface Shape { fun area(): Double }
来源：http://hz.jinyuanbaomall.cn/gtmkweflpa.html

[T16] Swift：Hello World
来源：http://hz.andypj.xyz/gtwybwcyhf.html

print("Hello")
来源：http://hz.shzxlz.cn/gtcyzsqdus.html

[T17] Swift：变量与常量
来源：http://hz.hnxiangtu.top/gtmipxetgv.html

var a = 1;  let b = 2
来源：http://hz.cucudq.cn/gteggiskul.html

[T18] Swift：字符串插值
来源：http://hz.sysykeji.top/gtnxpzqcsv.html

"值: \(b)"
来源：http://hz.jqgufenzy.top/gtemghyhra.html

[T19] Swift：可选绑定
来源：http://hz.aibaodan.cn/gtqvdqniwa.html

if let n = opt { print(n) }
来源：http://hz.kuanghao11.cn/gthqhfpknz.html

[T20] Swift：数组操作
来源：http://hz.yj20258.top/gtckumvnht.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.hammf.cn/gtjqudmlnv.html

[T21] Swift：遍历
来源：http://hz.ydzc1.top/gtvedmdjgo.html

for x in a { print(x) }
来源：http://hz.snrcjt.cn/gtjnpvwwbl.html

[T22] Swift：字典
来源：http://hz.jiagoushi.top/gthisighyr.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.tianlin.xyz/gtxkrptqtl.html

[T23] Swift：函数
来源：http://hz.yj20258888.top/gtjqweiufy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.dashuyun.cn/gtgnlwknbz.html

[T24] Swift：闭包
来源：http://hz.chenjidiqi.icu/gterfhyypp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.ppjwa.cn/gtalmvodyh.html

[T25] Swift：结构体
来源：http://hz.mhx1999.top/gtxervytvu.html

struct P { var x: Int }
来源：http://hz.gaohongyu789.top/gtuepxetsf.html

[T26] Swift：类与重写
来源：http://hz.zhengqikj.top/gtbmgintch.html

class A: Base { override func f() {} }
来源：http://hz.fzhhl.top/gtbyidwaad.html

[T27] Swift：错误处理
来源：http://hz.jinqigufen.top/gtsuprlvpg.html

do { try f() } catch { print(error) }
来源：http://hz.ywan-chungtsiang.top/gtfkjtsiyx.html

[T28] Swift：枚举
来源：http://hz.nanxinkj.top/gtpepkfxem.html

enum Color { case red, green }
来源：http://hz.feifeiyinyue.top/gtwlpfzpcl.html

[T29] Swift：guard 提前返回
来源：http://hz.cucudq.cn/gtshwiwias.html

guard let x = opt else { return }
来源：http://hz.daria6918.cn/gtclupbvjn.html

[T30] Swift：协议
来源：http://hz.shuidangran.top/gtovsyaugc.html

protocol Shape { func area() -> Double }
来源：http://hz.0kj1m.cn/gtqbuarmvs.html

[T31] Lua：Hello World
来源：http://hz.hywenlv.cn/gtcaosgdwn.html

print("Hello")
来源：http://hz.hfpthk.cn/gtyhqoioip.html

[T32] Lua：局部变量
来源：http://hz.316326.xyz/gtdxdnfimb.html

local a = 1
来源：http://hz.tianlin.xyz/gtfgfruxix.html

[T33] Lua：表（数组）
来源：http://hz.cucudq.cn/gtajjwgzja.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zdqjudy.top/gtzvaxriwf.html

[T34] Lua：遍历表
来源：http://hz.zhaomingkeji.xyz/gtlfedemue.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.xinyue.icu/gtogbjwmba.html

[T35] Lua：字典表
来源：http://hz.jinqigfzy.top/gtzwhiwvzr.html

local d = { a = 1 };  d.b = 2
来源：http://hz.wangshuangyany.cn/gtrblpgovl.html

[T36] Lua：函数
来源：http://hz.sysykeji.top/gtfwqtkbiq.html

function add(a, b) return a + b end
来源：http://hz.kuanghao11.cn/gttydkruah.html


<!-- 参考信息 -->