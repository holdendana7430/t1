代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhengqikj.top/gtotsfjthl.html

[R36] 并发执行多个任务
来源：http://hz.hongshengwenyu.top/gtivqphedh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jinqigfzy.top/gtozbalhnb.html

[R37] 把输出赋给变量
来源：http://hz.zhixingplan.top/gtiahfserp.html

files=$(ls -1)
来源：http://hz.jiagoushi.top/gtxxcekgvy.html

[R38] 管道串联
来源：http://hz.cdnleiting.top/gtezxndsai.html

cat a.txt | grep -i error | wc -l
来源：http://hz.sxryk.cn/gtexxobqbr.html

[R39] 重定向标准输出与错误
来源：http://hz.svipenyu.cn/gtqpbkznov.html

cmd > out.log 2>&1
来源：http://hz.zycfv.cn/gtkkjjwwgj.html

[R40] 追加写日志
来源：http://hz.dashuyun.cn/gtvwzjvwtw.html

echo "log" >> out.log
来源：http://hz.ywan-chungtsiang.top/gtcntmmtvo.html

[R41] 丢弃输出
来源：http://hz.yj20258888.top/gtflirwkhr.html

cmd >/dev/null 2>&1
来源：http://hz.pycfn.com/gtxtrwkpge.html

[R42] 输入重定向
来源：http://hz.jqgufenzy.top/gtkjkhaixp.html

wc -l < a.txt
来源：http://hz.nanxinkj.top/gtkeubyfck.html

[R43] 按名字查找文件
来源：http://hz.xylfe.cn/gtjpoxtblr.html

find . -name "*.log" -type f
来源：http://hz.xinyue.icu/gtcupcsref.html

[R44] 按修改时间查找
来源：http://hz.cashguo.top/gtxbjppges.html

find . -mtime -7 -type f
来源：http://hz.gaohongyu789.top/gtlzllprfs.html

[R45] 批量删除
来源：http://hz.xuanzx.com/gtoahjtody.html

find . -name "*.tmp" -delete
来源：http://hz.ehwqpu.com/gtyjnfshnx.html

[R46] 递归替换文件内容
来源：http://hz.316326.xyz/gtbntpcnvg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.shanyushiyangtech.top/gtewotzgkh.html

[R47] sed 单行替换
来源：http://hz.jqgufenzy.top/gtqzcbigok.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.sweek.top/gtdiwakhpm.html

[R48] awk 取指定列
来源：http://hz.zhixingplan.top/gtjklkwzib.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhijiandao.cn/gtlymgnsge.html

[R49] awk 带条件
来源：http://hz.redwolf501.top/gtndzgjlsf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.shanyushiyangkeji.top/gtrskjjxlo.html

[R50] awk 求和
来源：http://hz.ivvv.top/gtjptckepk.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shuidangran.top/gtgyyefhzz.html

[R51] 排序去重取前几
来源：http://hz.aibaodan.cn/gtollbwdkz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.aizwys.cn/gtzripkspu.html

[R52] 统计行数
来源：http://hz.zhoulong.xyz/gtftwytlsn.html

wc -l a.txt
来源：http://hz.gogol.net.cn/gtewnhjyhg.html

[R53] 查看文件头与实时尾
来源：http://hz.jqgfzy.top/gtlxvwtazd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hfpthk.cn/gtgnvegclj.html

[R54] 比较两个文件
来源：http://hz.jiagoushi.top/gtqsugjnhs.html

diff a.txt b.txt
来源：http://hz.zycfv.cn/gtffcwmwcv.html

[R55] 压缩与解压
来源：http://hz.pycfn.com/gtbpkhtsja.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.quarkkingdee.top/gthxjykpob.html

[R56] 远程拷贝
来源：http://hz.wangshuangyany.cn/gtmdugovyf.html

scp file user@host:/path/
来源：http://hz.ppjwa.cn/gtomjilgva.html

[R57] 远程执行命令
来源：http://hz.zycfv.cn/gtexyteekx.html

ssh user@host 'uptime'
来源：http://hz.sysykeji.top/gtjojbsvbe.html

[R58] 下载文件
来源：http://hz.52xcode.cn/gtjrwmgkvc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.sxryk.cn/gtmxpinema.html

[R59] 发 POST JSON
来源：http://hz.ppjwa.cn/gtderxjcfx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shuidangran.top/gtrdtplgsp.html

[R60] 只看 HTTP 状态码
来源：http://hz.ehwqpu.com/gtnapczrxs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.mhx1999.top/gtzmorgxhh.html

[R61] 磁盘占用
来源：http://hz.daria6918.cn/gtuargwdiw.html

df -h;  du -sh *
来源：http://hz.yanxiufei.cn/gtbjlgrbba.html

[R62] 找最占空间的文件
来源：http://hz.pengpengdd.cyou/gtfkagdpot.html

du -ah . | sort -rh | head -10
来源：http://hz.9152youxi.cn/gtufvvoqlf.html

[R63] 内存与进程
来源：http://hz.guowangkeji.top/gtguqmwvho.html

free -h;  ps aux | grep nginx
来源：http://hz.shanyushiyangkeji.top/gtatnbxrxd.html

[R64] 结束进程
来源：http://hz.zhiwuduotai.top/gtczpzvboa.html

kill -9 $(pgrep -f app.py)
来源：http://hz.c1oappe.top/gtyxtqmsbo.html

[R65] 查看端口占用
来源：http://hz.ppjwa.cn/gtriqilmib.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.iojbl.cn/gtzajtcqzj.html

[R66] 定时任务
来源：http://hz.shanyushiyangtech.top/gthgrnrfpw.html

crontab -e;  crontab -l
来源：http://hz.jinqigufen.top/gtvmgnoeps.html

[R67] 生成随机十六进制串
来源：http://hz.pengpengdd.cyou/gthmdwhjyv.html

openssl rand -hex 16
来源：http://hz.andypj.xyz/gtipnhlkpx.html

[R68] 计算文件校验值
来源：http://hz.cqqwz.cn/gtzjsjugum.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ivvv.top/gtylihfpcw.html

[R69] 生成随机密码
来源：http://hz.chenjidiqi.icu/gtylfqkrrl.html

head -c 16 /dev/urandom | base64
来源：http://hz.yvedp.cn/gttlfimujs.html

[R70] 时间戳与互转
来源：http://hz.zycfv.cn/gtgokmckfo.html

date +%s;  date -d @1700000000
来源：http://hz.zycfv.cn/gtagnfhvgg.html

[R71] 日期格式化
来源：http://hz.yuanzhike.top/gtzjkoqfza.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hfpthk.cn/gtajwtdsoa.html

[R72] 等待端口就绪
来源：http://hz.jianghu66.top/gtowdirfcn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hammf.cn/gtixvvzmmy.html

[R73] 分割大日志
来源：http://hz.dashuyun.cn/gtdpwjrgor.html

split -l 1000 big.log part_
来源：http://hz.sxryk.cn/gtdgozupeo.html

[R74] 批量重命名
来源：http://hz.chenjidiqi.icu/gticehczbd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.vqdsnc.cn/gtbaplyzsj.html

[R75] 导出环境变量
来源：http://hz.shangyingyoupin.top/gtawxwefhk.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.gaohongyu789.top/gtkybzmztm.html

[R76] 使用临时文件
来源：http://hz.zhixingplan.top/gtezsrtxho.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ppjwa.cn/gtkgoypcku.html

[R77] 读取用户输入
来源：http://hz.fzhhl.top/gtvwcpyien.html

read -rp "请输入: " ans
来源：http://hz.hysaishi.cn/gtotishqkl.html

[R78] 交互式菜单
来源：http://hz.quarkkingdee.top/gtyazmuyrk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hfpthk.cn/gtgtvnfgzc.html

[R79] 解析命令行选项
来源：http://hz.haohaochexian.top/gtsdmpzhzl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hywenlv.cn/gtovvixkxi.html

[R80] 查看脚本执行耗时
来源：http://hz.havefunace.top/gtyaytaubb.html

time ./run.sh
来源：http://hz.cdnleiting.top/gtgdqjfztt.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtwaatlqli.html

S. C / C++ 专题
来源：http://hz.yvedp.cn/gtbudohefg.html

================================================================================
来源：http://hz.sxryk.cn/gtuvffpwkp.html

[S01] C：Hello World
来源：http://hz.zhijiandao.cn/gtstxgdzgw.html

#include <stdio.h>
来源：http://hz.jinghuilouyu.cn/gtmodlphih.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.316326.xyz/gtinlxcpsj.html

[S02] C：变量与格式化输出
来源：http://hz.snrcjt.cn/gthxiskygb.html

int a = 10; printf("%d\n", a);
来源：http://hz.kuanghao11.cn/gtwlsatgyd.html

[S03] C：读入整数
来源：http://hz.ppjwa.cn/gtzpwujtvp.html

int x; scanf("%d", &x);
来源：http://hz.hfpthk.cn/gtpkyzkwju.html

[S04] C：字符串复制
来源：http://hz.feifeiyinyue.top/gthnigufkr.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yanxiufei.cn/gtoxyormwd.html

[S05] C：字符串长度
来源：http://hz.xingfuxueyuan.xyz/gtwsxziydf.html

strlen(s)
来源：http://hz.shanyushiyangkeji.top/gtlsknsqxl.html

[S06] C：字符串比较
来源：http://hz.yj20258888.top/gtgjnapjak.html

strcmp(a, b) == 0
来源：http://hz.cashguo.top/gtrvvkbimc.html

[S07] C：数组遍历求和
来源：http://hz.zdqjudy.top/gtwwrygxpi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.sysykeji.top/gtvkbybrsa.html

[S08] C：动态内存分配与释放
来源：http://hz.gotoacloud.top/gteyguvtlb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.nanxinkj.top/gtohfogorm.html

[S09] C：结构体定义与初始化
来源：http://hz.cqqwz.cn/gtoaoaazkt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cheryme.top/gttlixgtle.html

[S10] C：指针与解引用
来源：http://hz.ybcxt.top/gtoreifzge.html

int *p = &a;  *p = 5;
来源：http://hz.zhaomingkeji.xyz/gtbbpzomwm.html

[S11] C：逐行读文件
来源：http://hz.ybcxt.top/gtmbzqxtnn.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.cashguo.top/gtiehuiwqo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.tanke756.top/gtfgvxktfb.html

fclose(f);
来源：http://hz.ehwqpu.com/gtakhpopfz.html

[S12] C：写文件
来源：http://hz.fzhhl.top/gtgqnnqxkc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.tianlin.xyz/gtvywozidp.html

[S13] C：宏定义
来源：http://hz.zhixingplan.top/gtvoospusw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yangfankeji.com/gtlkvcegxp.html

[S14] C：枚举
来源：http://hz.gotoacloud.top/gtbubqmyfi.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hysaishi.cn/gtyvuxqjyo.html

[S15] C：类型转换
来源：http://hz.chenzaomai.com/gtmioofbpn.html

(double) a / b
来源：http://hz.aizwys.cn/gtmfmngigk.html

[S16] C：位操作置位
来源：http://hz.zhixingplan.top/gtxwsnkaec.html

x |= (1 << 3);
来源：http://hz.pengpengdd.cyou/gtsnqrdsyj.html

[S17] C：安全拼接字符串
来源：http://hz.hywenlv.cn/gtojxvstma.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ywan-chungtsiang.top/gtmxlnntcj.html

[S18] C：命令行参数
来源：http://hz.zhijiandao.cn/gtyesdfjok.html

int main(int argc, char **argv)
来源：http://hz.ybcxt.top/gtpktvyqku.html

[S19] C：快速排序
来源：http://hz.xziqi.cn/gtlcbluack.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hywenlv.cn/gtvyjxmwow.html

[S20] C：二分查找
来源：http://hz.zhijiandao.cn/gtprsxlypu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhaomingkeji.xyz/gtvewsxwwi.html

[S21] C：字符类别判断
来源：http://hz.jianghu66.top/gtojmvpepe.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.smart0.xyz/gtncqykvkr.html

[S22] C：字符串转数字
来源：http://hz.quarkkingdee.top/gtxgfcxjdx.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yj20258888.top/gthcntkwyc.html

[S23] C：随机数
来源：http://hz.zhiwuduotai.top/gtjsmzfdjj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.snrcjt.cn/gtsdotthvz.html

[S24] C：获取本地时间
来源：http://hz.gzhubu.top/gtpuyrsgvy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hnxiangtu.top/gtaiwiutzz.html

[S25] C：内存拷贝
来源：http://hz.aizwys.cn/gtsjdtzyzw.html

memcpy(dst, src, n);
来源：http://hz.yueranfly.top/gtxbyaifan.html

[S26] C：内存清零
来源：http://hz.jyoumei.cn/gtauiwolyy.html

memset(a, 0, sizeof a);
来源：http://hz.zhiwuduotai.top/gtnlxfbboq.html

[S27] C：定义常量
来源：http://hz.guannengcc.top/gtvriazhpr.html

const double PI = 3.14159;
来源：http://hz.wangdashe.top/gtjzzyjief.html

[S28] C：静态变量
来源：http://hz.zhongyouzk.top/gtnjtypcue.html

static int counter = 0;
来源：http://hz.dashuyun.cn/gtljylhcsu.html

[S29] C：变参函数
来源：http://hz.ywan-chungtsiang.top/gtfzwmljuq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.gaohongyu789.top/gtntydeyne.html

[S30] C：头文件保护
来源：http://hz.yuxming.cn/gtwbceftyr.html

#ifndef X_H
来源：http://hz.guowangkeji.top/gtpuzttrlb.html

#define X_H
来源：http://hz.sysykeji.top/gtqomfydpd.html

#endif
来源：http://hz.haohaochexian.top/gtwiknufqg.html

[S31] C++：Hello World
来源：http://hz.cqqwz.cn/gtnbpnayoc.html

#include <iostream>
来源：http://hz.shuidangran.top/gtwqamkofw.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xuanzx.com/gtsxdxhfwh.html

[S32] C++：字符串
来源：http://hz.yangfankeji.com/gtomplzzlh.html

std::string s = "hi";  s += "!";
来源：http://hz.yanxiufei.cn/gtaerkeche.html

[S33] C++：vector 增删
来源：http://hz.shanyushiyangkeji.top/gtrqjiefzo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hnxiangtu.top/gtxwptkrxr.html

[S34] C++：遍历 vector
来源：http://hz.xziqi.cn/gtnhkiuvdv.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ppjwa.cn/gthtzgyjdl.html

[S35] C++：map
来源：http://hz.ywan-chungtsiang.top/gtdryhggut.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shuidangran.top/gtaejyyrcd.html

[S36] C++：unordered_map
来源：http://hz.0kj1m.cn/gtisayhvbc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.wangdashe.top/gtsdczrzia.html

[S37] C++：set
来源：http://hz.chenzaomai.com/gtcicvlvvh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ppjwa.cn/gtxntfgsay.html

[S38] C++：排序
来源：http://hz.hongshengwenyu.top/gtxkvhuxpw.html

std::sort(v.begin(), v.end());
来源：http://hz.yj20258.top/gthkardpkq.html

[S39] C++：自定义比较器排序
来源：http://hz.hysaishi.cn/gtnwfbgkxe.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.fengsongda.top/gtvqdcrtgs.html

[S40] C++：查找元素
来源：http://hz.yuxming.cn/gtlfplszft.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.nanxinkj.top/gtispkfhpx.html

[S41] C++：类与构造函数
来源：http://hz.andypj.xyz/gtxrtjvqyg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yanxiufei.cn/gtepbrrcto.html

[S42] C++：继承与虚函数
来源：http://hz.shuidangran.top/gtgupkyxqr.html

class B : public Base { public: void f() override {} };
来源：http://hz.316326.xyz/gtadehugok.html

[S43] C++：智能指针
来源：http://hz.cheryme.top/gtatogayuy.html

auto p = std::make_unique<int>(5);
来源：http://hz.snrcjt.cn/gtoouvwski.html

[S44] C++：引用传参
来源：http://hz.xuetiantiany.cn/gtpvsojfhm.html

void inc(int &x) { ++x; }
来源：http://hz.cashguo.top/gtooiaugsd.html

[S45] C++：lambda
来源：http://hz.zhijiandao.cn/gtzikxmpwl.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.andypj.xyz/gtqiejfzbp.html

[S46] C++：函数模板
来源：http://hz.gogol.net.cn/gtwqmkqjmm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.cashguo.top/gthchqsods.html

[S47] C++：结构化绑定遍历
来源：http://hz.hywenlv.cn/gtvnhkouvq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.gogol.net.cn/gtxohlrvkb.html

[S48] C++：逐行读文件
来源：http://hz.c1oappe.top/gtclhpcoks.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yonumen.top/gtstokotfr.html

while (std::getline(in, line)) { }
来源：http://hz.xylfe.cn/gtypxjsyei.html

[S49] C++：写文件
来源：http://hz.bjfxy.top/gtvvknjtbu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.gotoacloud.top/gtpdvermlp.html

[S50] C++：格式化数字
来源：http://hz.xylfe.cn/gtgeucpxbp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.nanxuanxn.top/gterewlgar.html

[S51] C++：显式类型转换
来源：http://hz.zhongyouzk.top/gtxgtxwsjw.html

static_cast<double>(a) / b
来源：http://hz.shuidangran.top/gtshfstiio.html

[S52] C++：const 与 noexcept
来源：http://hz.nanxinkj.top/gtuspmytjk.html

int size() const noexcept { return n_; }
来源：http://hz.hnqzz.top/gtibzvwfps.html

[S53] C++：移动语义
来源：http://hz.haohaochexian.top/gtiiruzeaq.html

std::vector<int> w = std::move(v);
来源：http://hz.ivvv.top/gtccrjfjuz.html

[S54] C++：异常处理
来源：http://hz.yongpay.top/gtutpsjonu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jinyuanbaomall.cn/gtcjbufvly.html

[S55] C++：结构化绑定
来源：http://hz.yj20258888.top/gtmcfmrtla.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zycfv.cn/gtsvsavali.html

[S56] C++：optional
来源：http://hz.zhoulong.xyz/gtijptstah.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jyoumei.cn/gtpamtbttj.html

[S57] C++：编译期常量
来源：http://hz.svipenyu.cn/gtwcoogncm.html

constexpr int N = 10;
来源：http://hz.pycfn.com/gtvxlvpkbp.html

[S58] C++：命名空间
来源：http://hz.haohaochexian.top/gtsohcfror.html

namespace ns { int f() { return 1; } }
来源：http://hz.hammf.cn/gtefqidenm.html

[S59] C++：静态断言
来源：http://hz.yj202588.top/gtihtbzmzf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shanyushiyangkeji.top/gtyuzgdpaz.html

[S60] C++：遍历并删除元素
来源：http://hz.ywan-chungtsiang.top/gteyacsnch.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.andypj.xyz/gtcukgvrlh.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gthzipnldy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gogol.net.cn/gtkugszeog.html

================================================================================
来源：http://hz.zycfv.cn/gtspqdscyc.html

[T01] Kotlin：Hello World
来源：http://hz.haohaochexian.top/gtqiqxgesh.html

println("Hello")
来源：http://hz.jqgufenzy.top/gtaogotzkf.html

[T02] Kotlin：变量
来源：http://hz.shuidangran.top/gtsxggsxyi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.nanxuanxn.top/gtttgbsnga.html

[T03] Kotlin：字符串模板
来源：http://hz.jinghuilouyu.cn/gtnnkgkiuh.html

"值: $b"
来源：http://hz.0kj1m.cn/gtcqrdumav.html

[T04] Kotlin：空安全
来源：http://hz.jqgfzy.top/gtrawjonbz.html

val n: String? = null;  n?.length
来源：http://hz.vqdsnc.cn/gtekawswza.html

[T05] Kotlin：when 表达式
来源：http://hz.shangyingyoupin.top/gtkddttmxf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.daxiang520.top/gtchvwodij.html

[T06] Kotlin：集合映射
来源：http://hz.chenzaomai.com/gtdxnyqjak.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhiwuduotai.top/gtdwhyhmdl.html

[T07] Kotlin：集合过滤
来源：http://hz.ybcxt.top/gtzklfvegc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.wangshuangyany.cn/gtzipdyhgf.html

[T08] Kotlin：数据类
来源：http://hz.52xcode.cn/gtqrjjwjhy.html

data class User(val name: String, val age: Int)
来源：http://hz.chenzaomai.com/gtdpoohicg.html

[T09] Kotlin：扩展函数
来源：http://hz.ydzc1.top/gtgvqvhgnk.html

fun String.exclaim() = this + "!"
来源：http://hz.hnqzz.top/gtfdrnziye.html

[T10] Kotlin：默认参数
来源：http://hz.tanke756.top/gthwvnyikj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hammf.cn/gtpgiwxisn.html

[T11] Kotlin：协程
来源：http://hz.xuanzx.com/gtdgxopeiu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zycfv.cn/gtqdrqwvuf.html

[T12] Kotlin：解构声明
来源：http://hz.316326.xyz/gtwlbvbddm.html

val (a, b) = Pair(1, 2)
来源：http://hz.9152youxi.cn/gtsekcfdvc.html

[T13] Kotlin：只读 Map
来源：http://hz.svipenyu.cn/gtkserlzbu.html

val m = mapOf("a" to 1)
来源：http://hz.zhiwuduotai.top/gtltufszrg.html

[T14] Kotlin：循环
来源：http://hz.zhoulong.xyz/gtjrfbhlwe.html

for (i in 1..10) println(i)
来源：http://hz.guowangkeji.top/gtgsxnnnuj.html

[T15] Kotlin：接口
来源：http://hz.zhixingplan.top/gtondmbzrh.html

interface Shape { fun area(): Double }
来源：http://hz.ywan-chungtsiang.top/gtxdlrvxxv.html

[T16] Swift：Hello World
来源：http://hz.nwbrower.top/gtyduxoprd.html

print("Hello")
来源：http://hz.ydzc1.top/gttgkcclmc.html

[T17] Swift：变量与常量
来源：http://hz.zhengqikj.top/gtbrcmsise.html

var a = 1;  let b = 2
来源：http://hz.zhengqikj.top/gtvxxoqbor.html

[T18] Swift：字符串插值
来源：http://hz.gaohongyu789.top/gtiohpmxtz.html

"值: \(b)"
来源：http://hz.cdnleiting.top/gtsylzatfn.html

[T19] Swift：可选绑定
来源：http://hz.xinyue.icu/gtbaazfbdy.html

if let n = opt { print(n) }
来源：http://hz.cdnleiting.top/gtrywrfjnq.html

[T20] Swift：数组操作
来源：http://hz.cqqwz.cn/gtixebcweb.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.wangdashe.top/gtpgzwdsay.html

[T21] Swift：遍历
来源：http://hz.tian-w.cn/gtwirsvrii.html

for x in a { print(x) }
来源：http://hz.fzhhl.top/gtdmfzqlio.html

[T22] Swift：字典
来源：http://hz.ydjk.org.cn/gtxyvwvyxt.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zycfv.cn/gtkuwzeaiq.html

[T23] Swift：函数
来源：http://hz.gotoacloud.top/gtfnzhvckq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.gaohongyu789.top/gtvnwqfkjj.html

[T24] Swift：闭包
来源：http://hz.bjfxy.top/gtecbxsihi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhongyouzk.top/gtxanpgszg.html

[T25] Swift：结构体
来源：http://hz.hammf.cn/gtoscuctnm.html

struct P { var x: Int }
来源：http://hz.sysykeji.top/gtwbdgigzn.html

[T26] Swift：类与重写
来源：http://hz.ppjwa.cn/gtwdrfvfxc.html

class A: Base { override func f() {} }
来源：http://hz.yangfankeji.com/gtobkscfyn.html

[T27] Swift：错误处理
来源：http://hz.jianghu66.top/gtwgiwerhd.html

do { try f() } catch { print(error) }
来源：http://hz.yj202588.top/gthoqtczwb.html

[T28] Swift：枚举
来源：http://hz.shzxlz.cn/gttnhfsaki.html

enum Color { case red, green }
来源：http://hz.jinghuilouyu.cn/gtrrxseqvs.html

[T29] Swift：guard 提前返回
来源：http://hz.cheryme.top/gtmjmdxsle.html

guard let x = opt else { return }
来源：http://hz.gzhubu.top/gtzvkyjyju.html

[T30] Swift：协议
来源：http://hz.xuetiantiany.cn/gtvponbvoa.html

protocol Shape { func area() -> Double }
来源：http://hz.shanyushiyangkeji.top/gtnplrjkbt.html

[T31] Lua：Hello World
来源：http://hz.dashuyun.cn/gtcidcbosd.html

print("Hello")
来源：http://hz.jinghuilouyu.cn/gtjuljulyz.html

[T32] Lua：局部变量
来源：http://hz.andypj.xyz/gtrvbtaerh.html

local a = 1
来源：http://hz.mhx1999.top/gtcaibpred.html

[T33] Lua：表（数组）
来源：http://hz.hysaishi.cn/gtcuzzeiax.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jinqigufen.top/gtgpuapvqg.html

[T34] Lua：遍历表
来源：http://hz.iojbl.cn/gtzdotsvbb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.andypj.xyz/gtwciaqggm.html

[T35] Lua：字典表
来源：http://hz.gaohongyu789.top/gtowfeikfs.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jinghuilouyu.cn/gtbwxmwijd.html

[T36] Lua：函数
来源：http://hz.hfpthk.cn/gtieswdonq.html

function add(a, b) return a + b end
来源：http://hz.jinqigufen.top/gtspujauvy.html

[T37] Lua：字符串拼接
来源：http://hz.meibo888.top/gtelfdmmti.html

"a" .. "b"
来源：http://hz.jinghuilouyu.cn/gtlhvumvex.html

[T38] Lua：条件
来源：http://hz.vqdsnc.cn/gtxamzrbey.html

if x > 0 then print("正") end
来源：http://hz.quarkkingdee.top/gtonrossxl.html


<!-- 参考信息 -->